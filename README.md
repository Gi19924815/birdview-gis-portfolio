# 鸟瞰地图的图形基地 · 个人网站

赛博朋克风格个人网站，用于**作品展示 / 教程 / 插件展示·发布·出售**。
纯静态站点（HTML + CSS + JS），无构建步骤，直接部署。

## 线上地址
- 🌐 生产站点：https://personal-site-chi-nine-18.vercel.app
- 🐙 GitHub 仓库：https://github.com/Gi19924815/birdview-gis-portfolio
- 🔧 Vercel 后台：https://vercel.com/gi19924815s-projects/personal-site

> 已连接 GitHub，以后每次 `git push` 到 main 分支都会**自动重新部署**，无需手动操作。

## 文件结构
```
index.html          页面主体（样式、脚本、地球纹理、头像均已内嵌）
vendor/three.min.js 本地 three.js（旋转地球渲染，不依赖 CDN）
covers/work1~4.jpg  4 个作品的 16:9 封面图
README.md           本文件
.gitignore
```

## 本地预览
双击 `index.html` 用浏览器打开即可（地球、封面、脚本都能正常跑）。

## 修改内容只需要改一个地方
打开 `index.html`，找到开头的 `const SITE = { ... }`（约第 483 行）：

```js
const SITE = {
  bilibili : "https://space.bilibili.com/405303397",
  douyin   : "",   // 抖音主页链接
  email    : "",   // 联系邮箱，如 mailto:you@example.com
  afdian   : "",   // 爱发电主页，如 https://afdian.com/a/你的ID
  mbd      : "",   // 或面包多 https://mbd.pub/o/你的ID
};
```

改完保存，`git push` 即自动上线。

## 付费通道（爱发电）开通步骤
1. 打开 https://afdian.com 注册账号（微信/手机号都行）。
2. 点右上角头像 →「创作者中心」，设置你的专属主页 ID（即 `https://afdian.com/a/你的ID` 里的 `你的ID`）。
3. 在「商品 / 发电方案」里创建你要出售的插件商品（如「一键转换工具 Pro 版」，定价自定）。
4. 把 `https://afdian.com/a/你的ID` 填到上面 `SITE.afdian` 里。
5. 保存并 `git push` —— 首页「购买 Pro 版」和「去爱发电支持」两个按钮会自动指向你的主页。

> 想用面包多（mbd.pub）同理，把链接填到 `SITE.mbd` 即可（付费按钮优先用爱发电）。

## 部署方式（已配置，可复用）
- 已通过 Vercel CLI 部署并连接 GitHub 仓库。
- 若换新机器，重新登录即可：
  ```bash
  npm i -g vercel      # 安装 CLI
  vercel login         # 浏览器授权
  vercel --prod        # 在项目目录下部署
  ```
