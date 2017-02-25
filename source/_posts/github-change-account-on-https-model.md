---
title: github https模式下切换账号
date: 2017-02-25 13:40:16
categories: 
	Git
tags: [git, https, 切换账号]
---

## 前言

偶然从实践者论坛上看到了如何用Hexo+Next+Github搭建博客的文章，参照文章一路过来也算顺利，因为之前一直用的另一个账号做的Demo，后面遇到用自己账号来正式搭建后部署 hexo d 显示权限有问题，因为之前用https登录过，所以系统默认会以此账号上传。

## 多账号切换问题

因为我有两个github账号，所以在我用A账号登录过后再用B账号来部署就会出现权限问题。百度谷歌了很久看到的都是说通过SSH来实现多账号之间的切换 PUSH。关于Https方式的文章少之又少，而我想采用Https来实现多账号切换，所以始终不得其法。

偶然从一个帖子上看到GIthub官网关于https登录的说明，在这个说明的底部放了一个相关文章的链接，讲得就是https情况下怎么去更新切换账号问题，豁然开朗，原来需要通过MAC下的钥匙串管理工具去删除旧的账号就行了，链接如下：https://help.github.com/articles/updating-credentials-from-the-osx-keychain/ 。