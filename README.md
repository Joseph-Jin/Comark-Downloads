# Comark — Downloads

Capture on Mac or Windows. Annotate on iPad. Copy your feedback back.

This public repository contains product information and binaries only. All application source code remains private. Downloading a published release requires no GitHub sign-in.

[Website](https://comark.work) · [All releases](https://github.com/Joseph-Jin/Comark-Downloads/releases)

## Desktop downloads

| Platform | Download | Requirements |
| --- | --- | --- |
| Mac 1.0 | [Comark-Mac-v1.0.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/Comark-Mac-v1.0.zip) | macOS 14+, Apple silicon or Intel |
| Windows 1.0.2 (MSI) | [Comark-Windows-1.0.2.msi](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0.2-windows/Comark-Windows-1.0.2.msi) | Windows 10/11 x64; per-user install, no admin or Python needed |
| Checksums | [SHA256SUMS.txt](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0.2-windows/SHA256SUMS.txt) | Windows 1.0.2 + Mac 1.0 hashes |

One-line install:

    # macOS
    curl -fsSL https://comark.work/install.sh | sh

    # Windows
    irm https://comark.work/install.ps1 | iex

Both desktop companions require an iPad with Comark installed. They cannot be used on their own. The Comark iPad app 1.0 is in App Store review; the App Store link will be added here once it is approved. Comark is not offered on the China mainland App Store for this release.

### Mac 1.0

**⚠️ First-time users:** macOS may block this build from opening. [See installation guide](https://comark.work/mac-guide) for three simple methods to open it. This is a one-time step; after that, the app opens normally.

Unzip and move ComarkMac.app to Applications. Open it and allow screen recording when asked, then pair using its six-digit code. The download is the macOS universal app, signed with an Apple Development certificate. Apple notarization requires a Developer ID certificate and is pending.

### Windows 1.0.2 — MSI installer

Windows now ships as a standard MSI installer. Earlier releases were a ZIP: extracting a downloaded ZIP marks every EXE, DLL and PYD inside as coming from the internet, and Smart App Control or SmartScreen could block one of them. The MSI is installed by Windows Installer, the way most Windows software is installed.

Double-click `Comark-Windows-1.0.2.msi`. It installs for your user account with no administrator prompt and adds Comark to the Start menu. Upgrading from 1.0.1 keeps your device identity and pairing code; uninstall from Settings → Apps. Open Comark and run the self-check first: it verifies Wi-Fi, Bonjour, firewall rules, and display capture, and can request UAC permission to repair Comark firewall rules. Then click **Start advertisement** and allow the private-network firewall prompt. On iPad, open **Connect computer**, press Rediscover, select the PC, and enter its six-digit code. Keep both devices on the same LAN.

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

**iPad 端：** Comark iPad 1.0 正在 App Store 审核中，通过后会在这里补上 App Store 链接。本版本暂不在中国大陆 App Store 上架。

**Mac 用户注意：** 首次打开时 macOS 可能提示无法验证，请查看[安装指南](https://comark.work/mac-guide)了解三种简单的打开方法。

**Windows 用户注意（v1.0.2 改为 MSI 安装包）：** 以前的 ZIP 解压后，里面每个 EXE、DLL、PYD 都会带上"来自网络"的标记，可能被智能应用控制或 SmartScreen 拦截。现在改为标准 MSI 安装包，由 Windows Installer 安装。双击 `Comark-Windows-1.0.2.msi` 即可，按用户安装、无需管理员权限，并会添加到开始菜单；从 1.0.1 升级会保留配对码与设备身份，可在「设置 → 应用」中卸载。

**签名状态：** Windows 1.0.2 与 Mac 均未完成发行签名，SmartScreen / Gatekeeper / 智能应用控制仍可能提示确认。请不要关闭安全防护；如仍被拦截，请在事件查看器（CodeIntegrity → Operational，事件 3077）记下被拦截的文件名，并通过 [comark.work/support](https://comark.work/support) 反馈。已计划接入受信任的代码签名证书后发布签名版。

两台设备需在同一局域网；Windows 端无法脱离 iPad 单独使用。校验值见 `SHA256SUMS.txt`。

## Rights

Copyright © 2026 Joseph-Jin. All rights reserved. No open-source license is granted for the applications by this repository.
