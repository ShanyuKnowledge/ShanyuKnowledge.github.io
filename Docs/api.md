---
layout: default
title: API 文档
description: 产品 API 接口说明
---

# API 文档

本文档介绍 Shanyu Knowledge 的 API 接口。

## 基础信息

- **API 版本**: v1
- **基础路径**: `/api/v1`
- **认证方式**: API Key

## 接口列表

### 获取文档列表

**请求**: `GET /api/v1/docs`

**参数**:
| 参数名 | 类型 | 必填 | 说明 |
|--------|------|------|------|
| page | int | 否 | 页码，默认 1 |
| limit | int | 否 | 每页数量，默认 10 |

**响应**:
```json
{
  "success": true,
  "data": [
    {
      "id": 1,
      "title": "快速入门",
      "slug": "quickstart",
      "created_at": "2024-01-15T10:00:00Z"
    }
  ],
  "pagination": {
    "page": 1,
    "total": 100
  }
}
```

### 获取文档详情

**请求**: `GET /api/v1/docs/{slug}`

**响应**:
```json
{
  "success": true,
  "data": {
    "id": 1,
    "title": "快速入门",
    "content": "# 快速入门...",
    "created_at": "2024-01-15T10:00:00Z",
    "updated_at": "2024-01-15T10:00:00Z"
  }
}
```

## 错误处理

| 错误码 | 说明 |
|--------|------|
| 400 | 请求参数错误 |
| 401 | 未授权访问 |
| 404 | 资源不存在 |
| 500 | 服务器内部错误 |