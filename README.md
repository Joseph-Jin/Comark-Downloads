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

Unzip and move ComarkMac.app to Applications. Open it and allow screen recording when asked, then pair using its six-digit code. The download is the macOS universal app, signed with Apple Developer ID. Apple notarization is pending, so macOS may block this build from opening; right-click and choose Open to bypass the first-run prompt.

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

| 平台 | 下载 | 要求 |
| --- | --- | --- |
| Mac 1.0 | [Comark-Mac.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/Comark-Mac.zip) | macOS 14 及以上，Apple 芯片或 Intel |
| Windows 1.0 | [Comark-Windows.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/Comark-Windows.zip) | Windows x64，无需安装 Python |
| 校验值 | [SHA256SUMS.txt](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v1.0/SHA256SUMS.txt) | 用于校验压缩包 |

- 电脑端必须搭配已安装 Comark 的 iPad 使用，无法单独运行。iPad v1.0（Build 24）已上 TestFlight，需通过测试邀请安装，暂未公开上架。
- Mac 版已完成 Developer ID 签名，Apple 公证尚未完成，首次打开可以右键选择「打开」跳过系统提示。
- Windows 版启动后先运行自检，检查 Wi-Fi、Bonjour、防火墙和屏幕采集；防火墙检查失败时点击「修复网络访问」并批准 UAC。安装包未签名，SmartScreen 可能会询问。
- iPad 端默认使用 Apple 端上语音识别，开箱可用；语音笔落笔录音、抬笔转写，并在画面上生成带编号的标记。
- 断网、锁屏或切换 Wi-Fi 后会自动重连上次配对的电脑。

Copyright © 2026 Joseph-Jin. All rights reserved. No open-source license is granted for the applications by this repository.

