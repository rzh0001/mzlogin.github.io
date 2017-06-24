---
layout: post
title: Jekyll + Github Pages 搭建静态博客  
categories: [blog]
description: some word here
keywords: github, pages, jekyll, blog
music_id: 27588486
---

当有人叫我使用 Jekyll 搭建静态博客的时候，一开始我是拒绝的，不能你叫我用我就用。  我得先试试，当我使用下来的时候，很柔，很亮。我用是这样子，你用也是这样子的。:smile:  

# 文章目录
<!-- vim-markdown-toc GFM -->
* [搭建过程](#搭建过程)
	* [环境搭建](#环境搭建)
	* [创建博客](#创建博客)
	* [域名](#域名)
		* [域名购买](#域名购买)
		* [配置DNS解析](#配置dns解析)
		* [配置 CNAME](#配置-cname)

<!-- vim-markdown-toc -->

# 搭建过程

## 环境搭建

安装 Jekyll 运行需要的环境 [官方文档](http://jekyllcn.com/docs/installation/)

## 创建博客

使用 Jekyll 创建博客有两种方式：  
1. 根据 [Jekyll](http://jekyllcn.com/docs/quickstart/) 的文档从零开始搭建自己风格的博客
2. [在 Github 上找一个喜欢的 Jekyll Theme](https://github.com/search?p=1&q=topic%3Ajekyll-theme&type=Repositories&utf8=%E2%9C%93) ，在其基础上直接开始写博客。  

在下比较推荐第二种方式，先用起来再说，方便一些前段知识比较薄弱，只想安静写写文章的美男子/美女子。

1. [在 Github 上找一个喜欢的 Jekyll Theme](https://github.com/search?p=1&q=topic%3Ajekyll-theme&type=Repositories&utf8=%E2%9C%93)   
2. 直接下载该项目到本地，根据对应主题安装依赖后，`jekyll serve`看一下效果
3. Fork 该项目，将项目名改为 github_username.github.io，开启Github Pages。打开Pages的地址，看看博客是否正常。  
4. git clone 你的项目，修改 `_config.yml` 配置，删除原作者的文章。

## 域名
### 域名购买
如果你的自制力、**持久力**不足，还想坚持写博客，建议还是购买域名，越贵越好，钱花出去了总得用不是吗。:smile:  
我是在阿里云购买的域名，5块钱一年。域名需要实名验证，验证通过后即可通过域名访问。
### 配置DNS解析
首先得获取 博客主页的 IP 地址  
```
ping rzh0001.github.io
```
得到 Pages 的 IP 地址后，在`阿里云控制台->DNS管理->你的域名->解析列表`添加两条记录：@ 和 www。  参考下图  
![](/images/blog/dns-config.jpg)


### 配置 CNAME
在博客根目录下，新建一个文件 `CNAME`。内容为你购买的域名，不加 http
```
smily.space
```
至此，可以直接通过域名访问到博客了。 :smile:
 
