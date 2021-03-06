---
layout: post
title: "Mock"
description: "模拟请求 &amp; 模拟数据"
category-substitution: 工具
tags: [工具, Mock, JavaScript, Web]
published: false
---
{% include JB/setup %}

草稿！！！

# 目录

* 困境
* 方案
* 应用场景


# Mock - 模拟请求 & 模拟数据

在传统的前端-后端协作方式中，前端的开发进度往往会依赖于后端。在后端开发完成之前，前端只能设计和实现一些基础架构；而一旦后端完工，交付的压力就落在了前端头上，而此时后端却无所事事。如果后端延期，那么前端可能被迫压缩工期，JUST SAY NO？如果后端的接口不稳定，或者接口发生了变化，你需要修改本来可以运行的代码并重新测试。显然资源被浪费了。

> 不要误解我的意思，延期和变化常见的很，我吐槽的不是后端 or 前端，仅仅是瀑布式的前端-后端协作方式。

而另一方面，在过去的几年里，我们看到这样一个趋势：越来越多的 Web 开发工作在前端完成。有没有什么方式，可以让前端-后端同步开发、缩短项目周期呢，并减少冲突、愉悦开发呢？

我的答案是：
1. 在前端和后端之间加入一层“模拟层”，模拟后端服务，让前端-后端可以同步开发。
2. 把后端接口（通常会在设计阶段文档化）纳入版本管理，跟踪和记录变更内容，
3. 代码和业务越来越复杂，前端是时候引入测试用例啦。

在需求、设计、交互、后端、前端的分工中，前端作为交付的最后一个环节，deadline 就像一把达摩克利斯之剑，始终高悬在前端工程师的头顶。
    选择太多
    兼容太多

依赖后端的进度：Mock
后端接口不稳定或更新：API 设计、版本管理
测试代码
每个步骤都是关键步骤：
    前端-后端：RESTful 架构 
    后端：模拟
    前端：测试驱动
    测试：提前介入

## 2013.07.18
Mock for 测试、开发、演示？以 Treemap、Grid 为例？更多。。。

### 目的
解决数据部分，
展现 HTML、样式 CSS、行为 JavaScript、数据 Mock，参考 Chance 的定位）

### 定位
测试 & 演示，前端-开发，组件开发-组件用户，组件开发者-测试用例
Brix：数据 + 模板 + 行为（参考 Brix 的宣传文档）

### 特点
1. 开发无侵入，可以通过参数动态地控制
2. 灵活方便，数据+元数据
3. 简洁的多功能接口，Mock
4. 扩展方便：mockajax、placeholder
5. 引用方便，支持直接应用、通过 KISSY 或 SeaJS 加载，node 加载
6. 丰富的数据类型

### 适用场景
1. 方便测试，覆盖面
  Dropdown、Grid、Treemap、Pagination
2. 开发阶段的前期
3. 接口设计，直观、快速、简洁、验证，以结构为主，快速理解
4. DEMO 演示，如果数据部分过程，会看起来很不爽，还会影响代码结构，造成困惑，影响主体
5. 构造复杂数据
6. 构造大型数据
7. 以钻展为负面例子，以 DMP 为正面例子，特别是子标签、饼图、丰富折线图？

## 开发过程

TDD


## 参考资料
* [RANDOM.ORG - String Generator](http://www.random.org/strings/)
* [Behind the Name: Random Name Generator](http://www.behindthename.com/random/)
* [The Random Image Generator | RandomImageGenerator.com - rndimg.com](http://rndimg.com/default.aspx)
* [Random Word Generator With Definitions - Randomly Generate Thousands of Words](http://www.wordgenerator.net/random-word-generator.php)


