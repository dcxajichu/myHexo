---
title: '搬入hexo'
category: 技术
tags: [前端, 博客搭建]
date: 2017-12-13
updated: 2017-12-13
---

由于用 node 比较多，所以想试试基于 node 的 hexo...

<!-- more -->

# 准备

搭建 hexo 前需要先装 node。打开[Node.js 官网](https://nodejs.org/en/)下载 LTS 版本即可。Windows 安装直接双击 msi 文件，一直下一步即可完成安装。

# 安装 hexo

打开命令行，输入`npm install hexo-cli -g`。

# 建立你的博客

打开命令行，输入`hexo init blog`。然后就会在当前目录创建一个名为 blog 的文件夹，这个就是你的博客文件了。

# 运行你的博客

进入你的博客目录，打开命令行，输入`hexo server`。你就可以在`http://127.0.0.1:4000/`访问你的博客了。

# GitHub 部署博客

新建仓库
打开\_config.yml,进行基础配置

```
deploy:
  type: git
  repo: https://github.com/...... 仓库地址
```

安装 hexo-deployer-git 自动部署发布工具

```
npm install hexo-deployer-git  --save
```

发布到 Github

```
hexo clean && hexo g && hexo d
```
