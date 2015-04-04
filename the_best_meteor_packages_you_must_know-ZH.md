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

表单是所有网站中使用最多的组件，下面这些包帮助你更快地搭建和验证表单。

- [aldeed:autoform](https://github.com/aldeed/meteor-autoform): 一个灵巧（smart）的包，它为 Meteor 添加 UI 组件和帮助类，从而更轻易地创建出带有自动插入、更新事件，以及自动跟随地验证功能的基础表单。
- [templates:forms](https://github.com/meteortemplates/forms): 分分钟搭个可以用于生产环境的随动表单。即使工作流程复杂，也能用几行代码搞定。是`AutoForm`基于可复用组件的轻量版本。
- [copleykj:mesosphere](https://github.com/copleykj/Mesosphere): 一个可以在客户端和服务器端双向对表单数据进行验证，转换和拼装的包。
- [matteodem:easy-search](https://github.com/matteodem/meteor-easy-search): 易于使用的搜索，带[Blaze Components](https://matteodem.github.io/meteor-easy-search/docs/blaze-components/)，（支持[Elastic Search](https://matteodem.github.io/meteor-easy-search/docs/elastic-search/)）。
- [mizzao:autocomplete](https://github.com/mizzao/meteor-autocomplete/): 为 Meteor 的集合（collections）和随动（reactivity）所设计的客户端/服务器端自动补全包，想要个再简洁点的自动补全的包? [戳这](https://github.com/sebdah/meteor-autocompletion).

## 关于移动端开发的包 PACKAGES FOR MOBILE DEVELOPMENT

[2014年8月，Meteor 发布了一个令人惊叹的功能](https://www.youtube.com/watch?v=4dJLPLWMImw)：把你的应用（Application）编译后跑在 iOS 和安卓设备上（多亏有了 Cordova）。[心里总是想着同构（isomorphic）](https://www.meteor.com/blog/2014/08/28/isobuild-why-meteor-created-a-new-package-system)，一大波用于移动端开发的好用的包涌现出来。

- [meteoric:ionic](https://github.com/meteoric/meteor-ionic): 该包是首次对`Ionic`和`Meteor`真正集成的尝试。它不仅仅是将`Ionic`的`CSS`框架包装成一个`Meteor`包。它旨在于把`Ionic`的`Angular`指令（directives）完美移植成`Meteor Blaze`模板。还有，再看看补充包 [Meteor-SASS](https://github.com/meteoric/ionic-sass) 和 [Ionicons-SASS](https://github.com/meteoric/ionicons-sass).

## 关于测试的包 TESTING PACKAGES

在曾经的一段时间里，测试一个 Meteor 应用是个难事。但是现在，有了[Velocity](https://github.com/meteor-velocity/velocity)，你可以把多种测试框架如：mocha，cucumber或jasmine集成进来，并立即跑起随动（reactive）的测试。

- [velocity:core](https://github.com/meteor-velocity/velocity): Meteor的一个跑测试的东西，轻松与 Jasmine、Cucumber、Mocha、CasperJs及 Nightwatch集成。
- [velocity:html-reporter](https://github.com/meteor-velocity/html-reporter/): 为Meteor的Velocity测试框架生成HTML报表。
- [sanjo:jasmine](https://github.com/Sanjo/meteor-jasmine): 给你所有的 Meteor 代码轻松写出并运行Jasmine测试。
- [mike:mocha](https://github.com/mad-eye/meteor-mocha-web): 该包让你轻松安全地在Meteor中跑 mocha 测试。
- [xolvio:cucumber](https://github.com/xolvio/meteor-cucumber): Gherkin sytax testing for Meteor using Cucumber.js, served as a Velocity test framework.
- [clinical:nightwatch](https://github.com/awatson1978/clinical-nightwatch): 它使用Selenium和Nightwatch对你的 Meteor 应用做超容易的验收测试。
- [nblazer:casperjs](https://github.com/blazer82/meteor-casperjs/): 使用 Velocity 做端到端的 CasperJS 测试集成。
- [anti:gagarin](https://github.com/anticoders/gagarin): Gagarin 是一个可以在沙盒环境中测试运行 Meteor 应用的工具。它在你需要对 meteor 流程做更精准控制或者测试一些花哨的东西（比如：重启服务器或者多个应用实例写同一个数据库时的表现）时很有用。

## 关于SEO/SMO的包 PACKAGES FOR SEO/SMO

SEO 和 SMO 在营销上面显为重要。你需要对应用进行配置，来使得它们可以返回你想要给搜索引擎与社交媒体来发现和展示的东西。

- [manuelschoebel:ms-seo](https://github.com/DerMambo/ms-seo): 一个 SEO 帮手的 Meteor 包，点这篇[文章](http://www.manuel-schoebel.com/blog/meteor-and-seo)查看更多。
- [gadicohen:sitemaps](https://github.com/gadicc/meteor-sitemaps): 用自己的功能（functions）创建有效且动态的网站地图（sitemaps）。

## 关于账户和角色的包 ACCOUNTS & ROLE PACKAGES.

用 Meteor 创建账户系统很简单。大家可能已经知道核心包 `accounts-password`了，但是还有一些扩展可以锦上添花。

- [alanning:roles](https://github.com/alanning/meteor-roles): Meteor 的一个用来实现授权的包。它兼容于Meteor内置的`acounts`包。它可以为一个用户添加权限，并让你在以后决定授以Meteor方法或发布的数据访问权限时，可以检测该用户是否有足够权限。
- [artwells:accounts-guest](https://github.com/artwells/meteor-accounts-guest/): 给匿名访客自动添加`userId`，任何未登录访客都将获得一个用户ID（userId），这个用户ID可以通过账户和`Meteor.userId()`方法拿到。
- [mizzao:user-status](https://github.com/mizzao/meteor-user-status): 跟踪用户的连接数据，如：IP地址、客户端信息及活动，还能在`Meteor.users`及某些对象中追踪这些信息。这样你就可以方便地知道哪些用户是在线的，从而可以在应用中用红绿色来区分显示在线用户和空闲用户。
- [useraccounts:core](https://github.com/meteor-useraccounts/core): `User Accounts`是为`Meteor.js`平台提供的一系列包。它为许多不同的前端框架提供高可定制的用户账户UI模板。目前为止，包含有登录、注册、忘记密码、重置密码、修改密码、登记账号（enroll account）表单，还有链接至第三方服务或者移除第三方服务。（它还有各种[主题](https://atmospherejs.com/useraccounts)）。
- [joshowens:accounts-entry](https://github.com/Differential/accounts-entry): `accounts-entry`是一个依赖于`Iron Router`并为`accounts-ui`提供替代界面（含登录和注册全部页面）的`meteorite`包。

## 关于部署和监控的包 DEPLOYMENT AND MONITORING PACKAGES

去年，我们在[thow to deploy a Meteor application on Ubuntu](https://gentlenode.com/journal/meteor-1-deploy-and-manage-a-meteor-application-on-ubuntu-with-nginx/1) and [how to use MUP to easily configure your server](https://gentlenode.com/journal/meteor-19-deploying-your-applications-in-a-snap-with-meteor-up-mup/41)上写了一个教程。大家可以使用以下的包来测试和监控你的应用来保证它的正常运转。

- [Meteor Up](https://github.com/arunoda/meteor-up): Meteor Up (简称MUP) 是一个命令行工具，一行命令就可以让你在Debian/Ubuntu和Open Solaris服务器上初始化/配置/发布你的Meteor应用。它不是meteor包，可以通过命令`npm install -g mup`来安装。
- [Meteor Load Test](https://github.com/alanning/meteor-load-test): 利用[the Grinder](http://grinder.sourceforge.net/) 来管理agents的负载测试工具。
- [meteorhacks:kadira](https://github.com/meteorhacks/kadira): 集成`Kadira`来做Meteor应用的性能监控。
- [percolate:server-info](https://github.com/percolatestudio/meteor-server-info): 这个包通过一个路由（默认为 /info）来提供一个有调试数据的 JSON 对象，从而查询到应用的诊断信息。
- [mrt:server-stats](https://github.com/hharnisc/meteor-server-stats): 该包可以抓取到服务器的系统统计信息，如：CPU、内存、负载、版本、主机名。

## 关于第三方平台的包 PACKAGES FOR THIRD-PARTIES PLATFORMS

如果你要集成一个第三方服务到你的应用中，没准已经有人做了包干这个事。所有为避免重造轮子，检查Atmosphere上的包就尤为重要。

- [datariot:ganalytics](https://github.com/datariot/meteor-ganalytics): 记录页面和事件到谷歌日志分析中。
- [obvio171:disqus](https://github.com/obvio171/meteor-disqus): 相应的Disqus包。在模板中添加`{{>disqus}}`，真好。
- [limemakers:paypal](https://github.com/LimeMakers/meteor-paypal/): 相应的PayPal支付流程包。
- [mrgalaxy:stripe](https://github.com/tyler-johnson/stripe-meteor): 相应的Stripe.js与Node-Stripe包。
- [cunneen:mailgun](https://github.com/cunneen/meteor-mailgun): 用Mailgun轻松发送邮件的meteorite包。

## 关于管理的包 ADMINISTRATION PACKAGES

一些牛逼的包，立马做好管理

- [houston:admin](https://github.com/gterrono/houston): Houston是个零配置的Meteor Admin, 承自Django Admin, 希望以一种简单方式来为最终用户或者开发者自身轻松地做到查看和操控应用的数据。
- [yogiben:admin](https://github.com/yogiben/meteor-admin): 一个完整的管理dashboard解决方案，代替掉`icon-router`、`roles`和`autoform`包以及开源的管理dashboard模板（Admin LTE）的前端。
- [tail:core](https://github.com/Tarang/Meteor-Analytics): 一个超酷的管理分析包。

## 关于安全的包 SECURITY PACKAGES

如果你读过[Sacha Greif's article about Security](https://www.discovermeteor.com/blog/meteor-and-security/)，下面这些包可以帮助你更好地稳固应用。

- [matteodem:easy-security](https://github.com/matteodem/meteor-easy-security): 通过对远程方法调用限速来阻止有害的攻击。
- [ongoworks:security](https://github.com/ongoworks/meteor-security): 该包提供一个简单、有逻辑、朴素（plain）的语言API来定义你的MongoDB的collections上的写安全。包装了核心的允许/拒绝（allow/deny）安全。

## 关于调试的包 DEBUGGING PACKAGES

下面的包帮助你调试Meteor应用，让生活更美好。

- [msavin:mongoinspector](https://github.com/msavin/MongoInspector): 在浏览器里可视化Meteor的collections。

## 关于样板的包 METEOR BOILERPLATES

开始一个新的项目，你需要考虑好如何搭好应用的架子。如果你是开发Meteor的老鸟了，可能早有了自己的随时待命（ready-to-start）的Meteor仓库（repository）或者是下面这些样板之一：

- [Meteor Boilerplate (Differential)](https://github.com/Differential/meteor-boilerplate): Meteor应用的起点。包括了`iron-router`、`Bootstrap 3`、`Font Awesome`、`LESS`及其他。
- [Another Meteor Boilerplate (Matteo Dem)](https://github.com/matteodem/meteor-boilerplate): 同样是Meteor应用的起点，有一个轻松干活的控制台工具。含有必要的asmosphere包提供开箱即用的功能，如：路由(routing)和collection schemas。
- [Meteoric Boilerplate](https://github.com/dalequi/meteor-meteoric-boilerplate): A Boilerplate for Meteor using [Meteor Ionic](https://github.com/meteoric/meteor-ionic) as base. If you would like to build mobile application with Meteor, Cordova & Ionic, that's a good way to start a project in a snap and save time.
- [Meteoric Boilerplate](https://github.com/dalequi/meteor-meteoric-boilerplate): 使用[Meteor Ionic](https://github.com/meteoric/meteor-ionic)做为基础的一个Meteor样板。如果你想用`Meteor`、`Cordova & Ionic`做移动端应用，这是快速开始项目，节省时间的好办法。

## 其他牛逼的包 MISCELLANEOUS PACKAGES

这个长长的列表最后，还有这些包要瞅瞅。

- [tap:i18n](https://github.com/TAPevents/tap-i18n): 对Meteor应用及其包的语言国际化（i18n）全面解决方案。它旨在于使Meteor包的开发者们在做语言国际化时有标准可循，现在已被`Telescope`和更多的Meteor包使用。
- [ryw:blog](https://github.com/Differential/meteor-blog): 一个基础的、开箱即用的博客，位于 `/blog`。
- [percolate:synced-cron](https://github.com/percolatestudio/meteor-synced-cron): Meteor上简单的`cron`系统。它支持在多个处理器上同步任务（jobs）。换言之，如果你的布署含多个应用服务器，现在要添加一个每个小时运行一次的任务，但每次只能有一个应用服务器跑这个任务（不管哪个服务器抢到）。
- [sacha:spin](https://github.com/SachaG/meteor-spin): 一个通过`Npm.depends()`包装`Spin.js`的包。它让你使用`{{> spinner}}`来做添加和配置模板中的spinner。
- [template:tabs](templates:tabs): 与routing兼容的随动的tabbed界面。
- [dandv:http-more](dandv:http-more): 向远程服务器发送HTTP调用，传送任意额外的选项给底层后台。
- [anti:fake](https://github.com/anticoders/meteor-fake): 随机的文字和欢乐的名字生成器。
