# FORGE releases

Official downloads for FORGE products: installers, device firmware and release notes.
Hardware and AI software, built to work together.

Source code is not published here.

---

## Desk companion for Claude Code (working name: Fennec)

A small desk device that shows, at a glance, what your Claude Code sessions are doing and
how much of your usage limit is left.

> **Beta.** Versions 0.9.x are early releases for testers: expect rough edges, and please
> report what you find. Version 1.0.0 will be the first full release.

### Download

Open the newest **`fennec-vX.Y.Z`** release under
[Releases](https://github.com/AbdelhediMed05/FORGE-releases/releases) and download
**`FennecSetup.exe`**.

> The `channel/` folder in this repository is what the app reads to find updates. It is
> not a download.

### Requirements

- Windows 10 or 11, 64-bit
- Claude Code 2.1.157 or later
- The device, connected with a USB-C data cable

### Install

1. Run `FennecSetup.exe`. Windows may show a SmartScreen warning because the installer is
   not code-signed yet: choose **More info**, then **Run anyway**.
2. Plug in the device. Fennec finds it on its own.
3. Restart Claude Code once, so it picks up Fennec's hooks.

Installing a newer version over an installed one updates it in place and keeps your
settings.

### Updates

- Fennec checks for a new version at most once a day while it runs. You can turn that off
  in **Settings → Check for updates automatically**, and check by hand with **Check now**.
- Nothing is downloaded until you click **Update**.
- Device firmware updates come inside app updates. When one is available, the
  **Hardware** tab offers it; keep the device plugged in for about a minute.

### Privacy

- Everything runs on your own computer. There is no account and no telemetry.
- Fennec never opens your Claude Code conversations.
- It connects to the internet for exactly two things: checking this page for updates, and
  reading your own usage figure from Anthropic with the credentials Claude Code already
  keeps on your computer.

### Security

- Every release is signed. The app refuses an update that is not signed by FORGE, and checks
  the installer's size and checksum before running it.
- The device accepts only firmware signed by FORGE.

### Uninstall

**Settings → Apps → Fennec → Uninstall.** You are asked whether to keep your settings and
usage history, in case you reinstall later.

### Report a problem

Open an [issue](https://github.com/AbdelhediMed05/FORGE-releases/issues) with your
Fennec version (shown in Settings) and what happened. Please do not paste credentials,
tokens or the contents of your Claude Code conversations.
