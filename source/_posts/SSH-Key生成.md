---
title: SSH Key生成
date: 2017-09-22 22:34:01
tags:
---

当我们使用Github和Gitlab参与项目时，需要验证我们自己的身份。一种可能的解决方法是每次访问的时候都带上用户名和密码，另外一种是在本地保存一个唯一的Key，在你的账户中也保存唯一的一个Key，在你访问时带上Key即可
Gitlab和Github就是采用Key来验证你的身份的，并且利用RSA算法来生成这个密钥。

### 方法
1，首先你需要在github上或者gitlab上有一个自己的账户
2，打开git bash，输入命令ls -al ~/.ssh.检查是否显示有id_rsa.pub或者id_dsa.pub存在，如果存在请直接跳至第4步。
3，在git bash中键入ssh-keygen -t rsa -C "your_email@example.com"，注意将这里的邮箱地址替换成你自己的邮箱地址，一直按回车
4，用记事本之类的打开id_rsa.pub文件，并且复制全部内容
5，在你的gitlab或者github账户，打开SSH Key标签
然后选择Add SSH key按钮，将刚刚复制的内容粘贴进去即可，然后点击add key.
