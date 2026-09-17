# Comark — Downloads

Capture on Mac or Windows. Annotate on iPad. Copy your feedback back.

This public repository contains product information and binaries only. All application source code remains private. Downloading a published release requires no GitHub sign-in.

[Website](https://comark.1491563001.workers.dev) · [All releases](https://github.com/Joseph-Jin/Comark-Downloads/releases)

## Desktop previews

| Platform | Download | Requirements |
| --- | --- | --- |
| Mac 0.2.2 | [Comark-Mac.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v0.2.2/Comark-Mac.zip) | macOS 14+, Apple silicon or Intel |
| Windows 0.2.3 | [Comark-Windows.zip](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v0.2.3-windows/Comark-Windows.zip) | Windows x64; no Python installation needed |
| Checksums | [Mac](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v0.2.2/SHA256SUMS.txt) · [Windows](https://github.com/Joseph-Jin/Comark-Downloads/releases/download/v0.2.3-windows/SHA256SUMS.txt) | Verify each ZIP file |

Both desktop companions require an iPad with Comark installed. iPad 0.2.3 (9) has been uploaded to App Store Connect; TestFlight installation requires an invitation and completion of Apple processing. A public App Store download is not available yet.

### Mac

Unzip and move ComarkMac.app to Applications. Open it and allow screen recording when asked, then pair using its six-digit code. The download above remains the older 0.2.2 preview, which has not been notarized and may be blocked by macOS.

**Mac 0.2.3 is awaiting Apple notarization.** Its Developer ID signing is complete, but the new package has not replaced the old download. The upcoming release removes the development-keychain dependency.

### Windows

Unzip and open Comark-Windows.exe. Click Start advertisement and allow the private-network firewall prompt. On iPad, open Connect computer, press Rediscover, select the PC and enter its six-digit code. Keep both devices on the same LAN.

Windows supports direct iPad pairing, display selection, screenshot capture, and single or multiple image delivery to the clipboard. The executable is unsigned, so Windows may ask before opening it.

### What's changed

- The updated iPad beta offers nearby-computer refresh while connected.
- Offline devices leave the list after discovery/liveness checks and can reappear when back online.
- Windows discovery recovers after network changes and rejects duplicate listeners.

## 中文说明

本仓库仅公开产品说明与下载文件，应用源码保持私有。下载无需 GitHub 账号。

- 电脑端必须搭配已安装 Comark 的 iPad 使用。iPad 0.2.3（9）已提交 App Store Connect，需在 Apple 处理完成后通过 TestFlight 邀请安装，暂未公开上架。
- **Mac 0.2.3 正在等待 Apple 公证**，下载暂时保留尚未公证的旧版 0.2.2。支持 macOS 14 及以上、Apple 芯片和 Intel。
- Windows 已更新至 0.2.3，压缩包包含 EXE 和说明。启动广播后，iPad 可以在同一局域网发现并直接连接；支持选屏、截图和批量回传剪贴板。
- iPad 的连接页可重新发现电脑；离线设备会在扫描或连通性检查后移除。

Copyright © 2026 Joseph-Jin. All rights reserved. No open-source license is granted for the applications by this repository.
