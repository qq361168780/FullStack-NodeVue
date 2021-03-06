### 前言

一直想做一个人的Vue项目，刚好前段时间看到锦囊团官网（移动端）的UI设计的挺不错，所以就用Node作为后端仿照做了一套。


### 技术栈

前端：html、css、less、ES6、webpack、vue-cli、vue2、vuex、vue-router、vue-resource

后端：Node、Mysql

Vue2：采用最新Vue2的语法:grin:

Vuex：实现不同组件之间的状态共享:v:

vue-router：单页应用路由管理必备:sunglasses:

axios：发起http请求:wink:

SASS(SCSS)：css预处理语言:muscle:

Express(上线版本是Koa2)：因为vue-cli是用的Express做服务器，所以开源的开发版本是Express，自己生产环境用的是Koa2。 :stuck_out_tongue_winking_eye:

Webpack：自动化构建工具，大部分配置vue-cli脚手架已经弄好了，很方便。:smirk:

ES6：采用ES6语法，这是趋势。:clap:

localStorage(HTML5)：本地存储，保存用户个性化设置。:blush:

CSS3：CSS3动画及样式。:+1:

Mysql:本地存储数据。:smirk:



### 项目运行方法

#### 注：前端使用ES6的很多新特性，所以NodeJs 必须是6.0稳定版本，我使用的版本是8.9.0

（1）git clone https://github.com/moveondo/FullStack-NodeVue.git

（2）npm install

（3）npm run dev

（4）安装mysql数据库，新建数据库tour，然后导入全部数据（此项目根目录下的tour.sql）

（5）浏览器访问：localhost:9999

（6）数据库tour_user表中的用户默认密码均为123456


### 说明

如果对您有帮助，您可以点右上角 "Star" 支持一下 谢谢！ ^_^

或者您可以 "follow" 一下，我会不断开源更多的有趣的项目

开发环境 WIN7、Chrome 61.0、nodejs 8.9.0、Mysql5.7.14

#### 注：此项目纯属个人爱好，代码测试及学习使用，不用做任何商业活动。


>  vue-cli 入门建议参考 [基于VUE2.5仿天猫移动端首页的SPA](https://github.com/moveondo/VUE-Taobao)

>  node爬虫建议参考 [node+ejs爬上海链家房屋价格(张江地区租房)信息,promise,eventproxy,express,koa框架使用](https://github.com/moveondo/nodeJs-Reptile)  

> node框架express，koa 建议参考[nodejs框架-Express,Koa](https://github.com/moveondo/NodeJsFrame)


> vue + element-ui 的后台管理系统 建议参考 [ vue + element-ui 的后台管理系统](https://github.com/moveondo/vue-ManageSystem)

> 如果你想学习socket 建议参考 [vue全家桶+node.js+socket打造的智能聊天及新闻社区](https://github.com/moveondo/CloudNews)



### 目标功能

- [x] 登录、注册、密码修改（100%）
- [x] 个人中心信息展示、资料修改（100%）
- [x] 头像上传（100%）
- [x] app首页（100%）
- [x] app列表页——全球优惠券（100%）
- [x] 展示国家与地区列表（100%）
- [x] 每个国家与地区对应的优惠券、新闻、banner轮播图（100%）
- [x] 领取优惠券（100%）
- [x] 优惠券详情（100%）
- [x] 使用优惠券（100%）
- [x] 发布优惠券文字（100%）
- [x] 星级评价组件（100%）

### 目录结构

<pre>
├── build			// webpack及Node相关配置
├── config			// 项目dev和prod环境的配置
├── dist			// 项目build打包之后的目录
├── node_modules		// npm包
├── index.html			// 项目入口文件
├── package.json		// 项目描述文件
├── peoject.gif			// 项目GIF图
├── php_test			// 用PHP代替Node实现首页数据接口示例
├── server			// 后端目录
│   ├── account				// 登录、注册、找回密码等控制器
│   ├── get-coupon			// 领取优惠券控制器
│   ├── global-coupon			// 首页控制器
│   ├── global-coupon-list		// 全球优惠券列表页控制器 
│   └── personal			// 个人中心控制器，包括资料修改、头像上传等
├── src					// 前端目录
│   ├── assets				// 图片资源
│   ├── components			// 项目所有组件，每个文件头部都有组件名称注释
│   ├── router				// Vue路由
│   ├── store				// Vuex状态管理
│   ├── App.vue				// 主页面 
│   └── main.js				// Webpack 预编译入口
├── static			// 前端公用静态文件目录
│   ├── css         
│   ├── images          
│   ├── js     
│   ├── less         
│   └── upload
├── .babelrc			// ES6等babel的一些配置
├── .editorconfig		// 编辑器的一些配置
├── .eslintignore		// 忽略语法检查的目录文件，一般是忽略build和config目录
├── .eslintrc.js		// eslint的配置文件
├── // 关于项目目录各文件作用更加详细的介绍，请参考：
https://github.com/moveondo/FullStack-NodeVue/blob/master/knowledge/  
vue-cli%E8%84%9A%E6%89%8B%E6%9E%B6%E4%B9%8B%E5%90%8E%E7%9A%84%E7%9B%AE%E5%BD%95%E6%96%87%E4%BB%B6%E8%A7%A3%E6%9E%90.md
</pre>


#### 注：此项目纯属个人爱好及代码测试，如果需要完整的相关服务，可以去锦囊团官网。

### 项目GIF图

![gif](https://github.com/moveondo/FullStack-NodeVue/blob/master/static/images/project.gif)

### 写在最后

整个项目包括后台数据添加和前台数据展示两大部分,通过这个项目，梳理了一遍Vue的开发流程，并复习了相关使用方法，懂得了如何使用其他编程语言替换Node作为接口，还有就是之前写的一些例如iframefileupload.js前端页面无刷新文件上传插件、validatefileupload.js文件格式校验插件等都用上了。接下来就是不断的调整小细节，继续提升项目代码的性能和运行效率。



 
