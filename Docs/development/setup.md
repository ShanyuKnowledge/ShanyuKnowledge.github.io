---
layout: default
title: 开发环境搭建
description: 如何搭建本地开发环境
---

# 开发环境搭建

本文档介绍如何搭建 Shanyu Knowledge 的本地开发环境。

## 环境要求

- Ruby 2.7+
- Bundler
- Node.js (可选，用于前端开发)

## 安装步骤

### 1. 安装 Ruby

#### macOS

```bash
# 使用 Homebrew 安装
brew install ruby
```

#### Ubuntu/Debian

```bash
sudo apt-get update
sudo apt-get install ruby-full
```

### 2. 安装 Bundler

```bash
gem install bundler
```

### 3. 克隆仓库

```bash
git clone https://github.com/ShanyuKnowledge/Shanyuknowledge.github.io.git
cd Shanyuknowledge.github.io
```

### 4. 安装依赖

```bash
bundle install
```

### 5. 启动开发服务器

```bash
bundle exec jekyll serve --livereload
```

访问 `http://localhost:4000` 查看效果。

## 开发命令

| 命令 | 说明 |
|------|------|
| `bundle exec jekyll serve` | 启动开发服务器 |
| `bundle exec jekyll build` | 构建生产版本 |
| `bundle exec jekyll clean` | 清理构建产物 |

## 目录结构

```
├── _config.yml        # 站点配置
├── _docs/             # 文档内容
├── _layouts/          # 布局模板
├── _data/             # 数据文件
├── assets/            # 静态资源
└── index.md           # 首页
```