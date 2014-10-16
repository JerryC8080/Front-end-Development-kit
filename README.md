前端工具乱炖——之“百鸟归巢”
===
---

前言
---
前端的世界很精彩，也很无奈。要做好一道色香味俱全的前端菜肴，实属不易。本文罗列了一些小生接触到的框架、类库、工具之类的，旨在梳理脑海里千丝万缕的乱蚕丝。

这个世界不再是以前单纯的HTML+JS+CSS这种石器时代的概念了，我们要做的不仅仅是还原设计稿这么简单的工作了。

在这个世界，基于底层的支持，衍生出了各种框架与库。

基于我的视界，我把现在前端各种纷杂的规范、框架、类库、工具等等划分为了三层：

* Core层：由基本的HTML/HTML5、CSS/CSS3、原生JS组成，给上层提供支持。
* 架构层：由基于Core层而衍生出来的各种框架和库组成。在这层，出现了前端MVC框架、JS模块化、CSS预处理器、集成UI框架等等。
* 项目层：粒度更大，立足于项目来谈前端，像前端自动化构建、前端测试、前端优化等等。



项目构建
---

#### bower
> Bower 是 twitter 推出的一款包管理工具，基于nodejs的模块化思想，把功能分散到各个模块中，让模块和模块之间存在联系，通过 Bower 来管理模块间的这种联系。提供了注册机制、文件存储、上传下载、依赖分析等功能。

> **参考**：
> [twitter 的包管理工具 - bower](http://chuo.me/2013/02/twitter-bower.html)
> |
> [官网](http://bower.io/)




#### Grunt
> 简而言之，自动化。当你处理诸如代码最小化, 代码编译, 单元测试, 代码规范校验等等重复任务时, 你必须要做的工作越少，你的工作就变得越简单。在你完成配置后，不费吹灰之力，一个任务运行工具可以替你和你的团队完成绝大部分日常工作。

> **参考**：
> [中文社区](http://www.gruntjs.org/)
> |
> [官网](http://gruntjs.com/)


#### Gulp
> 和Grunt一样是一款前端的自动化构建工具，但是比Grunt简单和快速，但因为社区发展短，插件不多而不能替代Grunt。
> 
> **参考**：
> [官网](http://gulpjs.com/)
> |
> [Choose: Grunt, Gulp, or npm?](http://ponyfoo.com/articles/choose-grunt-gulp-or-npm)
> |
> [Gulp.js：比 Grunt 更简单的自动化的项目构建利器](http://segmentfault.com/blog/fenbox/1190000000372120)

#### LESS/SASS
>CSS预处理语言，扩展了原始的CSS，让CSS有了变量、函数、运算、继承等特性，能够提高项目CSS方面的可维护性。
> 
> **参考**：
> [为您详细比较三个 CSS 预处理器（框架）：Sass、LESS 和 Stylus](http://www.oschina.net/question/12_44255)
> |
> [Sass vs. LESS](http://css-tricks.com/sass-vs-less/)





CSS框架/UI类库
---

#### pureCss
>纯CSS 模板，响应式，提供了最基础的常用模块的样式表，包括有：网格Grids、表单Forms、按钮Buttons、表格Tables、菜单Menus。
> 
> **参考**：
> [官网](http://purecss.io/)
> |
> [Pure中文版](http://pure-site.ap01.aws.af.cm/)

#### BootStrap
>一套基于LESS的前端工具库，自称简介、直观、彪悍的前端开发框架，是一个js和css的框架，提供了具有设计的UI组件。
> 
>  **参考**：
> [官网](http://getbootstrap.com/)
> |
> [Bootstrap中文网](http://www.bootcss.com/)

#### Semantic UI
> 和其他CSS UI框架一样，提供了一系列通用的组件UI，充分利用了CSS3动画特效。根据官网的介绍，比Bootstrap更注重语义化。
> 
>  **参考**：
> [官网](http://semantic-ui.com/)
> |
> [Semantic UI中文网](http://www.semantic-ui.com.cn/)
> |
> [Semantic-UI和其他几个前端框架](http://dmyz.org/archives/548)







JS框架/类库
---

#### require.js
> RequireJS 是一个 JavaScript 文件和模块加载器，特别为浏览器优化，同时也可运行在 Rhino 和 Node 环境中
> 
> 遵循了[AMD](https://github.com/amdjs/amdjs-api/wiki/AMD)（异步模块定义规范），有提前执行、依赖前置等特点。
> 
>  **参考**：
> [官网](http://requirejs.org)
> |
> [前端模块管理器简介](http://www.ruanyifeng.com/blog/2014/09/package-management.html)

#### sea.js
> SeaJS是一个遵循CommonJS规范的JavaScript模块加载框架，可以实现JavaScript的模块化开发及加载机制。
> 
> 遵循了[CMD](https://github.com/seajs/seajs/issues/242)(通用模块定义规范)，有延后执行、依赖就近等特点
> 
>  **参考**：
> [官网](http://seajs.org/)
> |
> [LABjs、RequireJS、SeaJS 哪个最好用？为什么？](http://www.zhihu.com/question/20342350)


#### angular.js
> Angular.js是一款开源的JavaScript框架，由Google维护，其目标是增强基于Web应用，并带有MVC功能，使得开发和测试变得更加容易。
>  
> Angular.js读取包含附加自定义（标签属性）的HTML，遵从这些自定义属性中的指令，并将页面中的输入输出与由JavaScript变量表示的模型绑定起来。这些JavaScript变量的值可以手工设置，或者从静态或动态JSON资源中获取。
> 
>  **参考**：
> [官网](https://angularjs.org/)

#### ember.js
> Ember.js同样是一个用于创建web应用的JavaScript MVC 框架，其采用基于字符串的Handlebars模板，支持双向绑定、观察者模式、计算属性（依赖其他属性动态变化）、自动更新模板、路由控制、状态机等。
>
> Ember.js使用自身扩展的类来创建Ember.js对象、数组、字符串、函数，提供大量方法与属性用于操作。每一个Ember.js应用都使用各自的命名空间，避免冲突。
> 
>  **参考**：
> [官网](http://emberjs.com/)
> |
> [Angular.js VS. Ember.js：谁将成为Web开发的新宠？](http://www.csdn.net/article/2013-09-09/2816880-Angular-Ember-Javascript-Frameworks)
> |
> [前端开发框架三剑客—AngularJS VS. Backone.js VS.Ember.js](http://www.csdn.net/article/2014-08-28/2821409-javascript-framework-comparison)


#### Qatrix.js
> 轻量级前端框架，类jQuery。

#### Zepto
> Zepto是一个轻量级的针对现代高级浏览器的JavaScript库， 它与jquery有着类似的api。 如果你会用jquery，那么你也会用zepto。
> 
> 设计的目的是提供jquery的类似的APIs，但并不是100%覆盖jquery为目的。zepto设计的目的是有一个5-10k的通用库、下载并执行快、有一个熟悉通用的API，所以你能把你主要的精力放到应用开发上。
>
> 可惜不支持IE10以下的IE浏览器

> 
>  **参考**：
> [官网](http://zeptojs.com/)
> |
> [Zepto 中文网](http://www.html-5.cn/Manual/Zepto/)

#### HandlebarsJS

#### MustacheJS

#### KISSY

#### YUI3

#### phantomjs

#### Backbone

#### KnockoutJS

