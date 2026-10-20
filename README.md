<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub — one app for controls field work. Programmer+, Network+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases"><img src="https://img.shields.io/badge/first_release-0.9.1_in_preparation-FF7A29?style=flat-square" alt="First public release: 0.9.1, in preparation"></a>
  <img src="https://img.shields.io/badge/platform-Windows_x64-2E2F34?style=flat-square" alt="Platform: Windows x64">
  <img src="https://img.shields.io/badge/modules-3-2EC5B6?style=flat-square" alt="Three modules: Programmer+, Network+, BAS Copilot">
  <img src="https://img.shields.io/badge/telemetry-none-2EC5B6?style=flat-square" alt="No telemetry">
  <img src="https://img.shields.io/badge/license-Proprietary-17181A?style=flat-square" alt="License: proprietary">
</p>

---

## The full product site lives at **[bas-hub-app.github.io](https://bas-hub-app.github.io/)**

Screenshots, the demo, module tours, install reference, FAQ, and every release's notes — the complete BAS Hub site:

<p align="center">
  <a href="https://bas-hub-app.github.io/"><strong>→ bas-hub-app.github.io</strong></a>
</p>

This repository is the download shelf: it will carry the release downloads (the first public release is in preparation) and this gateway page. It contains no source code, and it never will — BAS Hub is proprietary software.

---

**BAS Hub** is a desktop suite for building-automation controls work. Instead of a pocketful of separate tools — one for programming, one for discovery, one for captures, one for the terminal, a spreadsheet for the records — BAS Hub is one app whose modules share **one device inventory, one backup system, and one standard of care**. A device you find in Network+ is the same record everywhere. A write to a live controller goes through the same safety path every time. Your data lives on your laptop, in one folder, and nothing leaves it unless you send it.

## The modules

<table>
  <tr>
    <td width="25%" align="center">
      <img src="assets/icon-hub.png" alt="Hub icon" width="72"><br>
      <strong>The Hub</strong><br>
      <sub>The home screen and launcher. Your modules as tiles, your own categories of shortcuts to the tools you already use, one settings home.</sub>
    </td>
    <td width="25%" align="center">
      <img src="assets/icon-programmer.png" alt="Programmer+ icon" width="72"><br>
      <strong>Programmer+</strong><br>
      <sub>The PPCL workbench: editor, block builder, simulator and debugger, point database, and code library.</sub>
    </td>
    <td width="25%" align="center">
      <img src="assets/icon-network.png" alt="Network+ icon" width="72"><br>
      <strong>Network+</strong><br>
      <sub>The network workbench: find devices, look at them, watch traffic, check health, prove changes, talk, and keep records.</sub>
    </td>
    <td width="25%" align="center">
      <img src="assets/icon-copilot.png" alt="BAS Copilot icon" width="72"><br>
      <strong>BAS Copilot</strong> <em>(optional)</em><br>
      <sub>An assistant that runs entirely on your computer. If you don't install it, there is no chat surface anywhere in BAS Hub.</sub>
    </td>
  </tr>
</table>

## First public release — 0.9.1, in preparation

> **No public release exists yet.** The internal first build (0.9.0) never published — it is not downloadable here, and never will be. Windows: tested on Windows. Linux: tested on Linux. The first public release, **0.9.1**, is in preparation. When it lands, this repository carries it as separate Windows and Linux packages, and this page takes its real file names, sizes, and checksums. The suite it will deliver: Programmer+ and Network+ side by side on one home screen, sharing one device inventory; BAS Copilot optional and entirely on-device; updates only when you press the button, verified by checksum and signature before anything is applied. Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

**Download & install — when the first public release lands**

1. Open the [**latest release**](https://github.com/JacobHamrac/bas-hub-releases/releases) and download the package for your OS: **`BAS Hub Setup.exe`** with its **`payload.zip`** and **`payload.sha256`** (Windows), or the Linux package. Keep them together in one folder — the installer needs all three.
2. Double-click **`BAS Hub Setup.exe`**. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture — its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference — requirements, silent-deployment switches, and exit codes — is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
