---
title: 示例文章 - 如何使用share功能
date: 2024-01-05
tags:
  - 示例
  - 教程
categories:
  - 文档
share: true
draft: false
description: 这是一篇示例文章，展示如何使用share功能将Obsidian笔记同步到Hugo博客
---

# 示例文章

这是一篇示例文章，用于演示如何将Obsidian笔记同步到Hugo博客。

## 使用方法

### 1. 设置frontmatter

在你的markdown文件顶部添加YAML格式的frontmatter：

```yaml
---
title: 你的文章标题
date: 2024-01-05
tags:
  - 标签1
  - 标签2
share: true
---
```

### 2. 关键字段说明

- `title`: 文章标题（必需）
- `date`: 发布日期（可选，默认使用当前日期）
- `tags`: 文章标签（可选）
- `categories`: 文章分类（可选）
- **`share: true`**: 设置为true以同步到博客（必需）
- `draft`: 是否为草稿（可选，默认false）

### 3. 文章内容

在frontmatter之后编写你的文章内容，支持所有markdown语法。

## 同步流程

1. 在Obsidian中编辑笔记
2. 设置 `share: true`
3. 保存并提交到GitHub
4. 自动触发同步工作流
5. 文章出现在博客仓库的 `content/posts/` 目录

## 注意事项

- 只有设置了 `share: true` 的文章才会被同步
- 目录结构会被保持
- 图片等资源需要使用在线链接或单独处理
- 修改文章后重新推送会自动更新

## 高级用法

### 控制同步的文章

如果你不想同步某篇文章，只需：
- 设置 `share: false`
- 或者完全不添加 `share` 字段

### 批量同步

可以在博客仓库手动触发工作流，选择"强制同步所有文章"来重新同步所有标记为share的文章。
