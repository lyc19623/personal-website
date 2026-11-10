# 项目协作说明

- 文件统一使用 UTF-8 编码。
- 首页文案在 `content/_index.md`，页面模板在 `layouts/home.html`，样式在 `static/css/site.css`。
- 修改后运行 `hugo --minify` 检查构建。`public/` 和 `work/` 中的文件不提交。
- 推送 `main` 后，GitHub Actions 构建并发布到 GitHub Pages。
