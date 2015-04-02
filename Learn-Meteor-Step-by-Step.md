# Learn Meteor Step by Step 
* 毛豆网《Meteor精益创业孵化营》内部培训教材大纲，报名请联系微信号 limingth

## 1 预备知识
* Install Tools
  - Meteor
  - Chrome
  - Robomongo
  - Sublime Text/WebStorm
  - Git and Github
* Commands
  - meteor create/run/add/mongo/deploy/log
  - git init/add/commit/push/pull/log
* Basics
  - HTML5
  - CSS/LESS
  - JavaScript/CoffeeScript

```
* 项目代码分析： hello
```

## 2 Meteor基础
* Meteor 7 Principles
  - Data on the Wire
  - Latency Compensation
  - Full Stack Reactivity
* Basic Concept
  - Template/Event/Helper
  - Session/Reactive
  - Blaze/Handlebar
* Meteor Deploy
  - meteor deploy/settings
  - meteor up/mup/mup.json
  - how to deploy to aliyun/amazon EC2
* Meteor app structure
  - client/server/lib/public/packages/tests
  - publications/subscriptions/methods/collections/routes/seeds

```
项目代码分析： todos
```

## 3 Mongo基础
* NoSQL vs SQL
* Collections
  - Schema
* Database Operations
  - Insert/Remove/Update/Find
* Shell Methods
  - find()/findOne()/insert()/remove()/update()
* Robomongo
  - Documents/Edit/View/Insert/Delete/Copy

```
项目代码分析： hero
```

## 4 Meteor进阶
* Publish and Subscription
  - Minimongo
  - DDP
  - cursor/record set
  - Multiple Subscriptions 
  - Publish with userFields
* Allow and Deny
  - insert/update/remove

```
项目代码分析： meteorhunt
```

## 5 常用package
* Iron router
  - Router.map()
  - this.render()
* ionic framework/UI 
  - meteoric:ionic
  - meteoric:autoform-ionic
* simple-schema
  - aldeed:autoform
* underscore
  - each/map/reduce/find/filter/where
* some other packages 
  - reywood:publish-composite
  - anti:fake
  - momentjs:moment
  - bengott:avatar

```
项目代码分析： welog
```

## 6 User用户登录
* Packages inside
  - accounts-password
  - accounts-ui
* Other Login Packages
  - weibo/qq
  - linkedin/github
* Meteor.users
  - onCreateUser()
  - ServiceConfiguration

```
项目代码分析： meteor-bbs
```

## 7 项目1 Meteor微信app应用开发
* 微信app
  - 微信公众号
  - 微信SDK
* 典型项目应用分析-活动行
  - 微信用户信息获取
  - 表单设计
* 典型行业应用分析-滴滴打车（可选）
  - 地图API
  - 获取地理位置API
  - O2O代码设计框架 

## 8 项目2 基于Meteor的iOS/Android app应用开发
* 典型购物商城项目案例
  - Code Analysis 代码分析
  - Data Design 数据设计
  - Work Flow 运转流程
  - Template Appliance 模版应用


