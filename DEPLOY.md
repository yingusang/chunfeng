# 🚀 部署指南 - GitHub Pages

## 步骤 1: 准备 GitHub 仓库

### 1.1 创建 GitHub 账号
如果还没有 GitHub 账号，访问 https://github.com 注册一个。

### 1.2 创建新仓库
1. 登录 GitHub
2. 点击右上角的 "+" 按钮，选择 "New repository"
3. 填写仓库信息：
   - Repository name: `chunfeng` (仓库名称)
   - Description: `春风 - 六爻占卜应用`
   - 选择 `Public` (公开)
   - **不要**勾选 "Add a README file"
4. 点击 "Create repository"

## 步骤 2: 上传代码到 GitHub

在终端中执行以下命令：

```bash
# 进入项目目录
cd /Users/tom/Downloads/pythontest0122/test_project

# 初始化 Git 仓库
git init

# 添加所有文件
git add index.html README.md .gitignore

# 提交
git commit -m "Initial commit: 春风占卜应用"

# 添加远程仓库（替换 YOUR_USERNAME 为你的 GitHub 用户名）
git remote add origin https://github.com/YOUR_USERNAME/chunfeng.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

## 步骤 3: 启用 GitHub Pages

1. 在 GitHub 仓库页面，点击 "Settings"（设置）
2. 在左侧菜单找到 "Pages"
3. 在 "Source" 部分：
   - Branch: 选择 `main`
   - Folder: 选择 `/ (root)`
4. 点击 "Save"
5. 等待几分钟，页面会显示你的网站地址：
   ```
   https://YOUR_USERNAME.github.io/chunfeng/
   ```

## 步骤 4: 访问你的网站

几分钟后，访问：
```
https://YOUR_USERNAME.github.io/chunfeng/
```

你的"春风"占卜应用就上线了！🎉

## 更新网站

当你修改了代码，想要更新网站时：

```bash
cd /Users/tom/Downloads/pythontest0122/test_project

# 添加修改的文件
git add .

# 提交
git commit -m "更新说明"

# 推送
git push
```

几分钟后，网站会自动更新。

## 自定义域名（可选）

如果你有自己的域名：

1. 在 GitHub Pages 设置页面的 "Custom domain" 填入你的域名
2. 在你的域名服务商那里添加 CNAME 记录指向：
   ```
   YOUR_USERNAME.github.io
   ```

## 注意事项

- ✅ 完全免费
- ✅ 自动 HTTPS
- ✅ 全球 CDN 加速
- ⚠️ 仓库必须是 Public（公开）
- ⚠️ 有一定的流量限制（但对个人使用完全够用）

## 需要帮助？

- GitHub Pages 文档: https://docs.github.com/pages
- 如果遇到问题，可以查看仓库的 Actions 标签页查看部署状态
