# 🚀 快速启动指南

## ✅ 已完成

你的个人学术网站已经完全配置好了！以下是已完成的工作：

### 配置信息
- **名字**: Yuetong Meng
- **职位**: 3rd-year PhD Candidate in Finance
- **机构**: Indiana University, Kelley School of Business
- **邮箱**: ym12@iu.edu
- **GitHub**: https://github.com/Yuetong-Meng
- **位置**: Bloomington, Indiana

### 研究兴趣
- Social Media and Finance
- Financial Intermediaries
- Investment Behavior
- Financial News
- AI in Finance

### 已创建的页面
1. **首页** (about.md) - 你的个人简介和研究方向
2. **简历** (cv.md) - 教育背景、研究经历和技能
3. **发布** - 准备好展示论文和研究 (_publications 目录)
4. **讲座** - 准备好添加演讲和会议 (_talks 目录)

## 📋 部署到 GitHub Pages（5步）

### 第1步：在 GitHub 创建仓库
1. 访问 https://github.com/new
2. 仓库名称输入：`Yuetong-Meng.github.io` ⚠️ **名称必须完全相同**
3. 选择 "Public"
4. 点击 "Create repository"

### 第2步：配置 Git（如果未配置）
```bash
git config --global user.name "Yuetong Meng"
git config --global user.email "ym12@iu.edu"
```

### 第3步：添加 GitHub 远程
```bash
cd ~/Documents/mengyuetong-website
git remote remove origin 2>/dev/null || true
git remote add origin https://github.com/Yuetong-Meng/Yuetong-Meng.github.io.git
```

### 第4步：推送代码到 GitHub
```bash
git add .
git commit -m "Initial commit: Personal academic website"
git push -u origin main
```

### 第5步：启用 GitHub Pages
1. 打开 https://github.com/Yuetong-Meng/Yuetong-Meng.github.io
2. 点击 **Settings** → **Pages**
3. 确保 Source 设为 "Deploy from a branch"
4. Branch 选择 "main" / "/(root)"
5. 点击 Save

**等待 1-2 分钟... 然后你的网站就上线了！** 🎉

访问: https://Yuetong-Meng.github.io

## 🎨 自定义你的网站

### 添加你的照片
1. 找一张专业的照片（推荐 400x400px）
2. 保存为 PNG 或 JPG
3. 放在 `images/` 目录，命名为 `profile.png`
4. 提交并推送

### 添加发布的论文
在 `_publications/` 目录创建 YAML 文件，例如 `2024-01-01-paper-title.md`：
```yaml
---
title: "Your Paper Title"
collection: publications
permalink: /publication/2024-01-01-paper-title
excerpt: 'Brief description'
date: 2024-01-01
venue: 'Journal Name'
paperurl: 'https://example.com/paper.pdf'
---
```

### 添加博客文章
在 `_posts/` 目录创建文件，例如 `2024-02-03-my-thoughts.md`：
```yaml
---
title: 'Post Title'
date: 2024-02-03
permalink: /posts/2024/02/blog-post-1/
---

你的内容写在这里...
```

### 编辑导航菜单
编辑 `_data/navigation.yml` 来添加或移除菜单项。

## 📚 有用的资源

- **模板文档**: https://academicpages.github.io
- **Jekyll 文档**: https://jekyllrb.com
- **GitHub Pages**: https://pages.github.com
- **Markdown 语法**: https://www.markdownguide.org

## ❓ 常见问题

**Q: 推送后网站没有立即更新？**
A: GitHub 需要 1-2 分钟来构建和部署。检查 Settings → Pages → Deployments 看构建状态。

**Q: 如何本地预览网站？**
A: 需要安装 Jekyll：
```bash
cd ~/Documents/mengyuetong-website
bundle install
bundle exec jekyll serve
# 然后访问 http://localhost:4000
```

**Q: 如何更新已发布的内容？**
A: 编辑文件后：
```bash
git add .
git commit -m "Update: Your changes"
git push
```

**Q: 可以添加自己的域名吗？**
A: 可以！在 Settings → Pages → Custom domain 中添加。

## 🎯 下一步建议

1. ✅ 部署到 GitHub Pages
2. 📸 添加个人照片到 images/profile.png
3. 📄 添加你的 CV/简历 PDF 到 files/ 目录
4. 📚 添加已发表的论文到 _publications/
5. 📢 在社交媒体和邮件中分享你的网站链接

---

**有任何问题，随时提问！** 😊
