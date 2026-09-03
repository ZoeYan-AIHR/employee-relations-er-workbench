# GitHub 上传与发布步骤

> 本仓库为静态单文件项目。`index.html` 可以直接发布至 GitHub Pages。

## 方式一：GitHub 网页上传（无需命令行）

1. 登录 GitHub，点击右上角 **+ → New repository**；
2. 仓库名称建议填写：`employee-relations-er-workbench`；
3. 如项目包含任何真实员工信息，请选择 **Private**；
4. 创建仓库时，不要勾选 *Add a README file*、*.gitignore* 或 *license*，避免与本地文件冲突；
5. 创建完成后，点击 **Add file → Upload files**；
6. 将当前目录下的 `index.html`、`README.md`、`.gitignore`、`.nojekyll` 拖入上传区域；
7. 点击 **Commit changes**；
8. 进入 **Settings → Pages**，按 README 的 GitHub Pages 章节发布即可。

## 方式二：Git 命令行上传

在当前目录执行：

```bash
git init
git add .
git commit -m "feat: add employee relations ER workbench"
git branch -M main
git remote add origin https://github.com/<你的GitHub用户名>/employee-relations-er-workbench.git
git push -u origin main
```

首次推送时，请在 GitHub Desktop、浏览器授权窗口或 Git Credential Manager 中完成认证。

**请勿将 Personal Access Token、密码或其他敏感凭证粘贴到聊天、README 或项目代码中。**
