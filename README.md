# DevFest DevTools MCP Workshop 官网

这是一个为 Google DevFest Workshop 准备的静态官网，用来介绍 **Chrome DevTools MCP Server** 相关内容，以及讲师 Leon 的背景信息。

站点包含以下页面（都在 `devfest-website/` 目录下）：

- `index.html`：主页，活动信息、亮点、议程、技术栈总览
- `gdg-devfest.html`：GDG 与 DevFest 介绍
- `devtools-mcp.html`：Chrome DevTools MCP Server 技术说明
- `about-leon.html`：讲师个人介绍

## 本地预览

由于是纯静态页面，你可以用任意静态文件服务器或直接用浏览器打开文件进行预览。

### 方式一：直接用浏览器打开

1. 在文件管理器中打开项目目录。
2. 进入 `devfest-website/` 目录。
3. 双击 `index.html`（或右键用你喜欢的浏览器打开）。

> 注意：
> - 直接用 `file://` 方式打开时，大部分浏览器都可以正常展示本页面。
> - 如果你后续加入了跨页面的脚本或相对路径较复杂的资源，建议使用本地静态服务器方式。

### 方式二：使用简单的静态服务器

如果你已经安装了 Node.js，可以在项目根目录运行一个简单的 HTTP 静态服务器，例如使用 `npx serve`：

```bash
cd devfest-website
npx serve .
```

然后在浏览器中访问命令行输出的本地地址（例如 `http://localhost:3000`）。

## 部署

仓库中包含 GitHub Actions 工作流（`.github/workflows/deploy.yml`），当你将代码推送到 `main` 分支时，会自动将 `devfest-website/` 目录部署到 GitHub Pages。

你可以在 GitHub 仓库的 **Actions** 和 **Settings → Pages** 页面查看部署状态和访问 URL。
