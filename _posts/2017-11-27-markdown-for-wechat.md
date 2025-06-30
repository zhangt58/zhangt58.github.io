---
title: "使用Markdown便捷微信公众平台文章写作"
subtitle: "Markdown for WeChat Official Account"
layout: post
date: 2017-11-27 09:41:38 AM EST
author: zhangt58
category: blog
hidden: true
tag:
- markdown
- wechat
---

### 引言

微信公众号平台是一个不错的写作平台，因为可以和微信这个中国最大的社交生态进行无缝的信息交流。但它的后台管理平台，特别是文章编辑发布差强人意，所以涌现了诸多第三方的应用软件来帮助广大写作者更快更好地发布他们的作品。对于其中的有些工具，功能已经太丰富，足足是另外一个生态了，回归写作的最原始出发点，无非就是以下做好以下两个方面：

1. 内容丰富，原创，言之有物
2. 排版漂亮，简单，赏心悦目

就第二点，Markdown是一个非常好的选择，因为公众号文章最后呈现的格式实际上是经过浏览器渲染后的，而写到编辑窗口的正是渲染后的结果（编辑窗口不支持HTML/CSS源码的直接输入），所以作者可以换个思路来做这个事情，那就是以其他的方式生成编辑窗口需要的输入。本文经过不断测试，总结了使用Markdown来简化公众号文章写作的主要步骤，可以让你专注文章的内容，而非格式。

### 使用Markdown的好处

- 专心写作，避免因来回操作鼠标进行格式排版带来的分心；
- 格式渲染独立于排版，可以通过更改CSS样式来适配自己的风格；
- 可以使用第三方的软件，或浏览器插件输出各种文档格式；
- 目前Markdown是各大写作平台，博客平台等的首要选择；

### 便捷公众号文章写作

因为Markdown写作的原文档，其最终的富文本展现形式，即在浏览器中呈现的文章，是依赖具体的样式渲染生成的，所以我们可以定义合适的样式。特别是针对微信公众号平台，不是所有的CSS样式都支持的，参考这个[微信样式](https://github.com/ayime/Markdown-here-CSS-for-wechat/blob/master/wechat.css)可以用来作为其适配。

#### Google Chrome/Chrome OS解决方案

1. 安装以下插件

	- **Minimalist Markdown Editor**：Markdown编辑器，支持预览
	- **StackEdit**: 同样是支持Markdown的编辑器，但有一些方便的编辑工具可使用
	- **Markdown Here**：Markdown渲染，支持自定义样式

2. 基本操作流程

	- 打开*Minimalist Markdown Editor*，开始写作，同时可以在右半窗口即时查看样式渲染效果；
	- 完成写作后，选择全部Markdown源文件（即左半窗口的字符），`CTRL-C`复制；
	- 转到微信公众号写作界面，将上一步复制的内容粘贴`CTRL-V`到文章正文部分；
	- 点击浏览器工具栏里的Makedown Here扩展插件，这时正文部分的Markdown源码将会渲染成指定格式的富文本；
	- 检查渲染之后的文本，如有错误（主要是格式上的不一致），可以修正；
	- 上一步的格式错误的原因往往是微信CSS不兼容造成的，这时候可以去修改Markdown Here的CSS设置文件；
	- 添加文章的其他要素，标题，作者，摘要等，及可预览，发布。

**注意**
1. *StackEdit*支持文档的云端同步，比如可以保存在Google Drive，Dropbox上，非常适合Chrome OS。
2. 一般不用去大改Markdown Here的CSS文件，一旦设置好之后，是一劳永逸的。
3. 在公众号文章编辑后台里面，Markdown Here插件不支持右键菜单，只能点击浏览器工具栏上的相应图标。
4. 关于图片，至少一下几种方案都可以实现图片的一致呈现
	- 首先上传到公众号管理后台的图片素材库，然后复制其链接到Markdown图片插入语句中去，如`![图片说明](图片的链接)`。
	- 图片链接可以是其他地方的图片链接，复制后插入同样有效。
	- 在Chrome浏览器中可以使用相应插件或应用来对图片进行编辑，转换格式，比如*Pixlr Editor*。
5. Markdown的一些基本使用，可以参考这个[Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)。
6. Markdown基本语法：

![mk基本用法](https://mmbiz.qpic.cn/mmbiz_jpg/G50dcd0KcMjuR63khsH1S2nBfflUZicVey8cuIib3SA1rOK8VYbSKQoI1cOmSvGtqIyzicCEjqHv4G9l2hhlUbDkA/0?wx_fmt=jpeg)

#### 其他平台解决方案

使用编辑器，比如Atom，安装Markdown Preview扩展包，就可以开始Markdown写作了，`CTRL-SHIFT-M`即时查看渲染效果，但最终还要以公众号平台支持的风格为准，所以最好使用Markdown Here配合相应的CSS预览一下（有相应的Firefox扩展），最后校对发布。
