---
title: npm快速上手
date: 2019-11-13
categories: web
tags:
    - web
    - npm
    - 前端
---

# npm简介

# npm常用命令
## 查看本地/远程包版本号
1. 查看远程包
   第一种方法： 
   ```js
   npm info <packageName>
   //详细列出包的说明，远程位置，依赖，维护人员，最新发布日期等信息。
   ```

   第二种方法： 
   ```js
   npm view <packageName> versions --json
   //只列出包历史所有版本信息
   ```

2. 查看本地包
   ```js
   npm ls <packageName>     //当前目录下的包
   npm ls <packageName> -g  //全局安装包
   ```

## 安装包
1. 全局安装
   ```js
    npm install <packageName> -g //全局安装
   ```
2. 本地（当前目录下）安装
   ```js
    npm install <packageName> //本地安装
   ```
3. 信息写入
   ```js
    npm install <packageName> --save
    npm install <packageName> --save-dev
    //安装的同时，将信息写入package.json中项目路径中
   ```
    --save 是你发布之后还依赖的东西
    --save-dev 是你开发时候依赖的东西

## 更新包
```js
npm update <packageName> //更新本地模块
npm update <packageName> -g //更新全局模块
```
