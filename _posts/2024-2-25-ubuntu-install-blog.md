---
title: ubuntu系统下搭建博客
date: 2024-2-25 07:30:00 +0800
categories: [技术文章, 编程]
tags: [博客]     # TAG names should always be lowercase
toc: true
---

## 前言
本文主要记录如何在ubuntu22.04系统上搭建博客，因为有之前在[window系统上搭建](https://pengluo22.github.io/posts/%E9%87%8D%E5%90%AF%E6%88%91%E7%9A%84%E5%8D%9A%E5%AE%A2/)的经验，所以在新环境上搭建非常顺利


## 搭建步骤

```shell

#安装ruby
sudo apt-get install ruby ruby-dev

#更换Gem sources，国外sources下载有问题。
#显示sources
gem sources 
sudo gem sources –r https://rubygems.org/
sudo gem sources –r http://rubygems.org/
sudo gem sources -a https://gems.ruby-china.com/
#更新source cache
gem sources -u 

sudo gem install jekyll
sudo gem install rdiscount
sudo gem install bundler

# 工作目录命令：安装博客仓库中所需的依赖
sudo bundle install

# 验证是否安装成功
jekyll -v

# 工作目录命令：将本地博客仓库跑起来
jekyll serve
```

访问  [http://127.0.0.1:4000](http://127.0.0.1:4000/) 即可


## 注意事项

搭建环境遇到各种报错是很正常的，可以通过询问 ChatGPT、查看 Github 仓库里 issue 里是否已经有回答等快速解决问题。

本次遇到的问题是下载依赖时没有写权限，使用sudo就完美解决了。

## 小结

此次在新环境本地部署博客，只花了1个小时的时间（包括解决遇到环境问题的时间），再一次体现到记录的巨大威力，感谢[曾经的自己](https://pengluo22.github.io/posts/%E9%87%8D%E5%90%AF%E6%88%91%E7%9A%84%E5%8D%9A%E5%AE%A2/)。


