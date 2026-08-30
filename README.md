# RemoteMouse 安装包发布

RemoteMouse 把安卓手机变成 Windows / macOS 的触摸板、飞鼠和键盘。本仓库只存放桌面端与 Android 安装包，源码在私有仓库开发，不在此公开。

## 下载 v1.0.0

- macOS（Apple Silicon，需 macOS 13+）：[RemoteMouse-1.0.0.dmg](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/RemoteMouse-1.0.0.dmg)
- Windows 10/11：[RemoteMouse-1.0.0.msi](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/RemoteMouse-1.0.0.msi)
- Android 8.0+：[RemoteMouse-1.0.0.apk](https://github.com/yangwuan55/remotemouse-release/releases/latest/download/RemoteMouse-1.0.0.apk)

以上链接始终指向最新版本。

## 安装说明

- **macOS**：打开 DMG，把 RemoteMouse 拖入 Applications；首次使用需在「系统设置 → 隐私与安全性 → 辅助功能」中授权。
- **Windows**：双击 MSI 安装并启动 RemoteMouse Desktop；如被 SmartScreen 拦截，选择「仍要运行」。
- **Android**：直接安装 APK（需允许安装未知来源应用）；应用上架 Google Play 后将优先从商店下载。

## 安全提示

安装包与手机端在同一局域网内通信（UDP 19826 / WebSocket 19827），6 位 PIN 配对，不经过任何公网服务器。请仅从本仓库 Releases 或官网获取安装包。
