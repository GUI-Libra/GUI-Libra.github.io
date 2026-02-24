# 部署到 GitHub Pages

## 1. 在 GitHub 上创建仓库

1. 打开：https://github.com/organizations/GUI-Libra/repositories/new
2. 填写：
   - **Repository name**: `GUI-Libra.github.io`（组织主站，将部署到 https://gui-libra.github.io）
   - **Description**: GUI-Libra Project Website（可选）
   - **Visibility**: **Private**
   - 不要勾选 "Add a README file"
3. 点击 **Create repository**

## 2. 推送代码

在终端执行（将 `YOUR_USERNAME` 替换为你的 GitHub 用户名）：

```bash
cd /Users/yangrui/Desktop/Cursor-agent/gui-libra-website

# 添加远程仓库
git remote add origin https://github.com/GUI-Libra/GUI-Libra.github.io.git

# 推送（首次推送）
git branch -M main
git push -u origin main
```

若使用 SSH：

```bash
git remote add origin git@github.com:GUI-Libra/GUI-Libra.github.io.git
git branch -M main
git push -u origin main
```

## 3. 启用 GitHub Pages

1. 打开：https://github.com/GUI-Libra/GUI-Libra.github.io/settings/pages
2. 在 **Source** 下选择 **Deploy from a branch**
3. **Branch** 选择 `main`，路径选 `/ (root)`
4. 点击 **Save**

等待几分钟后，网站将部署到：**https://gui-libra.github.io**

> 注意：私有仓库的 GitHub Pages 需要 GitHub Pro/Team/Enterprise 才能启用。若组织无此权限，可将仓库改为 Public 以使用免费 Pages。
