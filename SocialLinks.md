# 社交平台短链接

2026-11-09 建立。用于 TikTok、Facebook、YouTube 主页简介，把观众带到 Google Play，并按来源统计安装量。

## 链接对照

| 平台 | 短链接（放在主页简介） | 跳转目标（Play，带 referrer） |
| --- | --- | --- |
| TikTok | https://loadingstudiomy.github.io/tt | `https://play.google.com/store/apps/details?id=com.loadingstudiomy.waytohell&referrer=utm_source%3Dtiktok%26utm_medium%3Dsocial%26utm_campaign%3Dbio` |
| Facebook | https://loadingstudiomy.github.io/fb | `https://play.google.com/store/apps/details?id=com.loadingstudiomy.waytohell&referrer=utm_source%3Dfacebook%26utm_medium%3Dsocial%26utm_campaign%3Dbio` |
| YouTube | https://loadingstudiomy.github.io/yt | `https://play.google.com/store/apps/details?id=com.loadingstudiomy.waytohell&referrer=utm_source%3Dyoutube%26utm_medium%3Dsocial%26utm_campaign%3Dbio` |

不带追踪参数的商店链接：https://play.google.com/store/apps/details?id=com.loadingstudiomy.waytohell

## 文件与发布

- 项目里的副本：[website/tt](website/tt/index.html)、[website/fb](website/fb/index.html)、[website/yt](website/yt/index.html)。每个页面都用 meta refresh 立即跳转，同时留一个手动点击的链接，并设置 `noindex`。
- 线上位置：GitHub 仓库 `loadingstudiomy.github.io` 根目录下的 `tt/`、`fb/`、`yt/` 文件夹，与 `app-ads.txt` 同一个仓库。上传和修改都由用户在 GitHub 网页上操作。
- 发布状态：**未确认**。上传后要用浏览器逐个打开，确认能跳到 Play 才算完成。
- 以后如果给 GitHub Pages 绑定自定义域名，这些路径不用改，会自动变成 `域名/tt` 等。

## 查看来源数据

在 Play Console 打开 Way To Hell，进入 **用户获取 → 获取报告**，按 UTM 来源（utm_source）查看。数据通常会延迟一到两天。这个统计只记录经过上面链接安装的用户；直接在 Play 搜索安装的不算。

## 平台限制（2026-11 的整理，未逐项实测）

- 三个平台的自然流量竖屏视频，画面里都不能放可点击按钮；TikTok 和 Shorts 的说明栏、评论里的链接也不能点。所以链接放在主页简介里，视频结尾加上 “Free on Google Play · Link in bio”。
- 要让视频上直接出现安装按钮，只能投付费广告：TikTok App 推广、Meta 应用推广，或 Google Ads 应用广告系列（会覆盖 YouTube Shorts）。
- Firebase Dynamic Links 已经在 2025-08 停止服务，不要使用。
