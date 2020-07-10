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

> https://github.com/vincenteliang/vue-sell-cube/commit/441a7f82b88ba7261388d7b73cd29bc608e26b1b#diff-0e893b3578ae3d5c8b98bac1c80756a7

vue.config.js

## 第3章 头部组件开发

> 包括 Header组件编写，axios 封装和数据交互、star 组件抽象封装和 HeaderDetail 组件的编写和交互。

### 3-1 目录结构 & header 组件

> https://github.com/vincenteliang/vue-sell-cube/commit/347bd6fd4c6306b2a05373774ce2ccbf12876343

### 3-2 axios 封装 & 数据获取

> https://github.com/vincenteliang/vue-sell-cube/commit/ee9fce141b8a15aaf0736f1ea27be4417d52ca59

[axios 官网](https://github.com/axios/axios)

`npm i axios --save`

### 3-3 header-detail & star 组件

> https://github.com/vincenteliang/vue-sell-cube/commit/3e4fee3bbd683cd161b1b8725f9d408992d6062c

### 3-4 header-detail 交互

> https://github.com/vincenteliang/vue-sell-cube/commit/3aec844e98084591a0cdb4231e4be5f2bd094939

全屏弹窗最好写在body下，避免fixed布局中transform的影响，利用cube-ui的create-api模块来实现

## 第4章 Tab 组件开发

> 包括 Tab 组件的基础实现、上下联动实现、组件更高维度的抽象和封装。

### 4-1 tab 组件基础实现

> https://github.com/vincenteliang/vue-sell-cube/commit/f44efa39050951107aa61a50379df948de378a8e

### 4-2 tab 组件上下联动

> https://github.com/vincenteliang/vue-sell-cube/commit/0d5a9265c19656cae9a64dce9bd91e0685c4170e

### 4-3 tab 组件抽象和封装

> https://github.com/vincenteliang/vue-sell-cube/commit/56b2017c99951d92c74bd5f0fb7b2560f8e1d021
