# Comark — Downloads

Capture on Mac or Windows. Annotate on iPad. Copy your feedback back.

This public repository contains product information and binaries only. All application source code remains private. Downloading a published release requires no GitHub sign-in.

[Website](https://comark.work) · [All releases](https://github.com/Joseph-Jin/Comark-Downloads/releases)

## Desktop downloads

| Platform | Download | Requirements |
| --- | --- | --- |
| Mac 1.0 | [Comark-Mac-v1.0.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/Comark-Mac-v1.0.zip) | macOS 14+, Apple silicon or Intel |
| Windows 1.0.1 (ZIP) | [Comark-Windows.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0.1-windows/Comark-Windows.zip) | Windows 10/11 x64; no Python installation needed |
| Windows 1.0.1 (installer) | [Comark-Setup-1.0.1.exe](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0.1-windows/Comark-Setup-1.0.1.exe) | Per-user install, no admin required |
| Checksums | [SHA256SUMS.txt](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0.1-windows/SHA256SUMS.txt) | Windows 1.0.1 + Mac 1.0 hashes |

One-line install:

    # macOS
    curl -fsSL https://comark.work/install.sh | sh

    # Windows
    irm https://comark.work/install.ps1 | iex

Both desktop companions require an iPad with Comark installed. They cannot be used on their own. iPad v1.0 (Build 32) is on TestFlight; installation requires an invitation. A public App Store download is not available yet.

### Mac 1.0

**⚠️ First-time users:** macOS may block this build from opening. [See installation guide](https://comark.work/mac-guide) for three simple methods to open it. This is a one-time step; after that, the app opens normally.

Unzip and move ComarkMac.app to Applications. Open it and allow screen recording when asked, then pair using its six-digit code. The download is the macOS universal app, signed with an Apple Development certificate. Apple notarization requires a Developer ID certificate and is pending.

### Windows 1.0.1 — fixes the "part of this app has been blocked" startup error

Some Windows machines blocked v1.0 at startup: Windows Security reported *"Part of this app has been blocked ... registry.cp312-win_amd64.pyd"*. In 1.0.1 the Bonjour discovery library ships as **pure Python**, so that component no longer exists in the package. Pairing, display capture, and clipboard behavior are unchanged.

Also new in 1.0.1: startup errors are reported accurately (a blocked component is no longer mislabeled as "port in use"), a failed start releases the port so you can retry immediately, and the self-check no longer reports OK while another program occupies the port.

Extract the whole `Comark-Windows` folder (keep `_internal` beside the EXE) and double-click `Comark-Windows.exe`, or run the installer. Run the self-check first: it verifies Wi-Fi, Bonjour, firewall rules, and display capture, and can request UAC permission to repair Comark firewall rules. Then click **Start advertisement** and allow the private-network firewall prompt. On iPad, open **Connect computer**, press Rediscover, select the PC, and enter its six-digit code. Keep both devices on the same LAN.

**Not code-signed.** SmartScreen or Smart App Control may still confirm before opening, and additional security software could block a different component. Do not disable Windows security. If a block appears, note the file name from Event Viewer → CodeIntegrity → Operational (event 3077) and report it at [comark.work/support](https://comark.work/support). A fully signed release is planned once a trusted code-signing certificate is enrolled.

### What's in v1.0

- Apple on-device speech recognition is the default engine on iPad, with no configuration required.
- Voice pen records while you draw and drops numbered, transcribed markers on the image.
- Bottom caption renders live under the image and exports together with the annotation.
- Automatic reconnect to the last paired computer after sleep, lock, or a network change.
- Destination-aware copy messages that name Mac or Windows correctly.
- Windows self-check with one-click firewall repair, and a DPI fix for the window resizing on Start advertisement.
- English and Simplified Chinese throughout both desktop companions and the iPad app.

## 中文说明

本仓库仅公开产品说明与下载文件，应用源码保持私有。下载无需 GitHub 账号。

**Mac 用户注意：** 首次打开时 macOS 可能提示无法验证，请查看[安装指南](https://comark.work/mac-guide)了解三种简单的打开方法。

**Windows 用户注意（v1.0.1 修复）：** 部分电脑上 v1.0 启动时被 Windows 安全中心拦截——提示「此应用的一部分已被阻止 … registry.cp312-win_amd64.pyd」。v1.0.1 将发现服务改为纯 Python 实现，该组件已不存在；配对、截图、剪贴板功能不变。同时改进：启动错误如实提示（组件被拦截不再误报端口占用）、启动失败后释放端口可直接重试、自检不再把端口被其他程序占用误判为正常。完整解压 `Comark-Windows` 文件夹（保持 `_internal` 在 EXE 旁）后双击 `Comark-Windows.exe`，或直接运行安装器。

**签名状态：** Windows 1.0.1 与 Mac 均未完成发行签名，SmartScreen / Gatekeeper / 智能应用控制仍可能提示确认。请不要关闭安全防护；如仍被拦截，请在事件查看器（CodeIntegrity → Operational，事件 3077）记下被拦截的文件名，并通过 [comark.work/support](https://comark.work/support) 反馈。已计划接入受信任的代码签名证书后发布签名版。

两台设备需在同一局域网；Windows 端无法脱离 iPad 单独使用。校验值见 `SHA256SUMS.txt`。

## Rights

Copyright © 2026 Joseph-Jin. All rights reserved. No open-source license is granted for the applications by this repository.

