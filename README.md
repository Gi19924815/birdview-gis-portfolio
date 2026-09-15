# 鸟瞰地图的图形基地 · 个人网站

赛博朋克风格的静态单页网站，用于**作品展示 / 教程 / 插件展示·发布·出售**。
纯 HTML + CSS + JS，无任何依赖，单文件即可上线。

## 文件
- `index.html` —— 全部页面（样式、脚本、头像均已内嵌，可直接打开/部署）

## 本地预览
双击 `index.html` 用浏览器打开即可。

## 部署上线（任选其一）

### 方式 A：Vercel（推荐，免费 + 自动 HTTPS）
1. 打开 https://vercel.com 用 GitHub / 邮箱登录。
2. 点 **Add New → Project**，把本文件夹拖进去（或先推到 GitHub 再导入仓库）。
3. 框架选 **Other / 无需配置**，直接 **Deploy**。
4. 几分钟后得到 `xxx.vercel.app` 免费域名。

### 方式 B：任意静态托管
- GitHub Pages / Netlify / Cloudflare Pages：直接上传 `index.html` 即可。
- 自有服务器：把 `index.html` 放到网站根目录。

## 上线前你需要改的地方（搜索 TODO 或占位内容）
| 位置 | 要改什么 |
|---|---|
| 「一键转换工具 Pro 版」卡片 | 价格 `¥29` 与真实购买/授权链接（爱发电 / 面包多 / Gumroad） |
| 页脚「抖音」「联系我」 | 换成你的真实链接 / 邮箱 |
| 百度网盘链接 | 目前指向你原来的 `12Ik7cscFRKOTWLsBe9ghBg`（提取码 6666），确认仍是有效资源 |
| 作品卡封面 | 目前用 B 站 iframe 直接嵌入，可换成自制的 16:9 封面图 |

## 绑定正式域名（进阶）
买好域名后，在 Vercel 项目 **Settings → Domains** 添加，然后到域名商改 DNS 解析（Vercel 有图文引导）。
