# TouchSpan 安装包发布

TouchSpan 把安卓手机变成 Windows / macOS 的触摸板、飞鼠、键盘和语音输入。本仓库只存放桌面端与 Android 安装包，源码在私有仓库开发，不在此公开。

## 下载

以下链接始终指向最新版本的安装包：

- macOS（Apple Silicon，需 macOS 13+）：[TouchSpan-1.0.2.dmg](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/TouchSpan-1.0.2.dmg)
- Windows 10/11：[TouchSpan-1.0.2.msi](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/TouchSpan-1.0.2.msi)（另有 [TouchSpan-1.0.2.exe](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/TouchSpan-1.0.2.exe)）
- Android 8.0+：优先从 Google Play 安装 [com.touchspan.kmp](https://play.google.com/store/apps/details?id=com.touchspan.kmp)（当前 1.0.5）；也可直装 [TouchSpan-1.0.2.apk](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/TouchSpan-1.0.2.apk)（需允许安装未知来源应用）。

## 安装说明

- **macOS**：打开 DMG，把 TouchSpan 拖入 Applications。首次使用需在「系统设置 → 隐私与安全性 → 辅助功能」中授权 TouchSpan，否则手机能连上但指针不会动。安装包已用 Developer ID 签名，但**尚未做公证（notarization）**，若 Gatekeeper 拦截，请右键应用图标选择「打开」再确认。
- **Windows**：双击 MSI 安装并启动 TouchSpan Desktop。安装包**没有代码签名**，被 SmartScreen 拦截时选择「仍要运行」；首次运行需在防火墙提示中允许 TouchSpan 访问专用网络。
- **Android**：从 Google Play 安装即可；APK 直装为备选。

## 费用与广告

基础能力免费，无需账号。免费版含低频广告（设置页与历史页底部横幅，以及断开连接后受频控的插屏），广告不会遮挡触摸板或控制操作。**目前没有付费版。**

## 安全提示

安装包与手机端在同一局域网内通信（UDP 19826 发现 / WebSocket 19827 控制），6 位 PIN 配对，首次连接需电脑端确认，之后的控制消息携带仅本次连接有效的会话令牌；输入内容不经过任何公网服务器。不做远程桌面与文件传输。请仅从本仓库 Releases 或官网 <https://touchspan.gratiskit.com/> 获取安装包。
