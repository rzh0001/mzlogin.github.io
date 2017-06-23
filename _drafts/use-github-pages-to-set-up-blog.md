---
layout: post
title: 使用 Github Pages 写博客  
categories: [github pages, blog]
description: some word here
keywords: github, pages, jekyll
---


# List
<!-- vim-markdown-toc GFM -->
* [简介](#简介)
	* [准备使用的博文框架](#准备使用的博文框架)
* [购买域名](#购买域名)

<!-- vim-markdown-toc -->

## 简介
最近决定开始写博客，将自己的学习、成长与遭遇记录下来，同时也方便分享。本文主要目的是记录本次建立博客步骤。

### 准备使用的博文框架  
当有人叫我使用 Jekyll 搭建静态博客的时候，一开始我是拒绝的，不能你叫我用我就用，我得先试试，当我使用下来的时候，很柔，很亮。我用是这样子，你用也是这样子的。:smile:  



_当然喜欢从零开始的朋友，不妨根据 [Jekyll](http://jekyllcn.com/docs/quickstart/) 的教程搭建自己风格的博客。_

## 搭建过程

[安装 Jekyll](http://jekyllcn.com/docs/installation/)

## 创建博客

两种方式，一是根据[Jekyll](http://jekyllcn.com/docs/quickstart/) 的文档从零开始搭建自己风格的博客，二是直接在Github上找一个Jekyll Theme，在其基础上直接开始写博客。  

在下比较推荐第二种方式，先用起来再说，使用过程中再使用步步高打火机，哪里不爽点哪里。

1. 在 Github 上选一个喜欢主题 [点我免费传送](https://github.com/search?p=1&q=topic%3Ajekyll-theme&type=Repositories&utf8=%E2%9C%93)  
2. 直接下载该项目到本地，根据对应主题安装依赖后，`jekyll serve`看一下效果
3. Fork 该项目，将项目名改为 github_username.github.io，开启Github Pages。打开Pages的地址，看看博客是否正常。  
4. git clone 你的项目，修改 `_config.yml` 配置，删除原作者的文章。
