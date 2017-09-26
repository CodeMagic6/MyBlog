---
title: node环境搭建
date: 2017-09-27 06:45:43
tags:
---
___

### 前言

对于前端工程师来讲，当我们写项目时，经常需要用到Node，通常我们可以在NodeJs官网下载对应的Node版本，但有时候我们需要在不同的项目切换不同的Node版本，通过官网的安装包已经不能满足我们的需求了，我们需要一个能够方便管理Node的
工具，更好的安装，删除，切换Node版本。nvm就能够满足需求。

### NVM的下载

首先在Github上下载nvm，[](https://github.com/coreybutler/nvm-windows/releases)找到最新的nvm-setup.zip，下载保存

### NVM的安装

1. 将下载的nvm-setup.zip解压，为即将安装的nvm创建一个本地文件夹（这里创建一个名为dev的文件夹）。nvm的安装路径应为C:\dev\nvm
2. 选择node安装路径:默认的node安装路径为C:\Program Files\nodejs，我们更改为C:\dev\nodejs
3. 点击下一步，完成安装

### 设置安装的淘宝镜像目录（可选）

打开nvm目录下的settings.txt文件，在最后追加
    node_mirror: https://npm.taobao.org/mirrors/node/
    npm_mirror: https://npm.taobao.org/mirrors/npm/
![](https://github.com/CodeMagic6/blogImages/raw/master/blogimg/nvm-01.jpeg)

### node的安装

进入nvm目录C:\dev\nvm，按住shift右键点击空白处，点击"在此处打开命令窗口"

#### node安装

    nvm install latest //安装最新版本的node
    nvm install x.x.x  //安装指定版本的node 如nvm install 6.8.0

#### node的使用与版本切换

    nvm use latest  //使用最新版本的node
    nvm use x.x.x   //使用指定版本的node 如nvm install 6.8.0

#### node的卸载

    nvm uninstall latest    //卸载最新版本的node
    nvm uninstall x.x.x     //卸载指定版本的node 如nvm install 6.8.0

### NRM的安装

#### 什么是nrm？

nrm就是npm registry manager 也就是npm的镜像源管理工具，有时候国外资源太慢，那么我们可以用这个来切换镜像源。
    我们只要通过这个命令: npm install -g nrm 就可以实现安装。
