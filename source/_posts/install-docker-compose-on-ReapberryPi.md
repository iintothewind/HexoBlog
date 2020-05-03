---
title: install docker-compose on ReapberryPi
date: 2020-05-03 17:13:37
tags: [linux]
---

Arm Arch based docker-compose is not officially provided.
To install it, we should use:

```bash
pip3 install --user docker-compose
```

Do not use `pip`, because some dependencies may not support python2.

