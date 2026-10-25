# 手机版 0.36.5-beta.1 / Windows 0.14.22-beta.1 版本材料

发布日期：2026-10-25。普通用户下载 [手机版 APK](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/doulivideo-0.36.5-beta.1.apk) 或 [Windows x64 安装器](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/DouliListen-0.14.22-beta.1-windows-x64-setup.exe) 即可。

| 安装包 | 大小 | SHA-256 |
| --- | ---: | --- |
| doulivideo-0.36.5-beta.1.apk | 15,401,625 字节 | `472df044c45169a5e9ca3b256cb85f13c0e79689319f119d611fdfd0f23275a8` |
| DouliListen-0.14.22-beta.1-windows-x64-setup.exe | 526,818,544 字节 | `ab73724cc3d992460259fd0a41f22ee9d6219b8721d1c3129704681edb47f8a4` |

## 升级与签名

Android 应用 ID 为 `app.doulilisten.prototype`，版本代码 205，正式构建不可调试。沿用独立发布签名，证书 SHA-256 为 `016e9d674b549a39e6500cb072e14bfca6992aa420e89df7434ef3652dcca6f3`。同包名且签名匹配的旧发布包可覆盖更新；曾安装本地测试签名包时可能出现冲突，请先保留需要的数据。

Windows 退出旧版后运行安装器更新，沿用固定内测证书，证书 SHA-256 为 `6b7d4ef720fd83b29d6627b5f02fe5bb353b32f10f6653af82d75d7e83f55483`。自签名内测证书可能触发系统信任提示。安装器包含运行环境，支持 Windows 10/11 x64。

## 可下载的组件材料

- [SHA256SUMS.txt](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/SHA256SUMS.txt)：安装包与附件哈希。
- [SoundTouch-2.4.1-corresponding-source.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/SoundTouch-2.4.1-corresponding-source.zip)：与本次 APK 配套的 SoundTouch 上游源码、JNI 适配及构建说明。
- [Android-third-party-notices.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Android-third-party-notices.zip)：本次 APK 配套的第三方许可证和声明。
- [Windows-native-audio-component-source.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Windows-native-audio-component-source.zip)：Windows 原生音频输出及音量均衡组件源码、许可和构建脚本。
- [Windows-third-party-notices.zip](https://github.com/JinCrown/doulivideo/releases/download/v0.36.5-beta.1/Windows-third-party-notices.zip)：桌面运行组件的第三方声明与许可。
- [Windows 内测公开证书](DouliListen-Windows-Beta.cer)：供核对签名使用，无需导入证书即可使用软件。

组件材料不包含应用业务源码。GitHub 自动生成的 Source code 压缩包仅包含本仓库公开介绍资料与历史组件材料。

## 验证范围

手机版 1,007 项、电脑版 858 项自动化测试通过。两平台关注列表已完成真实账号只读核对；手机完成关注入口、搜索、排序、作者主页跳转及返回状态检查。电脑版完成隔离样例布局及真实播放器回归。测试不代表所有设备、所有账号或所有平台接口均已覆盖。
