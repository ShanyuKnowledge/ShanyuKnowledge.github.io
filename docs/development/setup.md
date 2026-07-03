# 开发环境搭建

本文档介绍如何搭建 Shanyu Knowledge 的本地开发环境。

## 环境要求

- Python 3.x（用于启动本地 HTTP 服务器）
- Node.js（可选，使用 docsify-cli）

## 安装步骤

### 方式一：使用 Python（推荐）

```bash
# 启动本地服务器
python -m http.server 3000
```

访问 `http://localhost:3000` 查看效果。

### 方式二：使用 docsify-cli

```bash
# 安装 docsify-cli
npm install -g docsify-cli

# 启动本地服务器
docsify serve
```

访问 `http://localhost:3000` 查看效果。

## 开发命令

| 命令 | 说明 |
|------|------|
| `python -m http.server 3000` | 使用 Python 启动开发服务器 |
| `docsify serve` | 使用 docsify-cli 启动开发服务器 |

## 目录结构

```
├── index.html         # Docsify 入口文件
├── _sidebar.md        # 侧边栏导航配置
├── README.md          # 首页内容
└── Docs/              # 文档目录
    ├── LGT-Nano系列/  # 产品文档
    └── development/   # 开发文档
```