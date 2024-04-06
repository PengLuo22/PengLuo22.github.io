---
title: C语言学习笔记
date: 2024-4-6 13:00:00 +0800
categories: [基本功,编程语言]
tags: [c]     # TAG names should always be lowercase
toc: true
---

## Hello world

练习：在命令行使用 gcc 编译、运行一个 C 程序

1、新建一个源文件 a.c

```shell
vim a.c
```

2、编辑a.c

```c
#include <stdio.h>

void  main() {
        printf("Hello world");
}
```

3、编译

```shell
gcc a.c
```

4、运行

```shell
./a.out
```

