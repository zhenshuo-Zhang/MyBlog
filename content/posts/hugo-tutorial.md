---
title: "Hugo 博客搭建指南"
date: 2024-01-16T14:30:00+08:00
draft: false
author: "博主"
tags: ["Hugo", "教程", "静态网站", "博客"]
---

# Hugo 博客搭建完整指南

Hugo 是一个快速、现代的静态网站生成器，非常适合搭建个人博客。本文将详细介绍如何使用 Hugo 搭建一个美观的博客。

## 为什么选择 Hugo？

- ⚡ **极快的构建速度** - 构建大型网站只需几秒钟
- 🎨 **丰富的主题生态** - 数千个免费主题可供选择
- 📝 **Markdown 支持** - 使用 Markdown 编写内容
- 🔧 **高度可定制** - 灵活的模板系统
- 🚀 **部署简单** - 生成静态文件，易于部署

## 安装 Hugo

### macOS
```bash
brew install hugo
```

### Windows
```bash
choco install hugo
```

### Linux
```bash
sudo apt-get install hugo
```

## 创建新站点

```bash
# 创建新的 Hugo 站点
hugo new site my-blog

# 进入目录
cd my-blog

# 初始化 Git 仓库
git init
```

## 选择主题

Hugo 有丰富的主题选择，推荐几个优秀的主题：

1. **PaperMod** - 现代化、功能丰富
2. **LoveIt** - 简洁美观
3. **Stack** - 响应式设计
4. **Ananke** - 简单易用

## 配置站点

编辑 `hugo.toml` 文件：

```toml
baseURL = "https://your-domain.com"
languageCode = "zh-cn"
title = "我的博客"
theme = "your-theme"

[params]
description = "我的个人博客"
author = "你的名字"
```

## 创建内容

```bash
# 创建新文章
hugo new posts/my-first-post.md
```

编辑文章内容：

```markdown
---
title: "我的第一篇文章"
date: 2024-01-15T10:00:00+08:00
draft: false
tags: ["Hugo", "博客"]
---

# 欢迎来到我的博客！

这是我的第一篇文章...
```

## 本地预览

```bash
# 启动开发服务器
hugo server -D

# 访问 http://localhost:1313
```

## 构建和部署

```bash
# 构建静态文件
hugo

# 文件将生成在 public/ 目录
```

## 部署到 GitHub Pages

1. 将代码推送到 GitHub 仓库
2. 启用 GitHub Pages
3. 设置构建源为 GitHub Actions
4. 配置自动部署

## 总结

Hugo 是一个优秀的静态网站生成器，具有以下优势：

- 构建速度快
- 主题丰富
- 配置简单
- 部署方便

希望这个指南能帮助您快速搭建自己的博客！
