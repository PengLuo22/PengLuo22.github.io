---
title: 如何搭建一个图床
date: 2024-4-6 13:00:00 +0800
categories: [Misc]
tags: [图床]     # TAG names should always be lowercase
toc: true
---

## 图床方案

本文主要采用的是 **[picGo+七牛云](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#%E5%9F%BA%E6%9C%AC%E6%93%8D%E4%BD%9C%E9%A2%84%E8%A7%88)**的方案，按照教程配置很容易实现。

然后上传了一个gif测试下，完美。

![](https://sbighb8sj.hn-bkt.clouddn.com/动画.gif)





## 遇到的问题

按照教程配置完后，出现了链接无法显示的问题。经过排查发现，是域名配置的问题。

![](https://sbighb8sj.hn-bkt.clouddn.com/Snipaste_2024-04-06_18-11-01.png)



文件上传的问题解决了，但是又有了 http://xxx.png is not an HTTPS link 的问题，这个问题之前就有遇到，当时选择不传http开头的链接避免了报错。



