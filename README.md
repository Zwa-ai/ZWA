# 张雯瑗 · 个人主页

数字媒体技术专业个人主页 —《布达佩斯大饭店》视觉 · 动效版。

- 单文件 HTML：CSS / JS / 图片全部内嵌，双击即可打开
- 外部依赖：动效库 CDN 双源（jsDelivr → cdnjs，失败自动原生降级）+ 字体 CDN
- 电话 / 邮箱为占位符（在 `index.html` 的 `SITE_CONFIG` 中更新后重建）

## 部署到 GitHub Pages

1. 新建公开仓库（网页操作）：
   - 个人主页模式：仓库名 `<用户名>.github.io` → 网址 `https://<用户名>.github.io/`
   - 或项目站点模式：仓库名如 `resume` → 网址 `https://<用户名>.github.io/resume/`
   - 不勾选 README / .gitignore（保持空仓）

2. 在本目录执行：
   ```bash
   git init
   git add index.html README.md
   git commit -m "init: 个人主页"
   git branch -M main
   git remote add origin https://github.com/<用户名>/<仓库名>.git
   git push -u origin main
   ```

3. 仓库 → Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)` → Save

4. 等待 1–2 分钟首次构建，访问上面对应网址验证。

> 前提：本机需先安装 Git（当前未安装）。
> 后续更新：替换本目录 `index.html` → `git add/commit/push` → Pages 自动更新。
