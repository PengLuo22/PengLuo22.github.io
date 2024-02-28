---
title: Redis分布式锁
date: 2024-2-28 21:00:00 +0800
categories: [分布式,分布式锁]
tags: [Redis, 分布式锁]     # TAG names should always be lowercase
toc: true
---

## 为什么有分布式锁？
使用分布式锁的目的，无外乎就是保证**同一时间**只有一个客户端可以对**共享资源**进行操作。比如常见的有：
* 秒杀场景，使用分布式锁避免超卖；
* 级联删除批次
* 分布式全局唯一ID生成器
* 发起批次计算

## Redis分布式锁
分布式锁的解决方案有很多，Redis分布式锁无疑是最佳实践，工作中经常打交道，所以本文来聊聊。

### 经典的写法

```java

```








## FAQ



## See Also

1. https://javaguide.cn/distributed-system/distributed-lock.html
2. 
