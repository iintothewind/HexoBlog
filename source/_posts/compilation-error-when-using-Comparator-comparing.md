---
title: compilation error when using Comparator.comparing()
date: 2019-12-10 18:13:12
tags: [java]
---

## the problem
First, lets take a look at the following code sample:

```java
Collections.sort(playlist, Comparator.comparing(s -> s.getTitle())
              .thenComparing(p1 -> p1.getDuration())
              .thenComparing(p1 -> p1.getArtist())
);
```

意图很简单, 给一个list按照三个不同的属性排序, 但是能编译通过吗?
答案是: 不能, 会出现编译错误.
JVM会抱怨不知道s是什么类型, p1是什么类型.

出现这个错误的原因是因为Java语言在类型推断上还是非常弱导致的。
你以为写第一个lambda( s->s.getTitle())时, java会知道遍历的对象是playlist里面的元素的类型, 其实不是, 它并不知道


## the solutions
有三种方法来解决这个问题:

### 用Java8的静态lambda表达式:

```java
Collections.sort(playlist, Comparator.comparing(Song::getTitle)
              .thenComparing(Song::getDuration)
              .thenComparing(Song::getArtist)
);
```

### 用临时变量显式调用

```java
Comparator<Song> byName = (s1, s2) -> s1.getArtist().compareTo(s2.getArtist());
Comparator<Song> byDuration = (s1, s2) -> Integer.compare(s1.getDuration(), s2.getDuration());
Collections.sort(playlist, byName.thenComparing(byDuration));
```


### 在comparing chain开始的时候加入泛型参数的显式声明

````java
Collections.sort(playlist, Comparator.<Song, String>comparing((s) -> s.getTitle())
              .thenComparing(p1 -> p1.getDuration())
              .thenComparing(p1 -> p1.getArtist())
);
```


## reference

[Very confused by Java 8 Comparator type inference](http://stackoverflow.com/questions/24436871/very-confused-by-java-8-comparator-type-inference)
