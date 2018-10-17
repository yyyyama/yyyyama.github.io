---
layout: post
title: artTemplate
category: 技术
tags: artTemplate
description: 
---

用ajax获取接口数据,然后用artTemplate把内容渲染出来,
从某种意义上来说实现了前后端,对自己来说也是一种进步.
<br/>
当然在这过程中也遇到了难题,
<br/>

有一些数据并不是从接口获取,而是通过地址传参把数据传过来,并且要在模板中把传过来的参数渲染出来
<br/>
解决方法:
在传数据是可以用对象传递数据

```html
/*模板渲染*/
var data = json_data;
var content = template('playlist',{
    showType: showType,
    matchId: matchId,
    inform:data
});
$('#playlist-tpl').html(content);

```
另一种方法
```html
/*模板渲染*/
    	var data = json_data;
    	var content1 = template('leage',data);
    	$('#leage-tpl').html(content1);
```

另一个问题是,在接口获取的数据是有三位小数点的浮点数,在渲染的时候只显示两位小数点,不改变数据,只需要在显示是显示两位小数点

解决方法

```js
//设置过滤器
template.defaults.imports.fixed = function(value) { return parseFloat(value).toFixed(2); }
//然后在模板中过滤
{{inform.data.r[0].odds_h | fixed}}
```

参考网址:
https://aui.github.io/art-template/zh-cn/docs/
