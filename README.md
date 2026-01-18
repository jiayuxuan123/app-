# ☁️ 个人私有图床仓库 (app-)
https://jiayuxuan123.rth1.xyz/yunluo.html
这是一个基于 **Cloudflare Workers** + **GitHub API** 构建的个人私有图床存储仓库。通过 jsDelivr CDN 提供全球加速访问。

## 🛠️ 架构说明
* **存储端**: GitHub Repository (`jiayuxuan123/app-`)
* **处理端**: Cloudflare Workers (负责 API 转发与鉴权)
* **加速端**: jsDelivr CDN (快速加载图片资源)

## 📂 目录结构
* `/images`: 存储所有上传的图片资源
* `.gitkeep`: 确保空文件夹不被 Git 忽略

## 🚀 使用指南

### 1. 图片上传
* 通过前端界面选择图片后，Worker 会调用 GitHub API 将图片推送到 `/images` 目录。
* 上传成功后，文件会自动重命名（时间戳+随机字符）以防止冲突。

### 2. 图片删除
* **手动删除**: 在手机浏览器开启“桌面版网站”模式，进入文件预览页点击“垃圾桶”图标并 Commit。
* **自动删除**: 修复 Worker 代码后，可在图床前端“上传历史”中一键删除。

## ⚠️ 注意事项
* **Token 安全**: 请务必妥善保管您的 GitHub Personal Access Token (classic)。
* **API 限制**: 确保 Token 拥有 `repo` 权限，否则会导致上传或删除操作失败。
* **大文件**: 建议上传压缩后的图片，以保证加载速度。

---
© 2026 jiayuxuan123. Built with ❤️.
