# 安装说明

本文档介绍如何安装和配置 Shanyu Knowledge。

## 环境要求

- Ruby 2.7+
- Jekyll 4.3+
- Git

## 安装步骤

### 1. 克隆仓库

```bash
git clone https://github.com/ShanyuKnowledge/ShanyuKnowledge.github.io.git
cd ShanyuKnowledge.github.io
```

### 2. 安装依赖

```bash
bundle install
```

### 3. 启动开发服务器

```bash
bundle exec jekyll serve
```

### 4. 访问网站

打开浏览器访问 `http://localhost:4000`

## 配置

编辑 `_config.yml` 文件进行自定义配置：

```yaml
title: 您的文档标题
description: 您的文档描述
url: https://yourdomain.com
```

## 构建生产版本

```bash
bundle exec jekyll build
```

构建结果将输出到 `_site` 目录。