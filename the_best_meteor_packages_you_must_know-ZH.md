# 带你装逼带你飞的超屌Meteor Packages

 [原文链接](https://gentlenode.com/journal/meteor-22-the-best-meteor-packages-you-must-know-to-code-faster-than-ever/52)

提到开发效率，meteor无疑是你所能找到的最好框架之一。通过meteor社区提供的一些实用的包（package），你的效率还会更高。目前在[Atmosphere](https://atmospherejs.com/)上有3500+个有效的包，它们被大量实例应用。为了节省你的时间，我们尝试引用使用最频繁的包。

每周都有新包被开发出，好地方式就是经常检查[the package category on Crater ](http://crater.io/category/packages)or [the most recent packages p ushed to Atmosphere](https://atmospherejs.com/packages/recent)。如果有哪些重要的包被我们错过，请你与我们联系哦~

如何添加一个包在你的meteor app。打开你的终端，使用`meteor add PackageName` 命令:

    # Add Iron Router to your project
	meteor add iron:router
	
	# Core packages do not need to be prefixed by the author's name.
	meteor add accounts-password
	
	# You can also add multiple packages with one command
	meteor add iron:router accounts-password

如何查询可用的包。使用`meteor search PackageName`命令:

注意:atmosphere反应有点慢吗？去[fastosphere](http://fastosphere.meteor.com/)看看，Algolia帮助你超快地提供了搜索meteor包。

## 核心包 CORE PACKAGES

核心包有120多个，在[这里](https://github.com/meteor/meteor/tree/devel/packages)可以查看它们. 这里我们列举几个你可能会感兴趣的包.

- [appcache](https://github.com/meteor/meteor/tree/devel/packages/appcache): 帮助在浏览器的缓存（cache）中保存Meteor应用的静态数据(即，客户端的Javascript, HTML, CSS, and images）

- [browser-policy](https://github.com/meteor/meteor/tree/devel/packages/browser-policy): 让你可以在新的浏览器设定安全相关（security-related）的规则（policy）。这些规则可以帮助你防止和缓解常见的网络攻击，如：跨站脚本攻击、点击劫持等

- [check](https://github.com/meteor/meteor/tree/devel/packages/check): 参数校验和模式匹配的轻量级包。

- [fastclick](https://github.com/meteor/meteor/tree/devel/packages/fastclick):一个简单易用的库，可以去除300秒的延迟 between a physical tap and the firing of a click event on mobile browsers.

## 关于模板和CSS的包 PACKAGES FOR TEMPLATES & STYLESHEETS

Meteor社区已经有许多包可以让大家更快捷地处理模板（template）。想要提高Meteor开发效率，下面这些包值得一看。

- [raix:handlebar-helpers](https://github.com/raix/Meteor-handlebar-helpers): 这个包提供了在Meteor Spacebars模板环境中使用会话（session）和集合（collection）的帮助方法helper。
- [mquandalle:jade](https://github.com/mquandalle/meteor-jade): Provides support for the Jade template engine as a Spacebars alternative and have some additional features like a `else if` component.
- [mquandalle:jade](https://github.com/mquandalle/meteor-jade): 与Spacebar是同类，提供了一套Jade模板引擎（Jade template engine），还提供了其他的功能，例如`else if`组件。 
- [fourseven:scss](https://github.com/fourseven/meteor-scss): 让Meteor项目可以使用.scss和.sass文件（通过node-sass编译）。
- [francocatena:compass](https://github.com/francocatena/meteor-compass): 为Meteor定制的compass。这个包依赖于`fourseven:scss`。
- [dburles:spacebars-tohtml](https://github.com/dburles/meteor-spacebars-tohtml): 提供了渲染spacebars入html超赞的帮助方法（helper）。这对发送html email有很大帮助。

## 关于路由和插件的包 ROUTING PACKAGES & EXTENSIONS

路由对于每个项目都是非常重要的组件。 Iron路由被认为是Meteor的官方路由。他可以帮助你在极短时间内建立路由并完成配置。

- [iron:router](https://github.com/eventedmind/iron-router/): 为Meteor定制的路由组件，可以同时在server和brower运行。
- [zimme:iron-router-auth](https://github.com/zimme/meteor-iron-router-auth): 扩展了iron-router, 允许快速锁定验证用户的路由。对于已登录用户，它可以提供自动重定向回到上一路由的帮助方法。 
- [martino:iron-router-i18n](https://github.com/yoolab/iron-router-i18n): 添加对iron-router的i18n的支持。
- [zimme:iron-router-active](https://github.com/zimme/meteor-iron-router-active): Active route/path template helpers for Iron Router.
- [multiply:iron-router-progress](https://github.com/Multiply/iron-router-progress): 在加载路由时使用[nProgress](http://ricostacruz.com/nprogress/)生成进度条。([示例](https://iron-router-progress.meteor.com/)).
- [manuelschoebel:wait-on-lib](https://github.com/DerMambo/wait-on-lib): 使用Iron-Router, 在waitOn时去加载外部js库

## 关于App优化的包 OPTIMIZE YOUR APPLICATION WITH THESE PACKAGES

如果你想延展和优化你的Meteor应用, 我们推荐你看一看 [Meteor Bulletproof](https://bulletproofmeteor.com/)。他可以帮助你更快地创建app. 同时，这里还有几个可以推荐包。 

- [meteorhacks:fast-render](https://github.com/meteorhacks/fast-render): 提高初始化加载效率2-10倍。 It provides the same effect as Server Side Rendering (SSR), but still sends data over the wire to avoid breaking one of Meteor’s core principles.
- [meteorhacks:unblock](https://github.com/meteorhacks/unblock): 为发布提供了 `this.unblock` 功能.
- [meteorhacks:subs-manager](https://github.com/meteorhacks/subs-manager/blob/master/package.js): 订阅的管理工具。Subscriptions Manager caches your subscriptions and runs all the subscriptions that have been cached when a route is changed. This means that when switching between routes, the user will no longer have to wait. Also, Meteor won't need to re-send data that's already in the client.

## 关于集合、发布/订阅的包 PACKAGES FOR COLLECTIONS & PUBLICATIONS/SUBSCRIPTIONS

[集合是Meteor数据持久化的方式](https://www.meteor.com/try/3). 这样可以在服务器端和客户端自动更新集合。你可以发现下面的很多包提供管理集合的好工具。

- [aldeed:collection2](https://github.com/aldeed/meteor-collection2): Meteor上的Mongo插件。帮助定义schema及其验证。
- [dburles:collection-helpers](https://github.com/dburles/meteor-collection-helpers): Collection helpers automatically sets up a transformation on your collections allowing for simple models, with an interface similar to template helpers.
- [mrt:collection-api](https://github.com/crazytoad/meteor-collectionapi):  帮助你通过http/https从应用外部对集合轻松地进行CURD操作;
- [percolate:paginated-subscription](https://github.com/percolatestudio/paginated-subscription/): 为订阅添加分页功能。
- [cfs:standard-packages](https://github.com/CollectionFS/Meteor-CollectionFS): CollectionFS is a smart package for Meteor that provides a complete file management solution including uploading, downloading, storage, synchronization, manipulation, and copying. It supports several storage adapters for saving to the local filesystem, GridFS, or S3, and additional storage adapters can be created.
- [matb33:collection-hooks](https://github.com/matb33/meteor-collection-hooks): Extends `Mongo.Collection` with before/after hooks for `insert`, `update`, `remove`, `find`, and `findOne`. Works across both client, server or a mix. Also works when a client initiates a collection method and the server runs the hook, all while respecting the collection validators (allow/deny).
- [reywood:publish-composite](https://github.com/englue/meteor-publish-composite): Meteor.publishComposite(...) provides a flexible way to publish a set of related documents from various collections using a reactive join. This makes it easy to publish a whole tree of documents at once. The published collections are reactive and will update when additions/changes/deletions are made.
- [dburles:factory](https://github.com/percolatestudio/meteor-factory): 帮助创建测试数据或静态测试文件
 
## 关于表单的包 PACKAGES FOR YOUR FORMS

Forms are among the most used components of every website. The packages below will help you build and validate your forms faster.

- [aldeed:autoform](https://github.com/aldeed/meteor-autoform): A smart package for Meteor that adds UI components and helpers to easily create basic forms with automatic insert and update events, and automatic reactive validation.
- [templates:forms](https://github.com/meteortemplates/forms): Build production-ready, reactive forms in minutes. Even complex workflows can be achieved with just a few lines of code. A light-weight alternative to AutoForm based around reusable components.
- [copleykj:mesosphere](https://github.com/copleykj/Mesosphere): A dual client/server side form data validation, transformation, and aggregation package for Meteor.
- [matteodem:easy-search](https://github.com/matteodem/meteor-easy-search): Easy-to-use search with Blaze Components (includes Elastic Search Support).
- [mizzao:autocomplete](https://github.com/mizzao/meteor-autocomplete/): Client/server autocompletion designed for Meteor's collections and reactivity. Looking for a more minimalistic autocompletion package? [Check this one](https://github.com/sebdah/meteor-autocompletion).

## 关于移动端开发的包 PACKAGES FOR MOBILE DEVELOPMENT

[August 2014, Meteor released a stunning feature](https://www.youtube.com/watch?v=4dJLPLWMImw): the ability to compile your application, thanks to Cordova, to iOS and Android devices.[ With isomorphic always in mind](https://www.meteor.com/blog/2014/08/28/isobuild-why-meteor-created-a-new-package-system), a lot of useful packages for mobile development have emerged.

- [meteoric:ionic](https://github.com/meteoric/meteor-ionic): This is an attempt at real Ionic and Meteor integration. This is not just Ionic's CSS framework wrapped in a Meteor package. It aims to be a complete port of Ionic’s Angular directives to Meteor Blaze templates. Also, check the complementary packages [Ionic-SASS](https://github.com/meteoric/ionic-sass) and [Ionicons-SASS](https://github.com/meteoric/ionicons-sass).

## 关于测试的包 TESTING PACKAGES

There was a time where testing a Meteor application was kind of hard. But now, [with Velocity](https://github.com/meteor-velocity/velocity), you can integrate several testing frameworks like mocha, cucumber or jasmine and run reactive tests in a snap.

- [velocity:core](https://github.com/meteor-velocity/velocity): A reactive test-runner for Meteor. Integrates easily with Jasmine, Cucumber, Mocha, CasperJs and Nightwatch ([read more](http://velocity.meteor.com/)).
- [velocity:html-reporter](https://github.com/meteor-velocity/html-reporter/): HTML reporter for Meteor's Velocity testing framework.
- [sanjo:jasmine](https://github.com/Sanjo/meteor-jasmine): Easily write and run Jasmine tests for all your Meteor code.
- [mike:mocha](https://github.com/mad-eye/meteor-mocha-web): This meteor package allows you to easily and safely run mocha tests within Meteor.
- [xolvio:cucumber](https://github.com/xolvio/meteor-cucumber): Gherkin sytax testing for Meteor using Cucumber.js, served as a Velocity test framework.
- [clinical:nightwatch](https://github.com/awatson1978/clinical-nightwatch): Ultra-easy acceptance testing for your Meteor app with Selenium and Nightwatch.
- [nblazer:casperjs](https://github.com/blazer82/meteor-casperjs/): CasperJS end to end test integration for meteor using velocity.
- [anti:gagarin](https://github.com/anticoders/gagarin): Gagarin is a tool you can use in your tests to run Meteor apps in a sandboxed environment. It's useful when you need more refined control over the meteor processes and test fancy things, e.g. the behavior of your app on server restarts or when you have multiple app instances writing to the same database.

## 关于SEO/SMO的包 PACKAGES FOR SEO/SMO

SEO and SMO are important marketing aspects. You need to configure your application to make them return the things you want search engines and social medias to see/display.

- [manuelschoebel:ms-seo](https://github.com/DerMambo/ms-seo): A SEO helper package for Meteor ([read more in this article](http://www.manuel-schoebel.com/blog/meteor-and-seo)).
- [gadicohen:sitemaps](https://github.com/gadicc/meteor-sitemaps): Create valid and dynamic sitemaps using your own functions.

## 关于账户和角色的包 ACCOUNTS & ROLE PACKAGES.

Building an account system with Meteor is straightforward. You probably know the core package `accounts-password` but here are a few extensions that will provide to your app additional features.

- [alanning:roles](https://github.com/alanning/meteor-roles): An authorization package for Meteor - compatible with built-in accounts package. Lets you attach permissions to a user which you can then check against later when deciding whether to grant access to Meteor methods or publish data.
- [artwells:accounts-guest](https://github.com/artwells/meteor-accounts-guest/): Automatically add visitor as anonymous guest with userId. Each non-logged in visitor gets a userId, accessible via Accounts and `Meteor.userId()`.
- [mizzao:user-status](https://github.com/mizzao/meteor-user-status): Keeps track of user connection data, such as IP addresses, user agents, and client-side activity, and tracks this information in Meteor.users as well as some other objects. This allows you to easily see users that are online, for applications such as rendering the users box below showing online users in green and idle users in orange.
- [useraccounts:core](https://github.com/meteor-useraccounts/core): User Accounts is a suite of packages for the Meteor.js platform. It provides highly customizable user accounts UI templates for many different front-end frameworks. At the moment it includes forms for sign in, sign up, forgot password, reset password, change password, enroll account, and link or remove of many 3rd party services. (also, [check his themes](https://atmospherejs.com/useraccounts))
- [joshowens:accounts-entry](https://github.com/Differential/accounts-entry): accounts-entry is a meteorite package that relies on Iron Router and provides an alternative interface to accounts-ui, with whole pages for sign up and sign in.

## 关于部署和监控的包 DEPLOYMENT AND MONITORING PACKAGES

We wrote last year a utorial on [thow to deploy a Meteor application on Ubuntu](https://gentlenode.com/journal/meteor-1-deploy-and-manage-a-meteor-application-on-ubuntu-with-nginx/1) and [how to use MUP to easily configure your server](https://gentlenode.com/journal/meteor-19-deploying-your-applications-in-a-snap-with-meteor-up-mup/41). You will find below additional packages to test and monitor your app so as to be sure that everything is running well.

- [Meteor Up](https://github.com/arunoda/meteor-up): Meteor Up (MUP for short) is a command line tool that allows you to initialize/configure your Debian/Ubuntu and Open Solaris server and to deploy your Meteor application with a single line. It's not a meteor package and it can be installed with `npm install -g mup`.
- [Meteor Load Test](https://github.com/alanning/meteor-load-test): A load testing tool for Meteor applications that utilizes [the Grinder](http://grinder.sourceforge.net/) to manage agents.
- [meteorhacks:kadira](https://github.com/meteorhacks/kadira): Integrate your Meteor application with Kadira for performance monitoring.
- [percolate:server-info](https://github.com/percolatestudio/meteor-server-info): A Meteor package for querying an application for diagnostics information. sets up a route (By default at /info) that returns a json object containing useful debugging data.
- [mrt:server-stats](https://github.com/hharnisc/meteor-server-stats): A Meteor package to grab system stats (cpu, memory, load, versions, hostname) from the server.

## 关于第三方平台的包 PACKAGES FOR THIRD-PARTIES PLATFORMS

If you are trying to integrate a third-party service with your application, chances are that someone has already built a package for that. That's why it's important that you check Atmosphere so as to avoid reinventing the wheel.

- [datariot:ganalytics](https://github.com/datariot/meteor-ganalytics): Log page views and events to Google Analytics.
- [obvio171:disqus](https://github.com/obvio171/meteor-disqus): Disqus package for Meteor. Add {{>disqus}} to template. Be happy.
- [limemakers:paypal](https://github.com/LimeMakers/meteor-paypal/): Meteor Package for easy Paypal payment processing.
- [mrgalaxy:stripe](https://github.com/tyler-johnson/stripe-meteor): Stripe.js and Node-Stripe brought to Meteor.
- [cunneen:mailgun](https://github.com/cunneen/meteor-mailgun): A meteorite package for sending emails easily using Mailgun.

## 关于管理的包 ADMINISTRATION PACKAGES

A few awesome packages we use to generate an administration quickly.

- [houston:admin](https://github.com/gterrono/houston): Houston is a zero-config Meteor Admin, modeled after Django Admin, intended as a simple way for developers to give end-users (or themselves) an easy way to view and manipulate their app's data.
- [yogiben:admin](https://github.com/yogiben/meteor-admin): A complete admin dashboard solution for meteor built off the iron-router, roles and autoform packages and frontend from the open source admin dashboard template, Admin LTE.
- [tail:core](https://github.com/Tarang/Meteor-Analytics): A super cool analytics package for Meteor.

## 关于安全的包 SECURITY PACKAGES

If you read [Sacha Greif's article about Security](https://www.discovermeteor.com/blog/meteor-and-security/), here are a some packages that will help you to enhance your app and go further.

- [matteodem:easy-security](https://github.com/matteodem/meteor-easy-security): Protection against harmful attacks by rate limiting remote method calls.
- [ongoworks:security](https://github.com/ongoworks/meteor-security): A Meteor package that provides a simple, logical, plain language API for defining write security on your MongoDB collections. Wraps the core allow/deny security.

## 关于调试的包 DEBUGGING PACKAGES

The following packages will help you debug your Meteor application and make your life easier.

- [msavin:mongoinspector](https://github.com/msavin/MongoInspector): Meteor package for visualizing your collections in the browser.

## 关于样板的包 METEOR BOILERPLATES

When starting a new project, you need to think about the way you will organize your application. If you are an experienced Meteor developer, you probably have your own ready-to-start Meteor repository or are using one of the boilerplates below.

- [Meteor Boilerplate (Differential)](https://github.com/Differential/meteor-boilerplate): A starting point for Meteor applications. Includes iron-router, Bootstrap 3, Font Awesome, LESS and more.
- [Another Meteor Boilerplate (Matteo Dem)](https://github.com/matteodem/meteor-boilerplate): This boilerplate is here to give you a starting point for your meteor projects, with a console tool to ease up some tasks. Essential atmosphere packages are included to give you features like routing and collection schemas out-of-the-box.
- [Meteoric Boilerplate](https://github.com/dalequi/meteor-meteoric-boilerplate): A Boilerplate for Meteor using [Meteor Ionic](https://github.com/meteoric/meteor-ionic) as base. If you would like to build mobile application with Meteor, Cordova & Ionic, that's a good way to start a project in a snap and save time.

## 其他牛逼的包 MISCELLANEOUS PACKAGES

To conclude this long list, here are some packages you should look at.

- [tap:i18n](https://github.com/TAPevents/tap-i18n): tap-i18n is a Meteor package that provides a comprehensive i18n solution for Meteor apps and packages, with the goal of standardizing the way package developers internationalize their packages (used by Telescope and more).
- [ryw:blog](https://github.com/Differential/meteor-blog): Gives you a basic, out-of-the-box blog at `/blog`.
- [percolate:synced-cron](https://github.com/percolatestudio/meteor-synced-cron): A simple cron system for Meteor. It supports syncronizing jobs between multiple processes. In other words, if you add a job that runs every hour and your deployment consists of multiple app servers, only one of the app servers will execute the job each time (whichever tries first).
- [sacha:spin](https://github.com/SachaG/meteor-spin): A Meteor package wrapper for Spin.js via Npm.depends(). Allows you to add and configure spinner in your template with `{{> spinner}}`.
- [template:tabs](templates:tabs): Reactive tabbed interfaces compatible with routing.
- [dandv:http-more](dandv:http-more): Make HTTP calls to remote servers, passing any extra options to the underlying backend.
- [anti:fake](https://github.com/anticoders/meteor-fake): Random text and joyful names generator.
