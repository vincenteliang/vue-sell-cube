<!-- # vue-sell-cube

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/). -->

# Vue.js2.5+cube-ui重构饿了么App

> https://coding.imooc.com/class/74.html

## 第1章 课程导学

> 包括课程概述、核心模块、核心技术、课程安排、课程收获、讲授方式、学习前提等方面的介绍，最后演示了整个外卖App的功能，让同学们对课程项目有一个直观的了解。...

### 1-1 导学

- 课程安排
  - 第1章准备工作
  - 第2-6章实战开发
  - 第7章create一api原理介绍
  - 第8章项目打包和部署
- 讲授方式
  - 按照App的功能依次开发页面组件
  - 先谈思路，再聊实现
  - 手写每一行JS代码，弱化CSS部分
- 课程收获
  - 学会使用Vue.js开发WebApp应用
  - 学会组件化、模块化的方式
  - 学会使用第三方组件库辅助我们的开发
  - 学会项目的部署构建过程
- 学习前提
  - 掌握前端基础知识如HTML、CSS、JS等
  - 有一定的Vue.js基础
  - 有ES6的基础

## 第2章 项目准备工作

> 包括项目需求分析、Vue-cli 3.0 脚手架介绍、cube-ui 介绍、目录模块分析、api 接口 mock 等。

### 2-1 Vue-cli 3.0 介绍

[vue-cli 官网](https://cli.vuejs.org/zh/)

`vue create vue-sell-cube`

    Manually
    CSS Pre- 
    stylus
    ESlint standard config

### 2-2 目录介绍 & cube-ui 安装

`vue add cube-ui`

- post-compile **Yes**
- Import **Partly**
- Custom **Yes**
- rem **No**
- vw **NO**

### 2-3 api 接口 mock

在vue.config.js