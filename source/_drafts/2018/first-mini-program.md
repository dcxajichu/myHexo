---
title: '记一次小程序开发'
category: 技术
tags: [总结, 前端]
date: 2018-9-28
updated: 2018-9-28
---

第一次小程序开发。

<!-- more -->

# 统计

开始时间：2018.8.20
开发结束时间：2018.9.21
测试结束时间：2018.9.28
页面统计:32 个页面
组件统计:11 个组件
实际工作时间(包括加班):

# 背景

第一次做手机端 APP，第一次使用小程序开发，第一次使用数据驱动做公司项目（原来用的 jQuery 进行 dom 操作）。

# 需求

按照 APP（商城类）开发小程序

# 详细经历

## 第一周

1. 像素单位用 rpx,2rpx ＝ 1px.
2. flex 垂直布局 margin-right 失效.

## 第二周

1. 问题：Java 后端返回 id 为 lang 类型，前端获取会丢失精度。
2. 创建了控制器文件夹，用来放与后端交互的接口(也不知道也没用).
3. 用 promise 封装了常用的请求方法，做了统一错误处理，后台异常处理

## 第三周

1. 发现有很多表单页面相似，于是封装了一个表单页面组件，通过给组件传入页面元素配置和验证规则实现复用

# 需要改进的地方

## 关于错误处理

1. 后端返回错误码和提示信息统一处理（已有，通过弹窗形式提示错误信息），应该换种形式来区分前端写的提示信息。
2. 错误上报
