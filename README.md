# 简易Jekyll网站

这是一个简单的Jekyll网站模板，专为GitHub Pages设计。

## 什么是Jekyll？

Jekyll是一个静态网站生成器，它可以将纯文本转换成静态网站和博客。GitHub Pages直接支持Jekyll，这使得您可以轻松地发布网站。

## 目录结构说明

```
jekyll_try/
├── _config.yml           # Jekyll配置文件
├── _layouts/             # 存放布局模板的文件夹
│   ├── default.html      # 默认布局模板
│   └── post.html         # 文章布局模板
├── _posts/               # 存放博客文章的文件夹
│   └── 2025-03-01-welcome-to-jekyll.md  # 示例文章
├── _site/                # Jekyll生成的静态网站文件(自动生成，不需上传)
├── assets/               # 存放资源文件的文件夹
│   ├── css/              # CSS文件夹
│   │   └── style.css     # 样式文件
│   └── images/           # 图片文件夹
├── index.md              # 网站首页
└── about.md              # 关于页面
```

## 如何使用

1. **本地预览网站**（可选，需要安装Jekyll）：
   - 安装Ruby和Jekyll
   - 在项目根目录运行`bundle exec jekyll serve`
   - 在浏览器中访问`http://localhost:4000`

2. **上传到GitHub Pages**：
   - 将整个文件夹上传到您的GitHub仓库
   - 在仓库设置中启用GitHub Pages
   - 选择`main`分支作为源

## 如何添加新文章

在`_posts`文件夹中创建新的Markdown文件，文件名格式为：`YYYY-MM-DD-标题.md`。

文件开头需要添加YAML前置信息：

```yaml
---
layout: post
title: "文章标题"
date: YYYY-MM-DD HH:MM:SS +0800
categories: 分类名称
---
```

之后，您可以使用Markdown语法编写文章内容。

## 如何修改网站样式

修改`assets/css/style.css`文件来自定义网站的外观。

## 如何修改网站配置

编辑`_config.yml`文件可以修改网站的标题、描述、主题等设置。
