---
layout: post
title: "GitHub 博客绑定自定义域名指北"
date: 2026-07-16 12:00:00 +0800
description: "记录将 GitHub 静态博客绑定到独立域名的完整流程与 DNS 配置"
tags:
  - 博客搭建
  - GitHub Pages
  - 域名
---
> “If you care about me at all, please don’t say anything to anyone. ”

### ▎正文

前几天在活动中申请了几个免费的域名，便想着给自己的静态博客挂一个域名。这里简单的记录一下将github博客绑定到自己域名的过程。

##### 步骤一

在github博客仓库下创建一个名为CNAME的文件，并在其中填入要绑定的域名地址，如 `sliverkiss.free.hr` 。

##### 步骤二

进入github博客仓库，点击 `settings`,查看 `Custom domian` 是否已经填写并保存。通常完成步骤一后会自动保存。

##### 步骤三

域名解析，由于我的域名是通过 `cloudflare` 解析的，所以需要登录cloudflare，点击网站选项，选择想要绑定的域名。在DNS解析选项中添加相应的记录

```plaintext
类型    名称           目标
CNAME   www  sliverkiss.github.io
CNAME    @   sliverkiss.github.io
```

配置完成后，等待1～2min直到DNS解析完毕，便可以通过域名 `sliverkiss.free.hr` 访问原来的博客 `sliverkiss.github.io` 了