# yyqy_daily_log — GitHub Pages 博客

这个文件包已配置给 yuuuuuhhha，最终网址为 https://yuuuuuhhha.github.io/ 。这是源码包，还未上传或上线。

## 第一次上线（无需本地安装软件）

1. 登录 GitHub，打开 https://github.com/new 。Owner 选择 yuuuuuhhha。
2. Repository name 填 yuuuuuhhha.github.io，选择 Public，勾选添加 README，再点 Create repository。如果已经存在同名仓库，请先检查其中内容，不要直接覆盖。
3. 解压文件包。打开仓库，点 Add file → Upload files。将解压后 blog 文件夹**里面的所有文件和文件夹**拖入页面，不要上传 zip，也不要把外层 blog 文件夹一起上传。现有 README 可以替换成包内版本。
4. 点 Commit changes。仓库根目录应该直接看到 _config.yml、index.html、_layouts、_posts 和 assets。
5. Settings → Pages → Source 选 Deploy from a branch；Branch 选 main，目录选 /(root)，点 Save。
6. 等待部署完成，Pages 页面会出现 Visit site。打开 https://yuuuuuhhha.github.io/ 。部署不是即时完成的，可以在 Actions 中查看状态。失败时把报错截图发来。

## 发布文章

在 GitHub 仓库点 Add file → Create new file。文件名填 `_posts/2026-10-07-my-note.md`，正文例如：

```markdown
---
title: "我的学习笔记"
date: 2026-10-07 12:00:00 +0800
categories: [数字IC]
description: "一句话摘要。"
---
这里开始写正文。

## 小标题

这是 **加粗** 的文字。
```

提交后自动更新。发布日期应为当前或过去的时间；未来日期的文章默认不会显示。分类可以自己起，例如 FPGA、数字IC、项目记录、随笔。有文章的分类会自动出现在分类页。

## 插入图片和代码

先把图片上传到 assets/images，再在文章里写：

`![图片说明](/assets/images/example.png)`

代码块前后各写一行三个反引号，第一行的反引号后写 verilog、python 或 c 等语言名称。

## 修改网站

- `_config.yml`：修改 title（网站名字）、description 和 author。
- `about.md`：修改个人介绍。
- `_posts`：存放文章，示例文章可修改或删除。
- `assets/style.css`：修改配色与布局。

没有后台编辑器，也没有评论服务；不需要这些服务的账号。文章由 GitHub Pages 的 Jekyll 构建成网页。完整构建与公开网址需要上传后验证。

官方发布设置说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
