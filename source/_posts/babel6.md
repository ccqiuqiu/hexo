---
title: babel6
date: 2017-01-21 14:20:46
tags: [babel]
categories: node.js
---

在node.js中使用babel6的方法

1. 安装babel6 
> npm install babel-core --save

2. 安装插件
> npm install babel-preset-es2015

3. 配置bedel6
	
	方法1 . 新建 .babelrc 文件
	```js
	{
	"presets": ["es2015"]
	}
	```
	方法2  在pageage.json里面配置
	```js
	"babel": {
      "presets": ["es2015"]
  	}
  	```
  	
4. 新建 index.js
```js
require('babel-core/register')
require('./app.js')
```

5. 运行
> node index.js


### koa2+async 直接使用 runkoa
> npm i -g runkoa
> runkoa app.js

### koa生成器,一键生成koa和koa2项目
[koa-generator](https://github.com/17koa/koa-generator)