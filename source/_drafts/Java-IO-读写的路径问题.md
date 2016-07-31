---
title: Java IO 读写的路径问题
id: 265
categories:
  - 未分类
tags:
---

最近在写项目的过程中一直遇到因为项目中路径不清楚的问题而导致异常的抛出，再此整理一下笔记，记录下自己踩的坑。

首先介绍几个常用的API

[Java]

XXX.class.getClassLoader().getResource(“”).getPath();

XXX.class.getResource(“”).getPaht();

System.getProperty(“user.dir&quot;);

new File(&quot;&quot;).getAbsolutePaht();

new File(&quot;&quot;).getCanonicalPath();

XXX.class.getClassLoader().getResource(&quot;&quot;).getPath(); 获取classPath的加载路径

XXX.class.getResource(&quot;&quot;).getPath(); 获取当前类的加载路径;

[/Java]

测试截图如下:![](http://www.dreamleilei.com/wordpress/wp-content/uploads/2016/06/2016-06-19-13-36-02-的屏幕截图.jpg "2016-06-19 13-36-02 的屏幕截图.png")