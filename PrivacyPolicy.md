# Way To Hell 隐私政策草稿

起草：2026-11-03，依据当时项目实际接入的 SDK（LevelPlay 9.5.1，Unity Ads 与 Google AdMob 适配器，只有激励视频广告；无账号、无分析、无内购）。这是模板草稿，不是法律意见；发布前把英文版贴到公开网页（如 Google Sites），并让 Play Console「目标受众」与第 6 条一致。以后加入分析、内购、账号或新广告网络时必须同步修改。

英文版是要发布的正文，中文版供对照。

---

## English (publish this)

# Privacy Policy — Way To Hell

**Effective date:** 3 November 2026
**Developer:** LoadingStudioMY
**Contact:** loadingstudiomy@gmail.com

This policy explains what information the mobile game *Way To Hell* (the "Game") handles and why. We have tried to keep it short and plain.

### 1. Information we collect ourselves

We do not ask for your name, email, phone number, location or any account. The Game has no login and no server of its own.

Your progress (coins, best depth, upgrades, shop items, sound volume and similar settings) is stored **only on your device**. We cannot see it. Uninstalling the Game deletes it.

If you email us, we receive your email address and whatever you write, and use them only to reply to you.

### 2. Advertising

The Game is free and shows **rewarded video ads only when you choose to watch one** (for example, to revive or to double your coins). Ads are delivered through these third-party services:

| Service | Provider | Privacy policy |
| --- | --- | --- |
| LevelPlay (ad mediation) | Unity Technologies / ironSource | https://unity.com/legal/game-player-and-app-user-privacy-policy |
| Unity Ads | Unity Technologies | https://unity.com/legal/game-player-and-app-user-privacy-policy |
| Google AdMob | Google LLC | https://policies.google.com/privacy |

To show and measure ads, prevent fraud and, where allowed, personalise ads, these services may collect from your device: the advertising ID (Android Advertising ID), IP address, device model, operating system and language, app version, approximate location derived from the IP address, and information about ads you see and interact with. They process this data under their own privacy policies listed above. We do not sell your personal information ourselves.

You can reset your advertising ID or opt out of personalised ads at any time in your Android settings (Settings › Google › Ads, or Settings › Privacy › Ads, depending on the device).

### 3. Consent (EEA, UK and Switzerland)

If you are in the European Economic Area, the United Kingdom or Switzerland, the Game asks for your choice about personalised advertising the first time you play, using Google's consent tool. You can change your choice later from **Settings › Privacy options** in the Game. If you do not consent, you may still see non-personalised ads.

### 4. United States privacy rights

Depending on your state, you may have the right to opt out of the "sale" or "sharing" of personal information for targeted advertising. The Game sends an opt-out signal to its ad services by default. You can also use the Android ad settings described in section 2.

### 5. Data retention and security

We keep no player data on our own servers. Emails you send us are kept only as long as needed to handle your request. Ad providers keep data according to their own policies.

### 6. Children

The Game is not directed at children under 13 (or the minimum age in your country), and we do not knowingly collect personal information from children. If you believe a child has sent us personal information, contact us and we will delete it.

### 7. Your rights

Depending on where you live, you may have rights to access, correct or delete personal data, or to object to its processing. Because we hold no player data except emails you send us, most requests about advertising data are handled by the ad providers listed above; we will help you reach them. Contact: loadingstudiomy@gmail.com.

### 8. Changes

If this policy changes, we will update the effective date above and publish the new version at the same address.

---

## 中文对照

# Way To Hell 隐私政策

**生效日期：** 2026 年 11 月 3 日
**开发者：** LoadingStudioMY
**联系方式：** loadingstudiomy@gmail.com

### 1. 我们自己收集的信息
不要求姓名、邮箱、电话、位置或账号，游戏没有登录，也没有自己的服务器。金币、最佳深度、升级、商品、音量等进度只存在你的手机上，我们看不到，卸载游戏即删除。你给我们发邮件时，我们只用你的邮箱地址和内容来回复你。

### 2. 广告
游戏免费，只有在你主动选择时（如复活、金币翻倍）才播放激励视频广告，由 LevelPlay（广告聚合）、Unity Ads、Google AdMob 提供（各自隐私政策链接见英文版表格）。为投放和统计广告、防作弊以及在允许时个性化广告，这些服务可能收集：广告 ID、IP 地址、设备型号、系统和语言、应用版本、由 IP 推算的大致位置、广告浏览和点击信息，并按它们自己的政策处理。我们自己不出售你的个人信息。你可以随时在安卓设置里重置广告 ID 或关闭个性化广告。

### 3. 同意（欧洲经济区、英国、瑞士）
首次游戏时会用 Google 的同意工具询问你是否接受个性化广告；之后可在游戏「设置 › 隐私选项」修改。不同意时仍可能看到非个性化广告。

### 4. 美国隐私权利
视所在州，你有权拒绝为定向广告「出售」或「共享」个人信息。游戏默认向广告服务发送拒绝信号，你也可以用第 2 条的安卓广告设置。

### 5. 保存与安全
我们不在自己的服务器上保存玩家数据；来信只保留到处理完为止；广告服务商按其政策保存数据。

### 6. 儿童
游戏不面向 13 岁以下（或你所在国家规定的最低年龄）儿童，我们不会故意收集儿童个人信息；如发现，请联系我们删除。

### 7. 你的权利
视所在地，你可能有权查阅、更正、删除个人数据或反对处理。我们除了来信外不持有玩家数据，涉及广告数据的请求主要由上述广告服务商处理，我们会协助你联系。

### 8. 变更
政策变更时会更新上方生效日期，并在同一网址发布新版本。

---

## 发布前核对

- 第 3 条描述的是计划中的同意弹窗和「隐私选项」入口；如果同意流程最终没有接入，或决定先不在欧洲、英国、瑞士上架，要删改第 3 条。
- 第 4 条依据当前代码 `LevelPlayPrivacySettings.SetCCPA(true)`（默认对所有人发送拒绝信号）；如以后改成让玩家选择，要同步修改。
- 第 6 条要与 Play Console「目标受众和内容」里选的年龄段一致（建议选 13 岁以上）。
- Unity 隐私政策链接以发布当天 unity.com/legal 页面为准，失效时替换。
