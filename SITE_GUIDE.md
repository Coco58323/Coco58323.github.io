# 个人网站维护指南

本网站基于 [AcademicPages](https://github.com/academicpages/academicpages.github.io) Jekyll 模板构建，托管在 GitHub Pages。

## 网站结构

```
coco-site/
├── _config.yml          # 站点配置（个人信息、SEO等）
├── _data/
│   └── navigation.yml   # 导航菜单配置
├── _pages/
│   ├── about.md         # 首页内容
│   ├── publications.md  # 论文列表页
│   └── year-archive.html # Blogs 页面
├── _publications/       # 论文 Markdown 文件
├── _posts/              # 博客文章（目前未使用）
├── _includes/           # 模板组件
│   └── archive-single.html # 列表项模板
├── images/              # 图片资源
│   └── profile.png      # 头像
└── spaces/              # 爬虫输出（通过 deploy.sh 同步）
```

## 常见维护操作

### 1. 更新个人信息

**修改 `_config.yml`：**

```yaml
author:
  name             : "你的名字"
  avatar           : "profile.png"
  bio              : "简短介绍"
  location         : "地点"
  employer         : "公司"
  email            : "邮箱"
```

### 2. 更新首页介绍

**修改 `_pages/about.md`：**

这是 Markdown 文件，直接编辑内容即可。支持：
- 标题、列表、链接
- HTML 标签（如需特殊格式）

### 3. 添加新论文

**在 `_publications/` 创建新文件，如 `venue2025-paper.md`：**

```markdown
---
title: "论文标题"
collection: publications
permalink: /publication/venue2025-paper
excerpt: '简短描述'
date: 2025-01-01
venue: 'VENUE'
citation: '<b>作者</b>, 其他作者. <b>VENUE 2025</b>'
---
```

### 4. 修改导航菜单

**编辑 `_data/navigation.yml`：**

```yaml
main:
  - title: "Publications"
    url: /publications/
  - title: "Blogs"
    url: /blogs/
  # 添加新菜单项
  - title: "新页面"
    url: /new-page/
```

### 5. 更新头像

将新头像命名为 `profile.png` 并替换 `images/profile.png`。

### 6. 更新爬虫内容

在 `/Users/kerry/work/crawler` 目录执行：

```bash
./deploy.sh "更新说明"
```

这会自动同步 `output/` 到网站的 `spaces/` 目录。

## 部署流程

修改后执行：

```bash
cd /Users/kerry/work/coco-site
git add -A
git commit -m "更新说明"
git push origin master
```

GitHub Pages 会在 1-2 分钟内自动重新构建。

## 本地预览（可选）

```bash
bundle install
bundle exec jekyll serve
# 访问 http://localhost:4000
```

## 文件修改对照表

| 需要更改的内容 | 修改的文件 |
|--------------|-----------|
| 个人信息（姓名、邮箱等） | `_config.yml` |
| 首页介绍 | `_pages/about.md` |
| 导航菜单 | `_data/navigation.yml` |
| 添加论文 | `_publications/` 新建 `.md` |
| 头像 | `images/profile.png` |
| Blogs 页面链接 | `_pages/year-archive.html` |
| 论文列表样式 | `_includes/archive-single.html` |

## 注意事项

1. **缓存问题**：修改后如果没有立即生效，尝试强制刷新（Cmd+Shift+R）
2. **Jekyll 语法**：页面头部的 `---` 之间是 YAML 格式的元数据
3. **路径问题**：链接使用相对路径 `/path/` 而非绝对路径
4. **图片**：放在 `images/` 目录，使用 `/images/filename.png` 引用

