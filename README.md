# 我的博客

这是一个使用 Hugo 构建的个人博客，采用简洁美观的自定义主题。

## 功能特性

- 🎨 **简洁美观的设计** - 现代化、响应式布局
- 📱 **移动端友好** - 完美适配各种设备
- 🏷️ **标签系统** - 方便内容分类和查找
- 📝 **Markdown 支持** - 使用 Markdown 编写文章
- ⚡ **快速加载** - 静态网站，加载速度快
- 🔍 **SEO 优化** - 搜索引擎友好

## 快速开始

### 本地开发

```bash
# 启动开发服务器
hugo server --buildDrafts

# 访问 http://localhost:1313/MyBlog/
```

### 创建新文章

```bash
# 创建新文章
hugo new posts/文章标题.md

# 编辑文章内容
# 在 content/posts/ 目录下找到新创建的文件
```

### 构建网站

```bash
# 构建静态文件
hugo

# 文件将生成在 public/ 目录
```

## 目录结构

```
my-blog/
├── content/           # 内容文件
│   ├── posts/        # 博客文章
│   └── _index.md     # 首页内容
├── themes/           # 主题文件
│   └── simple-blog/  # 自定义主题
├── static/           # 静态资源
├── layouts/          # 布局模板
├── hugo.toml         # 配置文件
└── public/           # 构建输出目录
```

## 配置说明

主要配置在 `hugo.toml` 文件中：

- `baseURL`: 网站的基础URL
- `title`: 网站标题
- `theme`: 使用的主题
- `params`: 主题参数配置

## 自定义主题

主题位于 `themes/simple-blog/` 目录：

- `layouts/`: HTML 模板文件
- `static/css/`: 样式文件
- `static/js/`: JavaScript 文件

## 部署

### GitHub Pages

1. 将代码推送到 GitHub 仓库
2. 启用 GitHub Pages
3. 设置构建源为 GitHub Actions
4. 配置自动部署

### 其他平台

由于生成的是静态文件，可以部署到任何支持静态网站的托管平台：
- Netlify
- Vercel
- Cloudflare Pages
- 阿里云 OSS
- 腾讯云 COS

## 许可证

MIT License

## 联系方式

如有问题或建议，欢迎通过以下方式联系：

- 📧 邮箱：your-email@example.com
- 🐙 GitHub：your-github-username
