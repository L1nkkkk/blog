# blog

[Mosaic](https://github.com/L1nkkkk/mosaic) 博客模块的文章仓库。推送到 `main` 后，站点会在几分钟内自动同步。

## 写一篇文章

在 `posts/` 下新建一个 Markdown 文件，文件名决定地址：

```text
posts/2026-10-13-hello.md   →   /post/hello
```

文件开头可以写这些信息，都是可选的：

```markdown
---
title: 文章标题
date: 2026-10-13
tags: [随笔, 技术]
summary: 列表里显示的一句话摘要。
draft: true
---
```

- 没写 `title` 时用正文的第一个 `# 标题`，再没有就用文件名。
- 没写 `date` 时用文件名开头的日期。
- `draft: true` 的文章不会出现在站点上。注意这个仓库是公开的，草稿在 GitHub 上仍然可见。

## 图片和链接

- 图片放进仓库（比如 `posts/img/`），用相对路径引用：`![说明](img/photo.png)`。支持 PNG、JPG、GIF、WebP、AVIF，单张不超过 5 MB。外链图片不会显示，会变成一个链接。
- 链接到另一篇文章，直接写它的文件：`[上一篇](2026-10-01-other.md)`。

## 支持的 Markdown

标题、段落、粗体、斜体、删除线、行内代码、代码块、引用、有序和无序列表、任务列表、表格、分隔线、链接和图片。文章里的 HTML 标签会按原样显示成文字，不会生效。
