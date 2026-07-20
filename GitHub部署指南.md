# GitHub Pages 部署指南

## 📋 准备工作

现在您的文件夹中包含：
- `index.html` - 网站主页面
- `README.md` - 项目说明
- `.gitignore` - Git忽略文件配置
- 导师照片文件（3张）
- 基本信息.txt

## 🚀 方式一：通过GitHub网站上传（推荐）

### 步骤1：创建GitHub账号
1. 访问 [https://github.com](https://github.com)
2. 如果没有账号，点击"Sign up"注册
3. 如果有账号，点击"Sign in"登录

### 步骤2：创建新仓库
1. 登录后，点击右上角的 "+" 号
2. 选择 "New repository"
3. 填写仓库信息：
   - **Repository name**: `space-exploration-lab`（或您喜欢的名字，建议用英文）
   - **Description**: `数智技术中心招生介绍网页`
   - **Public** ✅ (必须是公开的才能使用GitHub Pages)
   - **Add a README file** ❌ (不勾选，我们已经有了)
4. 点击 "Create repository"

### 步骤3：上传文件
1. 在新创建的仓库页面，点击 "uploading an existing file"
2. 将以下文件拖拽到页面中：
   - `index.html`
   - `README.md`
   - `.gitignore`
   - 所有导师照片（3张.jpg文件）
   - `基本信息.txt`
3. 在页面底部填写提交信息：
   - **Commit changes** 标题：`初始提交：添加招生介绍网页`
   - **Extended description**：`包含完整的招生介绍页面和相关资源文件`
4. 点击 "Commit changes"

### 步骤4：启用GitHub Pages
1. 在仓库页面，点击 "Settings" 标签
2. 在左侧菜单找到 "Pages"
3. 在 "Source" 部分：
   - 选择 "Deploy from a branch"
   - Branch: 选择 "main" (或 "master")
   - Folder: 选择 "/ (root)"
4. 点击 "Save"

### 步骤5：获取网站地址
1. 等待几分钟（通常1-5分钟）
2. 刷新页面，会看到绿色提示框显示：
   ```
   Your site is published at https://[你的用户名].github.io/space-exploration-lab/
   ```
3. 点击链接即可访问您的网站！

## 🔧 方式二：使用Git命令行（需要先安装Git）

### 安装Git
1. 下载Git：[https://git-scm.com/download/win](https://git-scm.com/download/win)
2. 安装后重启命令行

### Git命令操作
```bash
# 初始化仓库
git init

# 添加所有文件
git add .

# 提交文件
git commit -m "初始提交：添加招生介绍网页"

# 添加远程仓库（替换为您的仓库地址）
git remote add origin https://github.com/[你的用户名]/space-exploration-lab.git

# 推送到GitHub
git push -u origin main
```

## 🎯 重要提示

1. **仓库名影响网址**：
   - 仓库名：`space-exploration-lab`
   - 网址：`https://[用户名].github.io/space-exploration-lab/`

2. **特殊仓库名**：
   - 如果仓库名为：`[你的用户名].github.io`
   - 则网址为：`https://[用户名].github.io/`

3. **文件大小限制**：
   - 单个文件不超过100MB
   - 仓库总大小建议不超过1GB

4. **更新网站**：
   - 直接在GitHub上编辑文件
   - 或重新上传文件
   - 更改会在几分钟内生效

## ✅ 成功验证

网站部署成功后，您应该能看到：
- 美观的响应式招生介绍页面
- 所有导师照片正确显示
- 在手机和电脑上都能正常访问

## 🆘 常见问题

**Q: 网站显示404错误？**
A: 检查文件名是否为`index.html`，确保仓库是公开的

**Q: 图片不显示？**
A: 图片已经以base64格式嵌入HTML中，应该会正常显示

**Q: 多久能访问到网站？**
A: 通常1-5分钟，首次部署可能需要10分钟

**Q: 网站地址是什么？**
A: `https://[你的GitHub用户名].github.io/[仓库名]/` 