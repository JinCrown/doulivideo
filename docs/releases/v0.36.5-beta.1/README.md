# 手机版 0.36.5-beta.1 / Windows、macOS 0.14.22-beta.1 版本材料

发布日期：2026-10-25。普通用户从 [本次发布页](https://github.com/JinCrown/doulivideo/releases/tag/v0.36.5-beta.1) 按设备选择 APK、Windows 安装器或对应芯片的 Mac DMG。

| 安装包 | 大小 | SHA-256 |
| --- | ---: | --- |
| doulivideo-0.36.5-beta.1.apk | 15,401,625 字节 | `472df044c45169a5e9ca3b256cb85f13c0e79689319f119d611fdfd0f23275a8` |
| DouliListen-0.14.22-beta.1-windows-x64-setup.exe | 526,818,544 字节 | `ab73724cc3d992460259fd0a41f22ee9d6219b8721d1c3129704681edb47f8a4` |
| [DouliListen-0.14.22-beta.1-macos-arm64.dmg](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/DouliListen-0.14.22-beta.1-macos-arm64.dmg) | 430,096,885 字节 | `c3f6c56705fd901933b8089d830ed92c321e026bba2b22506fb84e046199e161` |
| [DouliListen-0.14.22-beta.1-macos-x64.dmg](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/DouliListen-0.14.22-beta.1-macos-x64.dmg) | 443,757,709 字节 | `28b9422f175188fcdca3305bce073858c60934b1e6a818a58de33f2042553597` |

## 升级与签名

Android 应用 ID 为 `app.doulilisten.prototype`，版本代码 205，正式构建不可调试。沿用独立发布签名，证书 SHA-256 为 `016e9d674b549a39e6500cb072e14bfca6992aa420e89df7434ef3652dcca6f3`。同包名且签名匹配的旧发布包可覆盖更新；曾安装本地测试签名包时可能出现冲突，请先保留需要的数据。

Windows 退出旧版后运行安装器更新，沿用固定内测证书，证书 SHA-256 为 `6b7d4ef720fd83b29d6627b5f02fe5bb353b32f10f6653af82d75d7e83f55483`。自签名内测证书可能触发系统信任提示。安装器包含运行环境，支持 Windows 10/11 x64。

Mac 测试包分别提供 Apple Silicon（ARM64）和 Intel（x64）版本。打开 DMG 后将「抖哩听视频.app」拖入 Applications。本包使用临时本地签名，未取得 Apple Developer ID 签名及苹果公证；首次打开可能需要在「系统设置 → 隐私与安全性」选择「仍要打开」，步骤见 [苹果官方说明](https://support.apple.com/zh-cn/102445)。自带 Java、VLC、FFmpeg 和登录运行库，无需另外安装。

Mac 本地资料及默认下载分别位于 `~/Library/Application Support/DouliListenDesktop` 与其 `downloads` 子目录，更新应用时不必清空这些目录。

## 可下载的组件材料

- [SHA256SUMS.txt](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/SHA256SUMS.txt)：安装包与附件哈希。
- [SoundTouch-2.4.1-corresponding-source.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/SoundTouch-2.4.1-corresponding-source.zip)：与本次 APK 配套的 SoundTouch 上游源码、JNI 适配及构建说明。
- [Android-third-party-notices.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Android-third-party-notices.zip)：本次 APK 配套的第三方许可证和声明。
- [Windows-native-audio-component-source.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Windows-native-audio-component-source.zip)：Windows 原生音频输出及音量均衡组件源码、许可和构建脚本。
- [Windows-third-party-notices.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Windows-third-party-notices.zip)：桌面运行组件的第三方声明与许可。
- [Mac-native-audio-component-source.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Mac-native-audio-component-source.zip)：Mac 音量均衡桥接、输出观察组件、许可与重建脚本。
- [SHA256SUMS-macos-arm64.txt](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/SHA256SUMS-macos-arm64.txt) / [SHA256SUMS-macos-x64.txt](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/SHA256SUMS-macos-x64.txt)：对应架构 DMG 的构建校验清单。
- [Windows 内测公开证书](DouliListen-Windows-Beta.cer)：供核对签名使用，无需导入证书即可使用软件。

组件材料不包含应用业务源码。GitHub 自动生成的 Source code 压缩包仅包含本仓库公开介绍资料与历史组件材料。

## 验证范围

手机版 1,007 项、电脑版 858 项自动化测试通过。两平台关注列表已完成真实账号只读核对；手机完成关注入口、搜索、排序、作者主页跳转及返回状态检查。电脑版完成隔离样例布局及真实播放器回归。测试不代表所有设备、所有账号或所有平台接口均已覆盖。

Mac 两种架构分别在 macOS 15 云构建机完成编译、自动化测试、原生静音播放与跳转、循环播放及均衡切换检查，应用临时签名和 DMG 完整性检查通过。Mac 真实账号登录与其他系统版本、设备仍需测试。
