---
title: 前端作品集网站搭建
link: astro-portfolio
catalog: true
date: 2026-09-02 00:00:00
tags:
  - Astro
  - 作品集
  - 部署
categories:
  - 项目
cover: /img/cover/3.webp
description: 使用 Astro + astro-koharu 主题搭建个人作品集，并部署到 GitHub Pages 的完整实践。
---

## 背景

秋招求职需要一个在线作品集，参考了开源博客主题 astro-koharu 的设计与结构，搭建了本站。

## 技术选型

| 模块 | 方案 | 选型理由 |
| ---- | ---- | -------- |
| 框架 | Astro | 静态输出、加载轻快，内容型站点首选 |
| 主题 | astro-koharu | 支持多分类 / 多标签 / 全站搜索，开箱即用 |
| 搜索 | pagefind | 无后端全站搜索 |
| 部署 | GitHub Pages | 免费托管，配合 GitHub Actions 自动发布 |

## 关键实现

1. 克隆主题模板，修改 `config/site.yaml` 完成站点信息与分类配置
2. 内容以 Markdown 编写，frontmatter 控制分类、标签、封面与置顶
3. 增加「项目」分类作为作品集核心展示区
4. 通过 GitHub Actions 实现 push 后自动构建部署

## 成果

- 网站地址：https://1011-wyl.github.io
- 源码仓库：https://github.com/1011-wyl/1011-wyl.github.io
