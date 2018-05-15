---
title: elementUI-基础使用
date: 2018-05-14 14:48:16
tags: 前端UI框架
---
## 一、基础使用---安装

### window安装

``` bash
$ npm install element-ui@x.x.x --save
```
<!-- more -->
### mac安装

``` bash
$ sudo npm install element-ui@x.x.x --save
```
注意: mac 安装的时候最好加上sudo 权限控制，亲身体验，没有sudo的时候有时候会出现异常，这个异常就不好说了，6的起毛

其他的先不说文档链接在此 [element UI](http://element.eleme.io/#/zh-CN/component/installation).



## 二、基础使用---各种常用的组件

### 布局

```html
<el-row>
  <el-col :span="24">内容</el-col>
</el-row>
<el-row>
  <el-col :span="12">内容</el-col>
  <el-col :span="12">内容</el-col>
</el-row>
```
#### 批注：其实布局没啥说的了，其他的看文档就可以了，只需要知道每个col占24个位置就可以了，其他的根据需要去设置所占的长度就可以了

### Container 布局容器

#### 布局所需条件

- el-header：顶栏容器。
- el-aside：侧边栏容器。
- el-main：主要区域容器。
- el-footer：底栏容器。

#### 举个简单常见的demo

```html
<el-container>
  <el-aside width="200px">Aside</el-aside>
  <el-container>
    <el-header>Header</el-header>
    <el-main>Main</el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</el-container>
```
#### 批注：这个没啥多说的

### 按钮

```html
<el-button type="text">文字按钮</el-button>
<el-button type="text" disabled>文字按钮</el-button>
<el-button type="primary"  disabled>主要按钮</el-button>
<el-button type="success"  disabled>成功按钮</el-button>
<el-button type="info"  disabled>信息按钮</el-button>
<el-button type="warning"  disabled>警告按钮</el-button>
<el-button type="danger"  disabled>危险按钮</el-button>
```

#### 批注：按钮这部分，主要三大类，普通按钮，文字按钮，仅用按钮(disabled)，按钮主要通过type属性设置



