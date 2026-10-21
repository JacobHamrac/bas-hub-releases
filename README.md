<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub: one app for controls field work. Programmer+, Network+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.2"><img src="https://img.shields.io/badge/current_release-0.9.2_beta-FF7A29?style=flat-square" alt="Current release: 0.9.2 (Beta)"></a>
  <img src="https://img.shields.io/badge/platform-Windows_x64-2E2F34?style=flat-square" alt="Platform: Windows x64">
  <img src="https://img.shields.io/badge/modules-3-2EC5B6?style=flat-square" alt="Three modules: Programmer+, Network+, BAS Copilot">
  <img src="https://img.shields.io/badge/telemetry-none-2EC5B6?style=flat-square" alt="No telemetry">
  <img src="https://img.shields.io/badge/license-Proprietary-17181A?style=flat-square" alt="License: proprietary">
</p>

---

## The full product site lives at **[bas-hub-app.github.io](https://bas-hub-app.github.io/)**

Screenshots, the demo, module tours, install reference, FAQ, and every release's notes, the complete BAS Hub site:

<p align="center">
  <a href="https://bas-hub-app.github.io/"><strong>→ bas-hub-app.github.io</strong></a>
</p>

This repository is the download shelf: it carries the release downloads (the current release is 0.9.2 (Beta)) and this gateway page. It contains no source code, and it never will: BAS Hub is proprietary software.

---

**BAS Hub** is a desktop suite for building-automation controls work. Instead of separate tools (one for programming, one for discovery, one for captures, one for the terminal, a spreadsheet for the records), BAS Hub is one app whose modules share **one device inventory and one backup system**. A device you find in Network+ is the same record everywhere. A write to a live controller goes through the same safety path every time. Your data lives on your laptop, in one folder, and nothing leaves it unless you send it.

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

## Current release: 0.9.2 (Beta)

> **BAS Hub 0.9.2 is a beta release.** It is published so it can be downloaded and used; it is still being proven in the field, and the first stable release is still to come. Separate per-OS packages: download the installer for your OS from the [**0.9.2 (Beta) release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.2). Tested on Windows. Tested on Linux. The Windows ARM64 package is in preparation and is not published. The in-app update check reads stable releases only, so it does not offer this beta: download it here, or from the [website](https://bas-hub-app.github.io/). Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

| File | Size (bytes) | SHA-256 |
| --- | ---: | --- |
| BAS-Hub-Setup-Windows-x64.exe | 176,302,025 | `04c1ddc84f5fc88602b5406e921a267c79f727388e8eb27c1b154245a864c27d` |
| BAS-Hub-Setup-Linux-x64 | 177,130,062 | `716e6103a9b27d1e6eb21384d1d6a3e77f6226c227297a715dcf66bc1d980500` |
| BAS-Hub-User-Guide-0.9.2.pdf | 3,466,537 | `abc59473ea33dfbb4ae129794e900675350f784d9c841574d43926568e84a855` |
| SBOM.json | 13,018 | `a37d8588367f332eecd08219b8ac8ae34ff65977c81fb7505b498871d760f25e` |

**Download & install**

1. Open the [**0.9.2 (Beta) release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.2) and download the installer for your OS: **`BAS-Hub-Setup-Windows-x64.exe`** (Windows) or **`BAS-Hub-Setup-Linux-x64`** (Linux): each is one self-contained file, with `SBOM.json` and the User Guide (PDF) beside it in the download set.
2. Run the installer. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture, its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference (requirements, silent-deployment switches, and exit codes) is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
