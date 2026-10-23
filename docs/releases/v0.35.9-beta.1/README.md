# 手机版 0.35.9 / Windows 0.14.13 版本材料

[返回安装包下载页](https://github.com/JinCrown/doulivideo/releases/tag/v0.35.9-beta.1)。普通用户只需按设备下载 APK 或 Windows setup.exe。

| 平台 | 发布版本 | 安装包 SHA-256 |
| --- | --- | --- |
| Android 8.0+ | 0.35.9-beta.1（版本代码 199） | `df912ee85e2d13f46b6a45e36c7c4100e30b46e1927289a6f5f9606d2c8d1f7b` |
| Windows 10/11 x64 | 0.14.13-beta.1 | `2f72f0a530146346522b5d518493a8b8e6073ceb8a2b03d2057b78ab55f7f416` |

Android 沿用原发布签名，可覆盖 GitHub 的 0.35.8-beta.1；本机 Debug/InternalQa 包可能签名不同。更新前应导出需保留的资料，避免因直接卸载丢失记录。

Windows 沿用固定的自签名内测身份，不具有 Windows 公共信任。发布包与之前本地未签名构建的区别为签名及内测版本标识，功能仍为 0.14.13。
证书 SHA-256：`6b7d4ef720fd83b29d6627b5f02fe5bb353b32f10f6653af82d75d7e83f55483`。
[公开证书](DouliListen-Windows-Beta.cer)仅供核对，不需要导入系统根证书。

## 组件材料

- [全部文件 SHA-256](SHA256SUMS.txt)
- [Android 第三方声明](third-party-notices.zip)
- [SoundTouch 2.4.1 对应源码、构建与替换材料](SoundTouch-2.4.1-corresponding-source.zip)
- [Windows 随包第三方许可证与声明](Windows-third-party-notices.zip)
- [Windows 原生音频组件源码及构建脚本](Windows-native-audio-component-source.zip)

Android 原生库与随包许可证已逐项核对，与 0.35.8-beta.1 一致，复用相同的组件材料。
Windows 安装包携带 CEF、VLC、FFmpeg 和 Java 运行时，无需另装 Java 或 VLC。
新下载保存在安装目录的 downloads 文件夹；旧下载、账号与本机记录仍保存在 `%LOCALAPPDATA%\DouliListenDesktop` 下。
第三方组件遵循各自许可；本发布仓库不提供应用业务源码，GitHub 自动生成的 Source code 压缩包只包含公开介绍资料与组件材料。

## 本次验证

Android：982 项单元测试、Lint、结构与安装包检查，固定签名与 16 KiB 对齐校验。
Windows：815 项自动化测试，14 组隔离样例界面截图、千条合集滚动/分页/缩放检查及播放下载检查。
预览图使用测试代码绘制的封面与隔离样例数据，不包含用户真实账号和收藏。测试通过不等于全机型或全部账号场景均已验收。
