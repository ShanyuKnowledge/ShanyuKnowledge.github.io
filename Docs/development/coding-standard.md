---
layout: default
title: 代码规范
description: 项目代码规范说明
---

# 代码规范

本文档描述 Shanyu Knowledge 项目的代码规范。

## Markdown 规范

### 标题

使用 `#` 表示标题，层级分明：

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
```

### 列表

- 使用 `-` 或 `*` 表示无序列表
- 使用数字 `.` 表示有序列表
- 列表项之间保持空行

### 代码块

使用三个反引号包裹代码，并指定语言：

```markdown
```ruby
def hello
  puts "Hello World"
end
```
```

### 链接

```markdown
[链接文字](URL "可选标题")
```

### 图片

```markdown
![替代文本](图片URL "可选标题")
```

## Git 规范

### 分支命名

- `feature/xxx` - 新功能开发
- `fix/xxx` - Bug 修复
- `docs/xxx` - 文档更新
- `refactor/xxx` - 代码重构

### Commit 消息

遵循 [Conventional Commits](https://www.conventionalcommits.org/) 规范：

```
<类型>(<范围>): <描述>

[可选的正文]

[可选的脚注]
```

**类型**:
- `feat`: 新功能
- `fix`: Bug 修复
- `docs`: 文档更新
- `style`: 代码格式
- `refactor`: 重构
- `test`: 测试
- `chore`: 构建/工具

**示例**:
```
feat(docs): 添加 API 文档

添加了用户认证相关的 API 接口文档
```

## 提交流程

1. 创建功能分支
2. 提交代码
3. 创建 Pull Request
4. 代码审查
5. 合并到主分支