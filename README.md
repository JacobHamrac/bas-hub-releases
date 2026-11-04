<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub: one app for controls field work. Programmer+, Network+, Reports+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9"><img src="https://img.shields.io/badge/current_release-0.9.9-FF7A29?style=flat-square" alt="Current release: 0.9.9"></a>
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

This repository is the download shelf: it carries the release downloads (the current release is 0.9.9) and this gateway page. It contains no source code, and it never will: BAS Hub is proprietary software.

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
      <sub>The reporting studio: 60 report subjects, fed by vendor files and by live subjects handed over from Network+ and Programmer+; built, previewed, edited, and exported in one place. PDF, XLSX, CSV, TXT out.</sub>
    </td>
    <td width="20%" align="center">
      <img src="assets/icon-copilot.png" alt="Copilot icon" width="72"><br>
      <strong>BAS Copilot</strong> <em>(optional)</em><br>
      <sub>An assistant that runs entirely on your computer. If you don't install it, there is no chat surface anywhere in BAS Hub.</sub>
    </td>
  </tr>
</table>

## Current release: 0.9.9

> **BAS Hub 0.9.9 is the current release, published as stable.** Separate per-OS packages: download the installer for your OS from the [**0.9.9 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9). 0.9.9 is the fix release for the field session run against 0.9.7 at a live site — nine findings, every one fixed here: a Cancel in the Connect window's Auto-assign flow that did not cancel (it now stops the work, sends nothing further, and closes, in every state); a network picker that was a dead end whenever detection found more than one network (a click now selects, and the selection survives re-renders); a Points tab that sat silent when it could not read (it now states what is missing, makes the attempt where an address exists, and reports the outcome — every attempt logged, every failure filed); device pages rebuilt from running text into a summary band and structured sections; every popup in the suite grabbable and movable, with Escape meaning Cancel in all twenty-two dialogs that gained it; and every internal working reference purged from the shipped text, verified by an exhaustive sweep at zero hits. The Mapper is navigable: double-click a device to open its page, right-click for evidence-gated options. Proven on the shipped build in the test rig (full battery plus the fix-specific gates), and installed and verified on a real Windows machine (269 files, checksum-exact), with the device pages and the points honesty path exercised in the running app; two re-checks on that machine — the Connect window's rebuilt chrome and the Mapper's new interactions — are carried openly in the release notes as still outstanding. Points against real field firmware remains unproven and is named as such. A Windows ARM64 package rides in the same release as a candidate build; it has not been verified on ARM64 hardware. The in-app update check reads the latest stable release, so an installed 0.9.7, 0.9.6, 0.9.5, 0.9.4, 0.9.3 or 0.9.2 is offered 0.9.9 by the app itself; the hop from an installed 0.9.3 or 0.9.4 still goes through the standalone Setup below. Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

| File | Size (bytes) | SHA-256 |
| --- | ---: | --- |
| BAS-Hub-Setup-Windows-x64.exe | 175,065,993 | `2b5c9c4cc5487f15f743482f84ad32b1aa700e03c28f8e88e41b39ccf0deaba0` |
| BAS-Hub-Setup-Linux-x64 | 175,893,518 | `ab682759605afe7ee33d0d59db8e7b820ed0cca9f60a26a28f34554545981688` |
| BAS-Hub-Setup-Windows-ARM64.exe (candidate) | 172,374,939 | `0d148dea5793599ecb9f5ff236ffdeb8e3fef899fbebf06b17eabca245741f94` |
| BAS-Hub-User-Guide-0.9.9.pdf | 2,803,681 | `3bc588b64690051750891ffc6b5d77ab0fd0b1754f0bb2aa5c2bd054045120fd` |
| SBOM.json | 14,987 | `f1e5f1cc973774cec40f3d23f2802fba1c2c5c3dcfdb8c21935e408708bf62c` |

**Download & install**

1. Open the [**0.9.9 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9) and download the installer for your OS: **`BAS-Hub-Setup-Windows-x64.exe`** (Windows) or **`BAS-Hub-Setup-Linux-x64`** (Linux): each is one self-contained file, with `SBOM.json` and the User Guide (PDF) beside it in the download set.
2. Run the installer. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture, its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference (requirements, silent-deployment switches, and exit codes) is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
