---
layout: post
title: github在线编辑器
category: 工具
tags: github
description: github在线编辑的一些用法
---

## 添加图片

添加github仓库代码里面的图片<br>
![](https://yyyyama.github.io/assets/img/avatar.jpg)<br>

添加来源于网络上面的图片
![](http://www.baidu.com/img/bdlogo.gif)<br>

在方括号内可以加入一些标志性的信息<br>
比如<br>
![baidu](http://www.baidu.com/img/bdlogo.gif)
还可以
![baidu](http://www.baidu.com/img/bdlogo.gif “百度LOGO”)

这个时候鼠标放到图片上面会有 “百度LOGO”这4个字。<br>

给图片加上超链接<br>

[![baidu]](http://baidu.com)[baidu]:http://www.baidu.com/img/bdlogo.gif "百度Logo"


## 插入标题
#一级标题  
##二级标题  
###三级标题  
####四级标题  
#####五级标题  
######六级标题  

## 换行
<br>

## 文字超链接
[我的博客](https://yyyyama.github.io)


## 插入代码片段
我们需要在代码的上一行和下一行用``` 标记。<br>
``` 不是三个单引号，而是数字1左边，Tab键上面的键。<br>
要实现语法高亮那么只要在 ``` 之后加上你的编程语言即可（忽略大小写）。<br>
c++语言可以写成c++也可以是cpp。看代码：<br>

```css
.box {
  display: flex;
}
```
