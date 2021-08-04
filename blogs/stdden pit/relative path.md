---
title: 相对路径
date: 2021-8-3
cover: ../../../cover8.jpg
tags:
 - 坑
 - 相对路径
categories:
 -  那些年犯过的傻事
---
*天知道自己可以这么傻*
<!-- more -->
# 在config里写logo地址

::: tip
我的目录
```
 .vuepress
├── public
|      ├── logo .jpn
├── theme
├── config.js

```
:::

然后我logo的地址是怎么写的  
`"logo": "public/logo.png",`  
通过查找地址属性，我发现logo后面多了一个空格!  
把空格去掉后发现还是不行  
最后去掉public直接./就行了  
`"logo": "./logo.png",` 