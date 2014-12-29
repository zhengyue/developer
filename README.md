开发人员需要具备的基本知识

目录
=====

  * [所有开发者都需要掌握的基础知识](#%E6%89%80%E6%9C%89%E5%BC%80%E5%8F%91%E8%80%85%E9%83%BD%E9%9C%80%E8%A6%81%E6%8E%8C%E6%8F%A1%E7%9A%84%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86)
    * [网络](#%E7%BD%91%E7%BB%9C)
    * [数据与编码](#%E6%95%B0%E6%8D%AE%E4%B8%8E%E7%BC%96%E7%A0%81)
    * [Web](#web)
    * [安全](#%E5%AE%89%E5%85%A8)
    * [编码哲学与业务实践](#%E7%BC%96%E7%A0%81%E5%93%B2%E5%AD%A6%E4%B8%8E%E4%B8%9A%E5%8A%A1%E5%AE%9E%E8%B7%B5)
    * [版本控制](#%E7%89%88%E6%9C%AC%E6%8E%A7%E5%88%B6)
  * [Web前端开发者需要掌握的知识](#web%E5%89%8D%E7%AB%AF%E5%BC%80%E5%8F%91%E8%80%85%E9%9C%80%E8%A6%81%E6%8E%8C%E6%8F%A1%E7%9A%84%E7%9F%A5%E8%AF%86)
    * [JavaScript](#javascript)
    * [CSS](#css)
    * [HTML](#html)
    * [框架](#%E6%A1%86%E6%9E%B6)
  * [iOS开发者需要掌握的知识](#ios%E5%BC%80%E5%8F%91%E8%80%85%E9%9C%80%E8%A6%81%E6%8E%8C%E6%8F%A1%E7%9A%84%E7%9F%A5%E8%AF%86)
    * [Objective-C](#objective-c)
    * [Cocoa-Touch框架](#cocoa-touch%E6%A1%86%E6%9E%B6)
    * [Xcode](#xcode)
    * [Swift](#swift)
    * [应用提交](#%E5%BA%94%E7%94%A8%E6%8F%90%E4%BA%A4)
    * [第三方库](#%E7%AC%AC%E4%B8%89%E6%96%B9%E5%BA%93)
  * [Android开发者需要掌握的知识](#android%E5%BC%80%E5%8F%91%E8%80%85%E9%9C%80%E8%A6%81%E6%8E%8C%E6%8F%A1%E7%9A%84%E7%9F%A5%E8%AF%86)
    * [SDK](#sdk)
    * [模拟器](#%E6%A8%A1%E6%8B%9F%E5%99%A8)
    * [开发工具](#%E5%BC%80%E5%8F%91%E5%B7%A5%E5%85%B7)
  * [后端开发者需要掌握的知识](#%E5%90%8E%E7%AB%AF%E5%BC%80%E5%8F%91%E8%80%85%E9%9C%80%E8%A6%81%E6%8E%8C%E6%8F%A1%E7%9A%84%E7%9F%A5%E8%AF%86)
    * [操作系统](#%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F)
    * [语言](#%E8%AF%AD%E8%A8%80)
    * [框架](#%E6%A1%86%E6%9E%B6-1)
    * [数据库](#%E6%95%B0%E6%8D%AE%E5%BA%93)

# 所有开发者都需要掌握的基础知识

## 网络

* TCP/IP基础
    * 了解IP、TCP、UDP、DNS这些协议的用途和原理
    * 了解IP地址、子网掩码、端口号
    * 域名的用途
* URL的构造：能正确地识别一个完整URL中的各个部分
    * 协议: http, https, mailto, tel...
    * 主机名
    * 域名
    * 端口号: 80, 443...
    * 路径
    * 查询参数
    * 绝对地址与相对地址
    * URL中只能使用部分英文字母和符号，其他字符需要使用%编码
* 了解HTTP协议
    * 基于文本的协议
    * 请求/响应的方式，无状态
    * GET/POST/PUT/DELETE方法
    * 要知道报头里面常用的字段的含义
        * User-Agent
        * Content-Type
        * Content-Length
    * 知道返回码的含义
    * 可以从命令行发送一个正确的HTTP请求给服务器
    * 会使用抓包工具分析HTTP请求和响应（Fiddler等） 

## 数据与编码

* JSON基础知识
* XML的基础知识
* 字符编码常识
    * ASCII编码
    * UTF-8编码
    * GB2312/GBK编码
    * Unicode 16/32编码
    * 能分析乱码的产生原因
        * 操作系统的默认编码、数据库的编码、编程语言中字符串的编码、HTTP的编码、客户端的编码等等
* Base64编码的用途
* MD5, SHA1等hash算法的用途

## Web

* HTML基本语法
* DOM的基本概念
* CSS的基本语法和概念
    * 盒子模型
    * 行级元素与块级元素
* JavaScript
    * JS核心语法与DOM操作
    * 如何进行函数回调
    * 如何操作DOM，jQuery的基本用法

## 安全

* SQL注入的原理与预防
* 对称加密与非对称加密算法的基本概念
* 浏览器的跨域访问限制

## 编码哲学与业务实践
* KISS - Keep it simple stupid。
    * 在简单但是性能稍差的方案与复杂但性能稍优的方案中，选择简单、容易理解的那个
    * 容易维护大于性能优化
* DRY - Don't repeat yourself
    * 禁止复制/粘贴编程法
    * 在发现自己需要复制代码的时候就要考虑重构了
    * 重构的首要目标是让代码便于理解和维护
* 不要在代码里埋地雷
    * 避免Magic Number，使用常量定义或者变量
    * 同一个变量不要有多种用途
* 防御性编码
    * 一个正常的软件花在处理边界条件和错误处理上的代码量可能比业务逻辑还要多
    * 截获该处理的异常，放过不该处理的异常，不要存在“异常黑洞”
* 过早优化是万恶之源
    * 找到正确的解决方案往往比优化更能有效提高性能
    * 先正确地解决问题，然后再去考虑如何优化
    * 在没有弄清楚需求将来的变化走向之前，不要过早考虑优化方案
    * 实现需求之后，用性能测试工具找出瓶颈，再有针对性地做优化
* 知道如何利用日志输出方便调试和查错
* 涉及到金额的地方不要使用浮点类型，而是用BigDecimal。如果精度允许，也使用以分为单位的整数

## 版本控制

* 基本概念：代码库、版本、历史、提交、更新、查看历史、分支、合并，中央与分布式版本控制
* 提交的原则：不提交垃圾文件，如何写好提交记录，多提交
* git基本操作：多使用分支，理解rebase
* svn基本操作：遵循 trunk/branches/tags 标准结构

# Web前端开发者需要掌握的知识

## JavaScript
* 如何扩展一个对象
* 理解和应用闭包
* 知道 Grunt / Gulp/ npm / Bower 这些工具的用途

## CSS
* CSS预处理器，了解Sass Compass, Less

## HTML
* HTML5

## 框架
* Bootstrap
* AngularJS
* 

# iOS开发者需要掌握的知识

## Objective-C
* 内存管理基本概念：autorelease的原理，对象生命周期
* 属性的内部实现方式
* KVO，KVC的用法
* Category的用法
* 解耦的方式：Delegate、Notification
* Objc Runtime

## Cocoa-Touch框架
* 应用生命周期
* View和Window：层级结构、坐标系、点与物理像素
* 屏幕适配：Autolayout，Size Class
* 事件响应流程
* 应用后台运行的规则
* 最佳实践
    * 如何根据不同OS版本执行不同代码：不要直接检测系统版本

## Xcode
* 代码静态分析
* Interface Builder, Storyboard
* 调试工具
* 性能检测工具

## Swift

## 应用提交
* 证书管理
* 代码签名

## 第三方库

# Android开发者需要掌握的知识

## SDK

## 模拟器
* adb的使用
* Genymotion

## 开发工具
* Android Studio，Gradle，代码混淆工具

# 后端开发者需要掌握的知识

## 操作系统

* Linux 操作系统基础操作

## 语言

* Java 语言基础: JDK 1.6, Java 7
* JVM常用配置参数
* Maven，Ant，Gradle

## 框架
* Web应用的标准结构
* Java Servlet 容器 或 Java Application Server 基础知识: Glassfish3,Jetty8
* Spring 应用框架基础

## 数据库

* SQL语言
* 关系型数据操作基础, PostgreSQL 数据库基础知识
* 数据库常用优化策略
* 非关系型数据库和缓存服务基础知识: Redis,Memcached
