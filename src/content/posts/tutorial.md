---
title: 博客基本教程
meta_title: ""
description: 博客仓库的拉取，nodejs环境的搭建，博客的本地运行与部署
date: 2025-12-30
image: 
categories: ["关于本博客"]
authors: ["biscuit"]
tags: ["基本教程"]
draft: false
---

推荐使用markdown语法喵，[文章标题头的注意事项参考](https://class0x0e.github.io/elements/)

### 推荐编辑器

#### vscode

[vscode](https://code.visualstudio.com/)

理由：

1. 免费开源

2. 插件丰富，支持markdown预览，git图形化，代码补全等功能

#### typora

[typora](https://typora.io/)

理由：

我不知道，没用过，这一块让老六补充

### 博客仓库的拉取

#### github上创建账号

参考官网文档：[github注册](https://git-scm.com/book/zh/v2/GitHub-%E8%B4%A6%E6%88%B7%E7%9A%84%E5%88%9B%E5%BB%BA%E5%92%8C%E9%85%8D%E7%BD%AE)

不要选任何付费套餐，免费版完全够用。

#### git安装

<Tabs client:load>
<Tab name="Windows">

##### windows下git安装

从官网安装：[git for windows](https://git-scm.com/download)

建议安装最新稳定版，找关键词`the latest (x.xx.x) x64 version of Git for Windows`这样的。

在安装流程里面参考[这一篇](https://www.cnblogs.com/xueweisuoyong/p/11914045.html)

安装完了之后打开cmd，输入

```bash
git --version
```

如果显示版本号说明安装成功
</Tab>
<Tab name="Linux">

##### linux下git安装

大部分linux发行版都自带git，如果没有可以通过包管理器安装。

对于Debian/Ubuntu系：

```bash
sudo apt update
sudo apt install git
```

对于Arch系：

```bash
sudo pacman -S git
```

对于Fedora系：

```bash
sudo dnf install git
```

安装完了之后打开终端，输入

```bash
git --version
```

如果显示版本号说明安装成功
</Tab>
<Tab name="macOS">

##### macOS下git安装

鼠鼠没有用过mac，希望懂哥补充
</Tab>

</Tabs>

#### git信息配置

先配置用户名和邮箱：用户名是你的github用户名（主页左上角的那个），邮箱是你注册github时使用的邮箱

```bash
git config --global user.name "你的github用户名"
git config --global user.email "你注册github时使用的邮箱"
```

再配置ssh，这一步可以跳过，老六实验过能直接clone，如果不行再来配置

#### 博客仓库的克隆

在你想存放博客仓库的目录下打开终端，输入

```bashbash
git clone https://github.com/class0x0E/class0x0e.github.io.git
```

这样就把博客仓库克隆到本地了

### nodejs环境的搭建

博客是基于[Astro](https://astro.build/)框架搭建的，需要nodejs环境（很神奇的是astro只支持nodejs的偶数版本）。

其实单纯写博客不需要安装nodejs环境，但是如果想在本地运行博客预览和调试就需要。如果电脑空间不够，或者装不明白可以跳过这一步。

先检查

<Tabs client:load>
<Tab name="Windows">

##### windows下nodejs安装

//todo

</Tab>

<Tab name="Linux">

