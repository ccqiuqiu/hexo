---
title: markdown语法
date: 2017-01-06 16:51:21
tags: [md,markdown]
categories: 杂项
---
既然以后要使用md来写笔记，首先当然要记下常用的md语法。
### 强调
星号与下划线都可以，单是斜体，双是粗体，符号可跨行，符号可加空格

<!-- more -->

> **加粗**
>__加粗__
>*斜体
>符号可以换行*
>_斜体_

### 分割线
三个或更多-，必须单独一行，可含空格
> a 
>--- 
> b

### 标题
三个或更多 ===  ---  或者#  1-6个
> 大标题
> ===
> 小标题
> ---
> # 1级标题
> ## 2级标题
> ### 3级标题
> #### 4级标题
> ##### 5级标题
> ###### 6级标题

### 无序列表
-+*
> - 无序列表
> + 无序列表
> * 无序列表

### 有序列表
数字不能省略但可无序，点号之后的空格不能少
> 1. 有序列表
> 2. 有无序列表
> 3. 有序列表

### 嵌套列表
-+*可循环使用，但符号之后的空格不能少，符号之前的空格也不能少
> - 嵌套列表
> + 嵌套列表
> + 嵌套列表
>   - 嵌套列表
>     * 嵌套列表
>- 嵌套列表

### 文字超链接
> [cc](http://ccqiuqiu.github.io "cc的博客")

### 图片
![alt] (url "title") 去掉括号前的空格
> ![GitHub Mark](http://github.global.ssl.fastly.net/images/modules/logos_page/GitHub-Mark.png "GitHub Mark")
> ![alt](1.png "title")

### 自动链接
直接加尖括号
> <http://ccqiuqiu.win>

### 代码块
```js
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) +
             ` class="${cls}"`;
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }
}

export  $initHighlight;
```
