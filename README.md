<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub: one app for controls field work. Programmer+, Network+, Reports+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.4"><img src="https://img.shields.io/badge/current_release-0.9.4-FF7A29?style=flat-square" alt="Current release: 0.9.4"></a>
  <img src="https://img.shields.io/badge/platform-Windows_x64-2E2F34?style=flat-square" alt="Platform: Windows x64">
  <img src="https://img.shields.io/badge/modules-4-2EC5B6?style=flat-square" alt="Four modules: Programmer+, Network+, Reports+, BAS Copilot">
  <img src="https://img.shields.io/badge/telemetry-none-2EC5B6?style=flat-square" alt="No telemetry">
  <img src="https://img.shields.io/badge/license-Proprietary-17181A?style=flat-square" alt="License: proprietary">
</p>

---

## The full product site lives at **[bas-hub-app.github.io](https://bas-hub-app.github.io/)**

Screenshots, the demo, module tours, install reference, FAQ, and every release's notes, the complete BAS Hub site:

<p align="center">
  <a href="https://bas-hub-app.github.io/"><strong>→ bas-hub-app.github.io</strong></a>
</p>

This repository is the download shelf: it carries the release downloads (the current release is 0.9.4) and this gateway page. It contains no source code, and it never will: BAS Hub is proprietary software.

---

**BAS Hub** is a desktop suite for building-automation controls work. Instead of separate tools (one for programming, one for discovery, one for captures, one for the terminal, a spreadsheet for the records), BAS Hub is one app whose modules share **one device inventory and one backup system**. A device you find in Network+ is the same record everywhere. A write to a live controller goes through the same safety path every time. Your data lives on your laptop, in one folder, and nothing leaves it unless you send it.

## The modules

<table>
  <tr>
    <td width="20%" align="center">
      <img src="assets/icon-hub.png" alt="Hub icon" width="72"><br>
      <strong>The Hub</strong><br>
      <sub>The home screen and launcher. Your modules as tiles, your own categories of shortcuts to the tools you already use, one settings home.</sub>
    </td>
    <td width="20%" align="center">
      <img src="assets/icon-programmer.png" alt="Programmer+ icon" width="72"><br>
      <strong>Programmer+</strong><br>
      <sub>The PPCL workbench: editor, block builder, simulator and debugger, point database, and code library.</sub>
    </td>
    <td width="20%" align="center">
      <img src="assets/icon-network.png" alt="Network+ icon" width="72"><br>
      <strong>Network+</strong><br>
      <sub>The network workbench: scan a network into a temporary network, open any device on its own page, snapshot and back up, and run batch work across devices.</sub>
    </td>
    <td width="20%" align="center">
      <span style="font-size:26px;font-weight:700;">R+</span><br>
      <strong>Reports+</strong><br>
      <sub>The reporting studio: 59 report subjects, fed by vendor files and by live subjects handed over from Network+ and Programmer+; built, previewed, edited, and exported in one place. PDF, XLSX, CSV, TXT out.</sub>
    </td>
    <td width="20%" align="center">
      <img src="assets/icon-copilot.png" alt="BAS Copilot icon" width="72"><br>
      <strong>BAS Copilot</strong> <em>(optional)</em><br>
      <sub>An assistant that runs entirely on your computer. If you don't install it, there is no chat surface anywhere in BAS Hub.</sub>
    </td>
  </tr>
</table>

## Current release: 0.9.4

> **BAS Hub 0.9.4 is the current release, published as stable.** It is the first BAS Hub release published as a stable (non-beta) release: 1.0.0 remains reserved for the first release proven end-to-end in the field. Separate per-OS packages: download the installer for your OS from the [**0.9.4 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.4). Tested on Linux; the Windows package's payload is verified, and its Windows install proof is the owner pass. A Windows ARM64 package rides in the same release as a candidate build; it has not been verified on ARM64 hardware. The in-app update check reads the latest stable release, so an installed 0.9.3 or 0.9.2 is offered 0.9.4 by the app itself. One defect, found on release day: the in-app download step in 0.9.3 and 0.9.4 crashes as the download begins, so for this hop install from the standalone Setup below; the crash changes nothing on the computer it runs on. Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

| File | Size (bytes) | SHA-256 |
| --- | ---: | --- |
| BAS-Hub-Setup-Windows-x64.exe | 185,844,105 | `29d6d5bc86fde9b650e3b74d9289b411b17238e2c93dc85d74e5222ba6f3a280` |
| BAS-Hub-Setup-Linux-x64 | 186,670,094 | `fb236d26152a8cec4e90734b75e1df98f8a9cb57fd9c306538f2944ad7e112a0` |
| BAS-Hub-Setup-Windows-ARM64.exe (candidate) | 183,157,147 | `dd96ccb82c534f3174f812414f4e69ee4775d734f920ee94c2dc530719802cc2` |
| BAS-Hub-User-Guide-0.9.4.pdf | 2,543,178 | `ab0c1673a8452d1d6277b369ce2c8b0aa64440ec2ed9b7726dfa6750b325df8c` |
| SBOM.json | 13,344 | `cc5774782817489c2022a37663e5b807fd69161b6ac685524fdfe32e0003814b` |

**Download & install**

1. Open the [**0.9.4 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.4) and download the installer for your OS: **`BAS-Hub-Setup-Windows-x64.exe`** (Windows) or **`BAS-Hub-Setup-Linux-x64`** (Linux): each is one self-contained file, with `SBOM.json` and the User Guide (PDF) beside it in the download set.
2. Run the installer. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture, its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference (requirements, silent-deployment switches, and exit codes) is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
