# 藏音网站

藏音的中文产品介绍、帮助与支持、隐私政策。纯静态 HTML 与 CSS，无 JavaScript、框架、构建步骤、外部字体或统计脚本。

## 文件

- `index.html` — 产品首页
- `support/index.html` — 帮助与支持
- `privacy/index.html` — 隐私政策
- `styles.css` — 三页共用样式
- `favicon.svg` — 本地站点图标
- `.nojekyll` — 直接提供静态文件

所有站内链接和资源使用相对路径，可在 GitHub Pages 的 `/cangyin/` 子路径下使用。外部链接仅在访客主动点击时打开。抽象专辑纸套由 CSS 绘制，不是 App 截图或真实专辑封面。

## 本地预览

在仓库目录运行：

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

访问 `http://127.0.0.1:8000/`，并检查 `/support/` 与 `/privacy/`。仅提供网站目录，不要公开包含 App 源码的父目录。

## GitHub Pages 发布

在本仓库的 Settings → Pages 中，Source 选择 Deploy from a branch，Branch 选择 `master`，目录选择 `/(root)`，点击 Save。首次发布完成前不要把预计地址当成已上线网站。发布后逐页检查主页、`support/` 和 `privacy/`。

## 检查清单

- 在 360px 手机宽度和桌面宽度检查布局，无横向溢出。
- 检查 200% 缩放、键盘 Tab 焦点、跳到正文链接与页脚导航。
- 检查三页标题、描述、图标和返回首页链接。
- 禁用网络后检查页面样式；首屏不请求第三方资源。
- 更新功能或数据处理方式时，同步复核支持页与隐私政策。
- 目前未提供 App Store 或 TestFlight 下载入口；正式可用并获准后再更新。

本仓库只包含公开网站资料，不包含 App 源码、私有规划、构建产物或发布凭据。
