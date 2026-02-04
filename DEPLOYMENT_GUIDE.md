# GitHub Pages 部署指南

## 你的网站项目已准备好！

已完成的配置：
- ✅ 项目已克隆到 `~/Documents/mengyuetong-website`
- ✅ 配置文件 (_config.yml) 已更新
  - 网站标题：Yuetong Meng
  - GitHub 用户名：Yuetong-Meng
  - 个人邮箱：ym12@iu.edu
  - 机构：Indiana University
  - 位置：Bloomington, Indiana
- ✅ 关于页面 (about.md) 已创建
- ✅ 简历页面 (cv.md) 已创建

## 后续步骤：部署到 GitHub Pages

### 1. 创建 GitHub 仓库

打开 https://github.com/new，创建一个新的公开仓库，**必须** 命名为：
```
Yuetong-Meng.github.io
```

这个名称很重要，因为 GitHub 会自动识别它并启用 Pages 功能。

### 2. 配置本地 Git（第一次配置）

```bash
cd ~/Documents/mengyuetong-website
git config --global user.name "Yuetong Meng"
git config --global user.email "ym12@iu.edu"
```

### 3. 设置远程仓库

```bash
cd ~/Documents/mengyuetong-website
# 删除原来的远程（如果存在）
git remote remove origin

# 添加你的新仓库
git remote add origin https://github.com/Yuetong-Meng/Yuetong-Meng.github.io.git

# 验证设置
git remote -v
```

### 4. 提交并推送代码

```bash
cd ~/Documents/mengyuetong-website

# 提交所有更改
git add .
git commit -m "Initial commit: Personal academic website"

# 推送到 GitHub
git push -u origin main
```

### 5. 启用 GitHub Pages

1. 打开 https://github.com/Yuetong-Meng/Yuetong-Meng.github.io
2. 点击 **Settings**
3. 在左侧菜单找 **Pages**
4. 在 "Build and deployment" 下：
   - **Source**: 选择 "Deploy from a branch"
   - **Branch**: 选择 "main" 和 "/ (root)"
5. 点击 **Save**

### 6. 验证部署

大约 1-2 分钟后，你的网站将发布在：
```
https://Yuetong-Meng.github.io
```

## 检查部署状态

1. 在 GitHub 仓库页面点击 **Settings** → **Pages**
2. 查看 "Deployment history" 部分
3. 如果看到绿色的勾号，说明部署成功

## 常见问题

**Q: 网站显示 404？**
A: 确保：
- 仓库名称完全正确：Yuetong-Meng.github.io
- Pages 已在 Settings 中启用
- main 分支中有 _config.yml 文件
- 等待 2-3 分钟让 GitHub 构建完成

**Q: 如何更新网站内容？**
A: 只需修改文件并推送到 GitHub：
```bash
git add .
git commit -m "Update: Your changes description"
git push
```
GitHub 会自动重新构建和发布。

**Q: 如何自定义域名？**
A: 在 Settings → Pages → Custom domain 中添加你的域名。

## 下一步：添加你的研究内容

1. **添加论文**: 在 `_publications/` 目录添加 YAML 文件
2. **添加博客**: 在 `_posts/` 目录添加博文
3. **添加讲座**: 在 `_talks/` 目录添加演讲信息
4. **上传 PDF**: 将简历、论文等放在 `files/` 目录

## 需要帮助？

- 查看原模板文档：https://academicpages.github.io
- GitHub Pages 文档：https://pages.github.com
- 有问题可以查看 GitHub 仓库的 Issues
