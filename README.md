###自己撸的个人博客系统，将其命名为《求開》.
1. 配置用于编译vue的webpack(vue支持less的配置还爬坑中。。。；其中单独提取出css的插件extract-text-webpack-plugin版本要大于2.0不然会报错)
2. 配置用于编译koa2的gulp（如要支持async/await需babel配置transform-runtime和stage-3）
3. 使用mysql数据库，使用的orm库为sequelize
4. 使用koa-router来控制路由访问。
5. 使用koa-jwt来签发token实现单点登陆.
6. 发送请求使用axios
7. 前端库使用elementUI和vue更配哦。
8. 使用vue-router来实现单页。
9. 使用koa-static来作为vue的静态服务器（好像跟vue-router有冲突，在爬坑中。。。）
10. 测试框架使用karma和mocha
11. 使用better-npm-run来使用yarn命令
12. 包管理是基于yarn(据说比npm好)
13. 然后就没有然后了  

###以后更加详细的教程会补上的。附上官方资料地址(大部分是中文的)
+ webpack2:https://webpack.js.org/guides/get-started/
+ gulp:http://www.gulpjs.com.cn/docs/getting-started/
+ sequelize:http://docs.sequelizejs.com/en/v3/docs/getting-started/
+ koa2:https://github.com/koajs/koa
+ koa2的中间件列表:https://github.com/koajs/koa/wiki
+ koa-router:https://github.com/alexmingoia/koa-router/tree/master/
+ koa-jwt:https://github.com/koajs/jwt
+ vue:http://cn.vuejs.org/v2/guide/
+ vue-router:https://router.vuejs.org/zh-cn/essentials/named-routes.html
+ elementUI:http://element.eleme.io/#/zh-CN/component/custom-theme
+ axios:https://github.com/mzabriskie/axios
+ better-npm-run:https://github.com/benoror/better-npm-run
+ md编辑器：https://github.com/NextStepWebs/simplemde-markdown-editor
+ yarn:https://yarnpkg.com/zh-Hans/


###第一天（2017-2-21）
* 今日完成：
	1. 配置开发目录环境（包括koa2和vue）。
	2. 数据库建表。

###第二天（2017-2-22）
* 今日完成：
	1. 实现单点登陆。
	2. header组件编写。
	3. vue-router引入及配置首页和跳转规则。

###第三天（2017-2-23）
* 今日完成：
    1. blog列表组件功能的编写。
    2. blog详情组件功能的编写。  
* 明日计划：
    1. 实现blog增删改查功能。
    2. 在写blog功能中加入md编辑器。
    3. 优化blog列表和详情的界面。

###第四天（2017-2-24）
* 今日完成：
	1. 引入vuex

###第五天（2017-2-26）
* 今日完成：
	1. 编写界面

###第六天（2017-2-27）
* 今日完成：
    1. 解决页面刷新服务器报错的问题。关键：koa-history-api
    2. 解决登录后跳转到list再刷新的问题。关键：this.$router.push()+this.$router.go(0);
