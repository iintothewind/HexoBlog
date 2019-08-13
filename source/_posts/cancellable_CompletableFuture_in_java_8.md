---
title: cancellable CompletableFuture in java 8
date: 2019-08-13 14:42:50
tags: java
---

## reason

`CompletableFuture` is a useful tool introduced since java 8.
It provides many convenient methods for concurrency handling.
Yet it did not support task cancelling in java 8 version.

Two new methods were added to `CompletableFuture` since java 9 to support timeout:

```java
public CompletableFuture<T> orTimeout(long timeout, TimeUnit unit)
public CompletableFuture<T> completeOnTimeout(T value, long timeout, TimeUnit unit)
```


### CompletableFuture.orTimeout() in java 9

A `CompletableFuture` would be completed exceptionally with `TimeoutException` if it did not complete with a `result` within given timeout.
The timeout feature was implemented by using two static final classes `Delayer` and `Timeout`.

```java
public CompletableFuture<T> orTimeout(long timeout, TimeUnit unit) {
  if (unit == null)
      throw new NullPointerException();
  if (result == null)
      whenComplete(new Canceller(Delayer.delay(new Timeout(this), timeout, unit)));
  return this;
}
```

If `result` is not given, The `CompletableFuture.completeExceptionally()` for current instance will be called in a scheduled task created by `Delayer.delay()` after the given timeout.

## solution in java 8

first we need to create a `CompletableFuture` named `promise` which always fails with `TimeoutException` after given timeout.
We can reuse the code implementation of `Delayer` and `Timeout` in java 9 to fail the created `promise`.

The always-fail `CompletableFuture` can be implemented as:
```java
final CompletableFuture<T> promise = new CompletableFuture<>();
Delayer.delay(new Timeout(promise), duration.toMillis(), TimeUnit.MILLISECONDS);
```

Then we can use `CompletableFuture.applyToEither()` to combine the results:
```java
static <T> CompletableFuture<T> within(CompletableFuture<T> completableFuture, Duration duration) {
  Objects.requireNonNull(completableFuture, "completableFuture is required");
  Objects.requireNonNull(duration, "duration is required");
  final CompletableFuture<T> promise = new CompletableFuture<>();
  Delayer.delay(new Timeout(promise), duration.toMillis(), TimeUnit.MILLISECONDS);
  return completableFuture.applyToEither(promise, Function.identity());
}
```

For `within()` method, it takes a `completableFuture` and returns a `CompletableFuture` instance when the input `completableFuture` is completed. However if it takes too long to completed the input `completableFuture`, `promise` will be returned as output after the given `duration`,
`TimeoutException` will be thrown in its completed result.

## sample code

```java
@Test
public void testCancellableFuture() {
  CompletableFuture<String> future = CompletableFuture.supplyAsync(() -> {
    try {
      TimeUnit.MILLISECONDS.sleep(100);
    } catch (InterruptedException e) {
      Throwables.throwIfUnchecked(e);
    }
    return "this is a message";
  });

  final CompletableFuture<String> cancellable1 = CancellableFuture.within(future, Duration.ofMillis(50));
  final CompletableFuture<String> cancellable2 = CancellableFuture.within(future, Duration.ofMillis(200));
  cancellable1.whenComplete((s, throwable) -> {
    if (s != null) {
      log.info("s == {}", s);
    } else {
      log.info(throwable.getMessage());
    }
  });
  cancellable2.whenComplete((s, throwable) -> {
    if (s != null) {
      log.info("s == {}", s);
    } else {
      log.info(throwable.getMessage());
    }
  });
}
```

output:
```
2019-08-13 16:20:20.998 [CompletableFutureDelayScheduler] INFO  sample.concurrent.CompletableFutureSample - java.util.concurrent.TimeoutException
2019-08-13 16:20:21.039 [ForkJoinPool.commonPool-worker-3] INFO  sample.concurrent.CompletableFutureSample - s == this is a message
```



## implementation for `CancellableFuture`


```java
import java.time.Duration;
import java.util.Objects;
import java.util.concurrent.*;
import java.util.function.Function;

public interface CancellableFuture {

  static <T> CompletableFuture<T> within(CompletableFuture<T> completableFuture, Duration duration) {
    Objects.requireNonNull(completableFuture, "completableFuture is required");
    Objects.requireNonNull(duration, "duration is required");
    final CompletableFuture<T> promise = new CompletableFuture<>();
    Delayer.delay(new Timeout(promise), duration.toMillis(), TimeUnit.MILLISECONDS);
    return completableFuture.applyToEither(promise, Function.identity());
  }

  /**
   * Action to completeExceptionally on timeout
   * copy from `java.util.concurrent.CompletableFuture.Timeout` in java 9 JDK
   */
  final class Timeout implements Runnable {
    final CompletableFuture<?> future;

    Timeout(CompletableFuture<?> f) {
      this.future = f;
    }

    @Override
    public void run() {
      if (future != null && !future.isDone()) {
        future.completeExceptionally(new TimeoutException());
      }
    }
  }

  /**
   * Singleton delay scheduler, used only for starting and cancelling tasks.
   * copy from `java.util.concurrent.CompletableFuture.Delayer` in java 9 JDK
   */
  final class Delayer {
    static final ScheduledThreadPoolExecutor delayer;

    static {
      (delayer = new ScheduledThreadPoolExecutor(1, new DaemonThreadFactory())).setRemoveOnCancelPolicy(true);
    }

    static final class DaemonThreadFactory implements ThreadFactory {
      @Override
      public Thread newThread(Runnable runnable) {
        Thread t = new Thread(runnable);
        t.setDaemon(true);
        t.setName("CompletableFutureDelayScheduler");
        return t;
      }
    }

    static ScheduledFuture<?> delay(Runnable command, long delay, TimeUnit unit) {
      return delayer.schedule(command, delay, unit);
    }
  }
}
```

## reference
[Asynchronous Timeouts with CompletableFuture](https://dzone.com/articles/asynchronous-timeouts)
