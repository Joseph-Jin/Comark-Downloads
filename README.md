# Comark — Downloads

Capture on Mac or Windows. Annotate on iPad. Copy your feedback back.

This public repository contains product information and binaries only. All application source code remains private. Downloading a published release requires no GitHub sign-in.

[Website](https://comark.work) · [All releases](https://github.com/Joseph-Jin/Comark-Downloads/releases)

## Desktop downloads · v1.0

| Platform | Download | Requirements |
| --- | --- | --- |
| Mac 1.0 | [Comark-Mac.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/Comark-Mac.zip) | macOS 14+, Apple silicon or Intel |
| Windows 1.0 | [Comark-Windows.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/Comark-Windows.zip) | Windows x64; no Python installation needed |
| Checksums | [SHA256SUMS.txt](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/SHA256SUMS.txt) | Verify each ZIP file |

One-line install:

    # macOS
    curl -fsSL https://comark.work/install.sh | sh

    # Windows
    irm https://comark.work/install.ps1 | iex

Both desktop companions require an iPad with Comark installed. They cannot be used on their own. iPad v1.0 (Build 24) is on TestFlight; installation requires an invitation. A public App Store download is not available yet.

### Mac

**⚠️ First-time users:** macOS may block this build from opening. [See installation guide](https://comark.work/mac-guide) for three simple methods to open it. This is a one-time step; after that, the app opens normally.

Unzip and move ComarkMac.app to Applications. Open it and allow screen recording when asked, then pair using its six-digit code. The download is the macOS universal app, signed with Apple Developer ID. Apple notarization is in progress.

### Windows

Unzip and open Comark-Windows.exe. Run the startup self-check first: it verifies Wi-Fi, Bonjour, firewall rules, and display capture, and can request UAC permission to repair Comark firewall rules. Then click Start advertisement and allow the private-network firewall prompt. On iPad, open Connect computer, press Rediscover, select the PC, and enter its six-digit code. Keep both devices on the same LAN.

Windows supports direct iPad pairing, display selection, screenshot capture, and single or batch image delivery to the clipboard. The executable is unsigned, so SmartScreen may ask before opening it.

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
