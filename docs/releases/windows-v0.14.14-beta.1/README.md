# Windows 0.14.14-beta.1 版本材料

[返回安装包下载页](https://github.com/JinCrown/doulivideo/releases/tag/windows-v0.14.14-beta.1)。

Windows 10/11 x64 安装器：[DouliListen-0.14.14-beta.1-windows-x64-setup.exe](https://github.com/JinCrown/doulivideo/releases/download/windows-v0.14.14-beta.1/DouliListen-0.14.14-beta.1-windows-x64-setup.exe)。安装器自带运行环境，退出旧程序后运行安装器更新。

SHA-256：`967c00038a4fbb451de0909f317b877d9360a18275a816e7e874d6fb99352d39`。

## 更新内容

- 平台切换区域与左侧导航栏统一宽度，改用圆角按钮、左右切换图标和“切换”文字。
- 删除侧栏“正在播放”和底栏字幕入口，保留左下角封面、标题区域进入播放页；播放页内的字幕与歌词功能保留。
- 清理 B站、抖音的首页卡片、悬浮按钮、更多菜单、播放页、队列、发现、历史及稍后再听中的本机收藏入口。
- 保留两平台的账号收藏操作，已有本地数据继续保留。

815 项自动化测试和 14 组隔离样例界面渲染通过，并检查千条合集的滚动、分页与缩放。预览图的封面由测试代码绘制，不包含用户真实账号或收藏。

## 签名与组件

沿用固定的 Windows 自签名内测身份，尚无 Windows 公共信任。证书 SHA-256：`6b7d4ef720fd83b29d6627b5f02fe5bb353b32f10f6653af82d75d7e83f55483`。[公开证书](DouliListen-Windows-Beta.cer)仅供核对，无需导入系统根证书。

- [文件 SHA-256](SHA256SUMS.txt)
- [Windows 随包第三方许可证与声明](Windows-third-party-notices.zip)
- [Windows 原生音频组件源码及构建脚本](Windows-native-audio-component-source.zip)

安装包携带 CEF、VLC、FFmpeg 和 Java 运行时，无需另装 Java 或 VLC。第三方组件遵循各自原有许可；本仓库不提供应用业务源码。

手机版继续使用 [0.35.9-beta.1 APK](https://github.com/JinCrown/doulivideo/releases/download/v0.35.9-beta.1/doulivideo-0.35.9-beta.1.apk)，本次没有更改手机版安装包或签名。其 [SHA-256 与 Android 组件材料](../v0.35.9-beta.1/README.md)保持原样。
