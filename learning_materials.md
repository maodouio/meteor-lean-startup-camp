# Meteor 项目孵化营学习资料

## 科学上网
* google 搜索镜像
  - [谷歌(加速)](http://ggss.so/) 可以在 chrome-》设置-》搜索 中将谷歌(加速)设置为默认搜索引擎
  - [glgoo](http://www.glgoo.com/)
  - http://www.itechzero.com/google-mirror-sites-collect.html
* chrome免费翻墙插件
  - [穿越-免费版](http://www.game4fun.cn/ec/index.html)
  - [frigate](http://chromecj.com/productivity/2014-12/323/download.html)

## 科普 & 基础知识
* Meteor是什么 & 优缺点
  * [2015.03.08 毛豆网Meteor开发者交流日 Kevin 演讲视频](http://www.youku.com/playlist_show/id_23545469.html) 
  * [Meteor适合精益创业](http://www.manuel-schoebel.com/blog/meteorjs-the-perfect-match-for-lean-startups)
  * [Meteor适合初学者](http://learn.meteorfactory.io/9-reasons-meteor-is-a-great-choice-for-beginners/)
* 哪些公司在用 meteor？
  * [Quora：哪些startups 使用了 Meteor?](http://www.quora.com/Which-startups-use-Meteor-in-production)
  * [Quora：哪些 web applications 使用了 Meteor?](http://www.quora.com/What-are-some-web-applications-built-with-Meteor-js)
  * [Made with Meteor](http://madewith.meteor.com/)
* Meteor基础视频课程
  * [麦子学院Kevin视频教程：node.js上最新HTML5开发框架-Meteor](http://www.maiziedu.com/lesson/3446/)

## 电子书 & 任务 demo
* leaderboard: meteor create --example leaderboard
* [免费初学者电子书：Your First Meteor Application](http://meteortips.com/)
* [discover meteor](http://zh.discovermeteor.com/): 建议先看完Your First Meteor Application，再看这本书

## 开发环境
* 安装：
  * windows：下载 https://install.meteor.com/windows
  * OSX：命令行`curl https://install.meteor.com/ | sh`
* 工具：
  * 代码编辑器：sublime，atom，webstrom
  * 版本控制：git
    - [常用命令](https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf)
  * 代码托管：github
    - [github for mac](https://mac.github.com/)
  * 命令行 安装 oh-my-zsh http://haoduoshipin.com/episodes/103
  * 调试：chrome 开发者工具

## 前端框架 & 图标
* [meteoric](http://meteoric.github.io/): 如果你想做 mobile app，就使用它吧。ionic 的详细文档在[这里](http://ionicframework.com/docs/components/)，自定义样式参考[Writing a Sass Theme](http://learn.ionicframework.com/formulas/working-with-sass/
)
* ionic图标：http://ionicons.com/
* font awesome 图标：https://atmospherejs.com/fortawesome/fontawesome
* [bootstrap](http://getbootstrap.com/): general framework for pc & tablet & mobile, not specially for mobile use
* [foundation](http://foundation.zurb.com/): mobile first front-end framework
* [AdminLTE - Free Premium Admin control Panel Theme That Is Based On Bootstrap 3.x](https://almsaeedstudio.com/preview)

## 知识库
* meteor 官方文档：https://docs.meteor.com/
* [meteor 常用学习网站](https://github.com/maodouio/meteor-lean-startup-camp/wiki/meteor%E5%B8%B8%E7%94%A8%E5%AD%A6%E4%B9%A0%E7%BD%91%E7%AB%99)
* [meteor 数据详解](https://medium.com/@stubailo/data-flow-from-the-database-to-the-ui-three-layers-of-meteor-d5e208b466c3)
* [Meteor DDP翻译](https://cnodejs.org/topic/51b030d9555d34c678e5fb2e)
* [mongoDB 基础](https://github.com/maodouio/meteor-lean-startup-camp/blob/master/mongoDB_basics.pdf)
* [常用 sublime 插件](https://github.com/maodouio/meteor-lean-startup-camp/wiki/sublime-%E7%9A%84-meteor-%E6%8F%92%E4%BB%B6)
* [常用 atom 插件](https://atom.io/packages/meteor-api)
* 常用 package 搜索：[atmosphere](https://atmospherejs.com/)
* [Cordova:调用手机 media 功能的 API](https://gist.github.com/luckyyang/00286f1a505933d95b84)
* [robomongo怎么看看服务器的数据](https://gist.github.com/luckyyang/c30638ee236d62b3b8e5)
* 左侧菜单模版: [Demo](http://maodou-ionic-example.meteor.com) [Code](https://github.com/netanelgilad/meteor-ionic-example)
* 用户
  - 用户注册登录的i18n(中文化)
    - [文字版](https://github.com/maodouio/meteor-lean-startup-camp/wiki/i18n-for-meteor-useraccounts) 
    - [视频](http://meteorcasts.meteor.com/)
  - [注册时添加自定义字段](https://github.com/meteor-useraccounts/core/blob/master/Guide.md#form-fields-configuration)
 
* IOS & Android
  - 消息推送：
    - https://atmospherejs.com/raix/push
    - https://github.com/richsilv/meteor-cordova-notifications

* IOS相关知识
  - [IOS app如何打包和发布](https://github.com/meteor/meteor/wiki/How-to-submit-your-Android-app-to-Play-Store)

* Android相关知识
 - [Android  app如何打包和发布](https://github.com/meteor/meteor/wiki/How-to-submit-your-Android-app-to-Play-Store)
 - [android 键盘输入时input框空白问题](https://github.com/maodouio/meteor-lean-startup-camp/wiki/meteoric-Android-keyboard-issue)

 
## 常用 package
* 如何使用 package？
  * 命令行meteor add package_name
  * 使用方法看 package 文档
* 图片裁剪：https://atmospherejs.com/jonblum/jquery-cropper
* 用户登录注册：https://atmospherejs.com/meteor/accounts-password
* 登录注册 UI：https://atmospherejs.com/meteor/accounts-ui

## 开发流程
* 修改代码
* git commit
* git push
* 测试
* 部署，done
 
## 部署
* vps 选择
  * amazon
  * 阿里云
  * linode
* 部署流程

## 参考项目
* https://github.com/limingth/maodou
* https://github.com/luckyyang/vote
* 高德地图定位集成：https://github.com/limingth/didipoop
* Ten meteor project you should know: https://github.com/maodouio/meteor-lean-startup-camp/wiki/Ten-meteor-project-you-should-know
* 孵化营项目微足：http://182.92.79.206/
* https://github.com/seanrose/broadcast
