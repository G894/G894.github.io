# 笔记

这是一个从[Eddie Webb](https://github.com/eddiewebb/hugo-resume)那拿来的一个主题，我并没有接受过正式的编程教育，这个项目只是为了自己做一个简历。这个笔记也主要是给我自己看不同修改内容在什么位置。

## 1.日常维护

### 添加新的项目经验/往期发表

使用命令：hugo new projects/TYPE/name-of-project.md

TYPE= projects or publication

### 管理项目经验

~\content\projects

### 管理往期发表

~\content\publications

### 修改介绍页个人信息

~\config.toml

### 修改介绍页自我介绍

~\content\_index.md

### 修改工作经验/教育经验/技能

~\data

### 修改照片

替换

~static\img\photo.png

注意，相片长宽比1：1，且仅允许png格式

### 更新在线简历

$ cd public
$ git init
$ git remote add origin https://github.com/G894/g894.github.io.git
$ git add -A
$ git commit -m "更新注释"
$ git push -u origin master

## 2.进阶管理

### 修改项目经验页面的介绍陈述

~\content\projects\_index.md

### 修改往期发表页面的介绍陈述

~\content\publications\_index.md

### 修改导航条内容以及顺序

~\themes\cover\layouts\partials\nav.html

完成该处修改之后需要修改

~\themes\cover\layouts\index.html

以保证右侧板块的顺序与内容与左侧导航条对应

### 修改首页二维码

~\themes\cover\layouts\partials\contact-qr

原本的二维码生成服务需要翻墙，现在修改成本地文件