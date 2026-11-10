# lyc19623 的个人网站

使用 Hugo 生成静态网页，推送 `main` 后由 GitHub Actions 发布到 GitHub Pages。

## 本地编辑

使用 [Hugo v0.169.0](https://github.com/gohugoio/hugo/releases/tag/v0.169.0)。修改 `content/_index.md` 可以更新首页文案。

```powershell
hugo server
```

打开 [本地预览](http://localhost:1313/personal-website/)。如果在本项目的 `work/hugo/` 中使用免安装版，在 PowerShell 中运行 `./work/hugo/hugo.exe server`。

## 构建与发布

```powershell
hugo --minify
git add .
git commit -m "Update website"
git push
```

构建结果位于 `public/`。首次发布时，在 GitHub 仓库的 Settings → Pages 中将 Source 设为 **GitHub Actions**，然后从 Actions 手动运行 **Deploy to GitHub Pages**，或推送一次更新。
