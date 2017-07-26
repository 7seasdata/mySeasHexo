---
title: GTM系列教程之 GTM部署以及GA结合埋码
tags: [Google Tag Manager]
categories: [GTM系列]
date: 2017-7-26
grammar_cjkRuby: true
---

# GTM系列教程之 GTM部署和GA埋码

### 背景：
随着现在很多业务的国际化，相信大家都会需要一个统计平台来对自己的业务进行数据的监控以及分析，在国际业务中，Google Analytics (GA) 基本是大家的主要选择，那么今天我们就一起来学习GTM的基础部署 以及 结合GA进行埋码吧

### GTM认识与部署
GTM 全称是 Google Tag Manager， 它是Google 在2012年发布的一个重要产品； GTM 主要是一个管理工具，能进行代码，标签，js脚本的管理，因此我们可以通过GTM 进行站点的跟踪的代码部署，APP跟踪的代码部署，以及再营销代码，和DCM代码等等

GTM的特性可以理解为一下节点：
* 免费的
* 可以直接使用
* 忘记限制
* 无缝与GA结合
* 跟踪方便
* 安全的
* 可以进行debug调试

### 开始部署GTM

 1.创建GTM账号，可以是公司名字，站点名字等，
 ![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/gtm-bushu-st1.png "创建账号")

 2.点击继续，进行设置容器
  ![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/gtm-bushu-st2.png "设置容器")

3.同意条款协议
  ![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/gtm-bushu-st3.png "同意条款协议")

4.产出部署代码
  ![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/gtm-bushu-st4.png "同意条款协议")

5.然后把需要部署跟踪的代码部署到页面对应位置上，检查网站是否正常加载到gtm.js 文件
  ![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/step5.png "检查gtm.js")

### 创建GA埋码

1.创建GA账号
 ![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-step1.png "创建账号")

2.填写网站基本信息
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-step2.png "填写网站基本信息")

3.获取网站埋码
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-step3.png "获取网站埋码")

### 通过GTM进行GA埋码关联注入

1.创建代码模块
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step1.png "创建代码")

2.选择自定义HTML，填写GA埋码脚本
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step2.png "填写埋码脚本")

3.选择触发条件为All page
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step3.png "选择触发条件")

4.提交改动信息，并且点击发布
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step4.png "提交更改")

![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step5.png "提交更改")

5.发布成功后查看网站请求  是否已经存在collect 请求
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step6.png "检查请求")

6.访问GA便可看到数据已经在统计
![alt text](http://otoxrqu0z.bkt.clouddn.com/site/img/ga-relate-step7.png "访问GA")

### 总结

通过以上的操作示例，我们完成了通过GTM 部署 GA代码的步骤， 通过GTM 我们可以在不用重新发布代码的状态下进行代码的部署与发布，大大地提高了效率