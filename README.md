# iOS PWA 部署说明

这个文件夹只包含可以公开部署的前端文件：

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `icon.svg`
- `icon-180.png`
- `icon-192.png`
- `icon-512.png`
- `.nojekyll`

不要把项目根目录里的 `server.js`、`api/`、`node_modules/`、`.bat`、`.lnk`、`cloudflared.exe` 上传到公开仓库。

## 推荐部署到 Cloudflare Pages

1. 新建一个 GitHub 仓库。
2. 只上传 `deploy` 文件夹里的文件到仓库根目录。
3. 打开 Cloudflare Pages，连接这个 GitHub 仓库。
4. 构建命令留空。
5. 输出目录填 `/`。
6. 部署完成后，用 iPhone Safari 打开 `https://你的项目.pages.dev`。
7. Safari 分享按钮 -> 添加到主屏幕。

首次在 iPhone 打开后，需要在右上角 AI 设置里重新填写硅基流动 API Key。API Key 只保存在你的手机本地，不要写进代码或上传到 GitHub。
