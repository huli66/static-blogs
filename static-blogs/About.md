# About

## 过往

2018 年最开始用 Hexo 搭建<br />2021 年采用 React + Next.js 搭建的服务端渲染博客，所有项目和文档在同一个项目

## 项目结构和技术栈

由 前端 + 服务端 + 文档 三个项目组成

- 文档项目 - 所有 markdown 文档发布到一个 git 仓库中
  - 设置 GitHub Action 每次推送代码后进入云服务器执行拉代码脚本（或者直接打包复制到指定目录）
  - 该目录映射后端读取文档的目录
- 服务端：TypeScript + Express
  - 通过 Docker node 容器在云服务器运行
  - 读取指定目录所有文件，返回内容
- 前端：React
  - 通过 Docker nginx 容器部署到云服务器
  - About 页面
  - BlogList 页面
  - Blog 详情页面
- 其他
  - 个人组件库
  - 个人工具库

## 个人简介
