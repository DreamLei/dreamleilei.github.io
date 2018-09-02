---
title: redis知识总结
date: 2018-09-01 11:51:50
tags:
    - redis
    - 阅读
categories:
    - redis
---

 最近在阅读《redis设计与实践》这本书，阅读这本书，了解了很多redis的内部实现，从开始会用，慢慢的向开始了解原理进军，
 在此记录一下，方便后续记录和复习。
        
## redis数据类型
redis的数据类型如下，目前有且只有以下五中数据类型:
- **String**
- **list**
- **hash**
- **set**
- **zset**

### String 
String 类型应该是redis五种数据类型中用到的最频繁的类型了，