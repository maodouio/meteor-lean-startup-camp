# THE BEST METEOR PACKAGES YOU MUST KNOW TO CODE FASTER THAN EVER

 [原文链接](https://gentlenode.com/journal/meteor-22-the-best-meteor-packages-you-must-know-to-code-faster-than-ever/52)

Regarding productivity, Meteor is undoubtedly one of the best frameworks you can find. But do you know that you can even be more efficient by knowing some of the most useful packages built by the community? [There are currently 3500+ packages available on Atmosphere](https://atmospherejs.com/) and they cover a wide range of use cases. We tried in this article to reference the most complete packages in order to save you time.

New packages are created every week and a great way to stay up-to-date is to check [the package category on Crater ](http://crater.io/category/packages)or [the most recent packages pushed to Atmosphere](https://atmospherejs.com/packages/recent). If we missed an important one that caught your attention, please add a comment.

To add a package in your Meteor application, open your terminal and use the `meteor add` command.

    # Add Iron Router to your project
	meteor add iron:router
	
	# Core packages do not need to be prefixed by the author's name.
	meteor add accounts-password
	
	# You can also add multiple packages with one command
	meteor add iron:router accounts-password
To query for available packages, use the `meteor search` command.

meteor search kadira

	> Matching packages:
	> meteorhacks:kadira    Performance Monitoring for Meteor
	
	# You can use 'meteor show' to get more information on a specific item.
Note: Is Atmosphere a little slow to respond? Take a look at [fastosphere](http://fastosphere.meteor.com/), a blazing fast Meteor packages search powered by Algolia.

## CORE PACKAGES

You can take a look at all 120+ core packages [available in the Meteor repository](https://github.com/meteor/meteor/tree/devel/packages). Here are a few ones that may interest you.

- [appcache](https://github.com/meteor/meteor/tree/devel/packages/appcache): Stores the static parts of a Meteor application (the client side Javascript, HTML, CSS, and images) in the browser's application cache.
- [browser-policy](https://github.com/meteor/meteor/tree/devel/packages/browser-policy): Lets you set security-related policies that will be enforced by newer browsers. These policies help you prevent and mitigate common attacks like cross-site scripting and - clickjacking.
- [check](https://github.com/meteor/meteor/tree/devel/packages/check): Lightweight package for argument checking and general pattern matching.
- [fastclick](https://github.com/meteor/meteor/tree/devel/packages/fastclick): A simple, easy-to-use library for eliminating the 300ms delay between a physical tap and the firing of a click event on mobile browsers.

## PACKAGES FOR TEMPLATES & STYLESHEETS

The Meteor community has built a lot of packages to make work easier with templates. Here are a few packages you should look at to increase your productivity.

- [raix:handlebar-helpers](https://github.com/raix/Meteor-handlebar-helpers): This package provides handy helpers and a simple way of using sessions and collections in the Meteor Spacebars template environment.
- [mquandalle:jade](https://github.com/mquandalle/meteor-jade): Provides support for the Jade template engine as a Spacebars alternative and have some additional features like a `else if` component.
- [fourseven:scss](https://github.com/fourseven/meteor-scss): This allows .scss and .sass files to work with Meteor (compile them through node-sass).
- f[rancocatena:compass](https://github.com/francocatena/meteor-compass): Compass 0.13.alpha.4 packaged for Meteor. This package requires `fourseven:scss` to work.
- [dburles:spacebars-tohtml](https://github.com/dburles/meteor-spacebars-tohtml): A simple helper function to assist with rendering spacebars to HTML. Works on both the server and the client. This is very useful for sending HTML emails.

## ROUTING PACKAGES & EXTENSIONS

One of the most key components of every project is the routing system. Iron router is considered as the official router for Meteor. It will help you build your first routes in a snap but you will sometimes want to implement additional features. Before doing so, take a look at the packages below.

- [iron:router](https://github.com/eventedmind/iron-router/): Routing specifically designed for Meteor. A router that works on the server and the browser, designed specifically for Meteor.
- [zimme:iron-router-auth](https://github.com/zimme/meteor-iron-router-auth): Extends the iron-router package, allowing you to quickly lock routes down to authenticated users. It also provides the ability to auto-redirect back to the previous route on a successful login.
- [martino:iron-router-i18n](https://github.com/yoolab/iron-router-i18n): Add i18n support for the popular Iron Router package.
- [zimme:iron-router-active](https://github.com/zimme/meteor-iron-router-active): Active route/path template helpers for Iron Router.
- [multiply:iron-router-progress](https://github.com/Multiply/iron-router-progress): A little package that implements a simple progress bar (using [nProgress](http://ricostacruz.com/nprogress/)), when loading different routes ([check examples here](https://iron-router-progress.meteor.com/)).
- [manuelschoebel:wait-on-lib](https://github.com/DerMambo/wait-on-lib): Use Iron-Router waitOn to load external javascript libraries.

## OPTIMIZE YOUR APPLICATION WITH THESE PACKAGES

Trying to scale and optimize your Meteor application? We recommend that you take a look at [Meteor Bulletproof](https://bulletproofmeteor.com/), a resource that will help you build faster apps. Meanwhile, here are a few packages we use in our projects to make them more efficient.

- [meteorhacks:fast-render](https://github.com/meteorhacks/fast-render): Fast Render can improve the initial load time of your app, giving you 2-10 times faster initial page loads. It provides the same effect as Server Side Rendering (SSR), but still sends data over the wire to avoid breaking one of Meteor’s core principles.
- [meteorhacks:unblock](https://github.com/meteorhacks/unblock): Provide `this.unblock` functionality to publications.
- [meteorhacks:subs-manager](https://github.com/meteorhacks/subs-manager/blob/master/package.js): Subscriptions Manager for Meteor. Subscriptions Manager caches your subscriptions and runs all the subscriptions that have been cached when a route is changed. This means that when switching between routes, the user will no longer have to wait. Also, Meteor won't need to re-send data that's already in the client.

## PACKAGES FOR COLLECTIONS & PUBLICATIONS/SUBSCRIPTIONS

[Collections are Meteor's way of storing persistent data](https://www.meteor.com/try/3). They can be accessed from both the server and the client and update themselves automatically. You can find multiple packages below that provides additional features to manage and play with them.

- [aldeed:collection2](https://github.com/aldeed/meteor-collection2): A Meteor package that extends Mongo.Collection to provide support for specifying a schema and then validating against that schema when inserting and updating.
- [dburles:collection-helpers](https://github.com/dburles/meteor-collection-helpers): Collection helpers automatically sets up a transformation on your collections allowing for simple models, with an interface similar to template helpers.
- [mrt:collection-api](https://github.com/crazytoad/meteor-collectionapi): Allows you to easily perform CRUD operations on Meteor Collections over HTTP/HTTPS from outside of the Meteor client or server environment (or how to build an API in a few minutes).
- p[ercolate:paginated-subscription](https://github.com/percolatestudio/paginated-subscription/): Adds pagination to Meteor's standard subscriptions.
- [cfs:standard-packages](https://github.com/CollectionFS/Meteor-CollectionFS): CollectionFS is a smart package for Meteor that provides a complete file management solution including uploading, downloading, storage, synchronization, manipulation, and copying. It supports several storage adapters for saving to the local filesystem, GridFS, or S3, and additional storage adapters can be created.
- [matb33:collection-hooks](https://github.com/matb33/meteor-collection-hooks): Extends `Mongo.Collection` with before/after hooks for `insert`, `update`, `remove`, `find`, and `findOne`. Works across both client, server or a mix. Also works when a client initiates a collection method and the server runs the hook, all while respecting the collection validators (allow/deny).
- [reywood:publish-composite](https://github.com/englue/meteor-publish-composite): Meteor.publishComposite(...) provides a flexible way to publish a set of related documents from various collections using a reactive join. This makes it easy to publish a whole tree of documents at once. The published collections are reactive and will update when additions/changes/deletions are made.
- [dburles:factory](https://github.com/percolatestudio/meteor-factory): Meteor package for creating test data or generating fixtures.
 
## PACKAGES FOR YOUR FORMS

Forms are among the most used components of every website. The packages below will help you build and validate your forms faster.

- [aldeed:autoform](https://github.com/aldeed/meteor-autoform): A smart package for Meteor that adds UI components and helpers to easily create basic forms with automatic insert and update events, and automatic reactive validation.
- t[emplates:forms](https://github.com/meteortemplates/forms): Build production-ready, reactive forms in minutes. Even complex workflows can be achieved with just a few lines of code. A light-weight alternative to AutoForm based around reusable components.
- [copleykj:mesosphere](https://github.com/copleykj/Mesosphere): A dual client/server side form data validation, transformation, and aggregation package for Meteor.
- [matteodem:easy-search](https://github.com/matteodem/meteor-easy-search): Easy-to-use search with Blaze Components (includes Elastic Search Support).
- [mizzao:autocomplete](https://github.com/mizzao/meteor-autocomplete/): Client/server autocompletion designed for Meteor's collections and reactivity. Looking for a more minimalistic autocompletion package? [Check this one](https://github.com/sebdah/meteor-autocompletion).

## PACKAGES FOR MOBILE DEVELOPMENT

[August 2014, Meteor released a stunning feature](https://www.youtube.com/watch?v=4dJLPLWMImw): the ability to compile your application, thanks to Cordova, to iOS and Android devices.[ With isomorphic always in mind](https://www.meteor.com/blog/2014/08/28/isobuild-why-meteor-created-a-new-package-system), a lot of useful packages for mobile development have emerged.

- [meteoric:ionic](https://github.com/meteoric/meteor-ionic): This is an attempt at real Ionic and Meteor integration. This is not just Ionic's CSS framework wrapped in a Meteor package. It aims to be a complete port of Ionic’s Angular directives to Meteor Blaze templates. Also, check the complementary packages [Ionic-SASS](https://github.com/meteoric/ionic-sass) and [Ionicons-SASS](https://github.com/meteoric/ionicons-sass).

## TESTING PACKAGES

There was a time where testing a Meteor application was kind of hard. But now, [with Velocity](https://github.com/meteor-velocity/velocity), you can integrate several testing frameworks like mocha, cucumber or jasmine and run reactive tests in a snap.

- v[elocity:core](https://github.com/meteor-velocity/velocity): A reactive test-runner for Meteor. Integrates easily with Jasmine, Cucumber, Mocha, CasperJs and Nightwatch ([read more](http://velocity.meteor.com/)).
- [velocity:html-reporter](https://github.com/meteor-velocity/html-reporter/): HTML reporter for Meteor's Velocity testing framework.
- [sanjo:jasmine](https://github.com/Sanjo/meteor-jasmine): Easily write and run Jasmine tests for all your Meteor code.
- [mike:mocha](https://github.com/mad-eye/meteor-mocha-web): This meteor package allows you to easily and safely run mocha tests within Meteor.
- [xolvio:cucumber](https://github.com/xolvio/meteor-cucumber): Gherkin sytax testing for Meteor using Cucumber.js, served as a Velocity test framework.
- [clinical:nightwatch](https://github.com/awatson1978/clinical-nightwatch): Ultra-easy acceptance testing for your Meteor app with Selenium and Nightwatch.
- [nblazer:casperjs](https://github.com/blazer82/meteor-casperjs/): CasperJS end to end test integration for meteor using velocity.
- [anti:gagarin](https://github.com/anticoders/gagarin): Gagarin is a tool you can use in your tests to run Meteor apps in a sandboxed environment. It's useful when you need more refined control over the meteor processes and test fancy things, e.g. the behavior of your app on server restarts or when you have multiple app instances writing to the same database.

## PACKAGES FOR SEO/SMO

SEO and SMO are important marketing aspects. You need to configure your application to make them return the things you want search engines and social medias to see/display.

- [manuelschoebel:ms-seo](https://github.com/DerMambo/ms-seo): A SEO helper package for Meteor ([read more in this article](http://www.manuel-schoebel.com/blog/meteor-and-seo)).
- [gadicohen:sitemaps](https://github.com/gadicc/meteor-sitemaps): Create valid and dynamic sitemaps using your own functions.

## ACCOUNTS & ROLE PACKAGES.

Building an account system with Meteor is straightforward. You probably know the core package `accounts-password` but here are a few extensions that will provide to your app additional features.

- [alanning:roles](https://github.com/alanning/meteor-roles): An authorization package for Meteor - compatible with built-in accounts package. Lets you attach permissions to a user which you can then check against later when deciding whether to grant access to Meteor methods or publish data.
- [artwells:accounts-guest](https://github.com/artwells/meteor-accounts-guest/): Automatically add visitor as anonymous guest with userId. Each non-logged in visitor gets a userId, accessible via Accounts and `Meteor.userId()`.
- [mizzao:user-status](https://github.com/mizzao/meteor-user-status): Keeps track of user connection data, such as IP addresses, user agents, and client-side activity, and tracks this information in Meteor.users as well as some other objects. This allows you to easily see users that are online, for applications such as rendering the users box below showing online users in green and idle users in orange.
- [useraccounts:core](https://github.com/meteor-useraccounts/core): User Accounts is a suite of packages for the Meteor.js platform. It provides highly customizable user accounts UI templates for many different front-end frameworks. At the moment it includes forms for sign in, sign up, forgot password, reset password, change password, enroll account, and link or remove of many 3rd party services. (also, [check his themes](https://atmospherejs.com/useraccounts))
- [joshowens:accounts-entry](https://github.com/Differential/accounts-entry): accounts-entry is a meteorite package that relies on Iron Router and provides an alternative interface to accounts-ui, with whole pages for sign up and sign in.

## DEPLOYMENT AND MONITORING PACKAGES

We wrote last year a utorial on [thow to deploy a Meteor application on Ubuntu](https://gentlenode.com/journal/meteor-1-deploy-and-manage-a-meteor-application-on-ubuntu-with-nginx/1) and [how to use MUP to easily configure your server](https://gentlenode.com/journal/meteor-19-deploying-your-applications-in-a-snap-with-meteor-up-mup/41). You will find below additional packages to test and monitor your app so as to be sure that everything is running well.

- [Meteor Up](https://github.com/arunoda/meteor-up): Meteor Up (MUP for short) is a command line tool that allows you to initialize/configure your Debian/Ubuntu and Open Solaris server and to deploy your Meteor application with a single line. It's not a meteor package and it can be installed with `npm install -g mup`.
- [Meteor Load Test](https://github.com/alanning/meteor-load-test): A load testing tool for Meteor applications that utilizes [the Grinder](http://grinder.sourceforge.net/) to manage agents.
- [meteorhacks:kadira](https://github.com/meteorhacks/kadira): Integrate your Meteor application with Kadira for performance monitoring.
- p[ercolate:server-info](https://github.com/percolatestudio/meteor-server-info): A Meteor package for querying an application for diagnostics information. sets up a route (By default at /info) that returns a json object containing useful debugging data.
- [mrt:server-stats](https://github.com/hharnisc/meteor-server-stats): A Meteor package to grab system stats (cpu, memory, load, versions, hostname) from the server.

## PACKAGES FOR THIRD-PARTIES PLATFORMS

If you are trying to integrate a third-party service with your application, chances are that someone has already built a package for that. That's why it's important that you check Atmosphere so as to avoid reinventing the wheel.

- [datariot:ganalytics](https://github.com/datariot/meteor-ganalytics): Log page views and events to Google Analytics.
- [obvio171:disqus](https://github.com/obvio171/meteor-disqus): Disqus package for Meteor. Add {{>disqus}} to template. Be happy.
- [limemakers:paypal](https://github.com/LimeMakers/meteor-paypal/): Meteor Package for easy Paypal payment processing.
- [mrgalaxy:stripe](https://github.com/tyler-johnson/stripe-meteor): Stripe.js and Node-Stripe brought to Meteor.
- [cunneen:mailgun](https://github.com/cunneen/meteor-mailgun): A meteorite package for sending emails easily using Mailgun.

## ADMINISTRATION PACKAGES

A few awesome packages we use to generate an administration quickly.

- h[ouston:admin](https://github.com/gterrono/houston): Houston is a zero-config Meteor Admin, modeled after Django Admin, intended as a simple way for developers to give end-users (or themselves) an easy way to view and manipulate their app's data.
- [yogiben:admin](https://github.com/yogiben/meteor-admin): A complete admin dashboard solution for meteor built off the iron-router, roles and autoform packages and frontend from the open source admin dashboard template, Admin LTE.
- t[ail:core](https://github.com/Tarang/Meteor-Analytics): A super cool analytics package for Meteor.

## SECURITY PACKAGES

If you read [Sacha Greif's article about Security](https://www.discovermeteor.com/blog/meteor-and-security/), here are a some packages that will help you to enhance your app and go further.

- [matteodem:easy-security](https://github.com/matteodem/meteor-easy-security): Protection against harmful attacks by rate limiting remote method calls.
- [ongoworks:security](https://github.com/ongoworks/meteor-security): A Meteor package that provides a simple, logical, plain language API for defining write security on your MongoDB collections. Wraps the core allow/deny security.

## DEBUGGING PACKAGES

The following packages will help you debug your Meteor application and make your life easier.

- m[savin:mongoinspector](https://github.com/msavin/MongoInspector): Meteor package for visualizing your collections in the browser.

## METEOR BOILERPLATES

When starting a new project, you need to think about the way you will organize your application. If you are an experienced Meteor developer, you probably have your own ready-to-start Meteor repository or are using one of the boilerplates below.

- [Meteor Boilerplate (Differential)](https://github.com/Differential/meteor-boilerplate): A starting point for Meteor applications. Includes iron-router, Bootstrap 3, Font Awesome, LESS and more.
- A[nother Meteor Boilerplate (Matteo Dem)](https://github.com/matteodem/meteor-boilerplate): This boilerplate is here to give you a starting point for your meteor projects, with a console tool to ease up some tasks. Essential atmosphere packages are included to give you features like routing and collection schemas out-of-the-box.
- [Meteoric Boilerplate](https://github.com/dalequi/meteor-meteoric-boilerplate): A Boilerplate for Meteor using [Meteor Ionic](https://github.com/meteoric/meteor-ionic) as base. If you would like to build mobile application with Meteor, Cordova & Ionic, that's a good way to start a project in a snap and save time.

## MISCELLANEOUS PACKAGES

To conclude this long list, here are some packages you should look at.

- [tap:i18n](https://github.com/TAPevents/tap-i18n): tap-i18n is a Meteor package that provides a comprehensive i18n solution for Meteor apps and packages, with the goal of standardizing the way package developers internationalize their packages (used by Telescope and more).
- [ryw:blog](https://github.com/Differential/meteor-blog): Gives you a basic, out-of-the-box blog at `/blog`.
- [percolate:synced-cron](https://github.com/percolatestudio/meteor-synced-cron): A simple cron system for Meteor. It supports syncronizing jobs between multiple processes. In other words, if you add a job that runs every hour and your deployment consists of multiple app servers, only one of the app servers will execute the job each time (whichever tries first).
- [sacha:spin](https://github.com/SachaG/meteor-spin): A Meteor package wrapper for Spin.js via Npm.depends(). Allows you to add and configure spinner in your template with `{{> spinner}}`.
- [template:tabs](templates:tabs): Reactive tabbed interfaces compatible with routing.
- [dandv:http-more](dandv:http-more): Make HTTP calls to remote servers, passing any extra options to the underlying backend.
- a[nti:fake](https://github.com/anticoders/meteor-fake): Random text and joyful names generator.
