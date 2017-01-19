---
title: 使用axios读取远程图片保存到本地
date: 2017-01-19 16:15:47
tags: [图片,axios]
categories: node.js
---

使用axios读取远程图片保存到本地

```js
const axios = require('axios');
var fs = require('fs');

 axios.get('https://a-ssl.duitang.com/uploads/item/201506/21/20150621002052_uMTRQ.jpeg', {
  responseType: 'arraybuffer'
 })
  .then(function(response) {
      console.log(response.status);
      console.log(response.headers);
  	fs.writeFile('out.jpeg', response.data, function (err) {
    	if (err) throw err;
    	console.log('保存成功');
 	});
 }); 
```