---
layout: post
title: GitHub 搭建个人主页（基础版）
description: windows 下，如何搭建最简版的个人 blog？有哪些注意事项？
category: github
---

## 0. 背景

现在准备在 windows 环境下，搭建一个最简版的 `GitHub` 个人博客主页。

几个焦点：

1. 如何搭建，个人博客？
2. 如何编写，个人博客？

## 1. 如何搭建，个人博客？

在 GitHub 下，如何搭建个人博客呢？从官网中，查看到搭建的指南：

* [GitHub Pages]： Websites for you and your projects.

其中，详细介绍了 2 个部分：

1. GitHub Pages 是什么
2. GitHub Pages 如何搭建和使用，涵盖 5 个基本步骤

按照上述[官网指导][GitHub Pages]，搭建一份个人主页。

搭建完之后，个人主页只是一个非常朴素的页面，一般建议启用 `Jekyll` 主题，具体办法：

1. 前往个人 github pages 对应 github 仓库（一般为 `username.github.io`）， `settings` 页面
2. 在 `GitHub Pages` 配置部分，`Theme Chooser` 项中，选定一个 `Jekyll` 主题即可.

> **Note**: GitHub Pages 上，官方推荐的 Jekyll 主题，样式比较简陋，因此，推荐使用现有的 Jekyll 主题。

以使用 `ningg.github.io` 的个人博客 jekyll 主题为例，具体步骤：

1. 下载代码：下载 `ningg.github.io` 的网站代码，即可作为自己的 jekyll 主题
2. 删除配置：刚下载的 jekyll 主题中，删除个人配置，例如：blog 内容、评论、微博插件、google 统计。
3. 提交代码：将调整后的内容，提交到自己的 github 个人仓库中。

具体操作细节：

```
# 1. 下载代码：即可获取完整的网站代码
git clone https://github.com/ningg/ningg.github.com.git 

# 2. 删除配置 TODO
TODO

# 3. 提交代码
TODO：将上述删除后的文件，提交到自己的个人仓库
```

## 2. 如何编写，个人博客？

分为 4 个部分：

1. 安装软件： git 
2. 下载博客仓库的代码
3. 编写个人博客
4. 提交代码


### 2.1. 安装软件

为了能够下载`博客仓库代码`，需要提前安装 git 软件：

* [Set up git](https://help.github.com/en/articles/set-up-git)

具体，Windows 环境下，下载下述 git 安装软件即可：

* [git Downloads](https://git-scm.com/downloads)


### 2.2. 下载博客仓库的代码

安装了 git 软件后，打开 `命令行终端`，并执行下述命令，下载博客仓库的代码：

```
# 下载仓库代码
git clone https://github.com/DXXXX/DXXXX.github.io.git
```


### 2.3. 编写个人博客

在 `_posts\blog` 目录下，参照 `template.md` 模板，创建一个 `md` 文件，其中，编写自己的博客内容即可。

其中，`md`文件，使用 markdown 语法，细节参考 

* [markdown入门介绍](http://ningg.top/introduction-to-markdown/)


### 2.4. 提交代码

编写完个人博客后，通过下述命令，提交博客到 github 仓库即可完成博客内容发布：

```
# 1. 将修改/新增内容，标记提交
git add .

# 2. 编写提交的备注信息
git commit -m "这次增加了一篇博客"

# 3. 内容，推送到远端服务器
git push origin master

# 4. 上述都结束后，大约 2~3 mins，就完成了 blog 内容的公开发布
```


## 附录

### 附录 A：部分内容，修改

关于采用的 `ningg.github.io` 的 jekyll 主题，如何修改 About 页面内容呢？

* 在 `about` 目录下， 修改 `index.md` 页面即可。






















[NingG]:    http://ningg.github.com		"NingG"

[GitHub Pages]:		https://pages.github.com/
