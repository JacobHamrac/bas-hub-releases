<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub: one app for controls field work. Programmer+, Network+, Reports+, TBC+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter6"><img src="https://img.shields.io/badge/current_release-0.9.9-FF7A29?style=flat-square" alt="Current release: 0.9.9"></a>
  <img src="https://img.shields.io/badge/platform-Windows_x64-2E2F34?style=flat-square" alt="Platform: Windows x64">
  <img src="https://img.shields.io/badge/modules-5-2EC5B6?style=flat-square" alt="Five modules: Programmer+, Network+, Reports+, TBC+, BAS Copilot">
  <img src="https://img.shields.io/badge/telemetry-none-2EC5B6?style=flat-square" alt="No telemetry">
  <img src="https://img.shields.io/badge/license-Proprietary-17181A?style=flat-square" alt="License: proprietary">
</p>

---

## The full product site lives at **[bas-hub-app.github.io](https://bas-hub-app.github.io/)**

Screenshots, the demo, module tours, install reference, FAQ, and every release's notes, the complete BAS Hub site:

<p align="center">
  <a href="https://bas-hub-app.github.io/"><strong>→ bas-hub-app.github.io</strong></a>
</p>

This repository is the download shelf: it carries the release downloads (the current release is 0.9.9, iteration 6) and this gateway page. It contains no source code, and it never will: BAS Hub is proprietary software.

---

**BAS Hub** is a desktop suite for building-automation controls work. Instead of separate tools (one for programming, one for discovery, one for captures, one for the terminal, a spreadsheet for the records), BAS Hub is one app whose modules are separate tools under one roof: each module carries its own discovery, its own settings and its own help, and a write to a live controller goes through the same safety path every time. Everything the modules save lives in one file system on your laptop, organised by site — open a site and everything for that site is together, whichever module made it — and nothing leaves it unless you send it.

## The modules

<table>
  <tr>
    <td width="16%" align="center">
      <img src="assets/icon-hub.png" alt="Hub icon" width="72"><br>
      <strong>The Hub</strong><br>
      <sub>The Launch Pad: the home screen and launcher. Your modules as tiles, your own categories of shortcuts to the tools you already use, and the Module Manager.</sub>
    </td>
    <td width="16%" align="center">
      <img src="assets/icon-programmer.png" alt="Programmer+ icon" width="72"><br>
      <strong>Programmer+</strong><br>
      <sub>The PPCL workbench: editor, block builder, simulator and debugger, point database, and code library.</sub>
    </td>
    <td width="16%" align="center">
      <img src="assets/icon-network.png" alt="Network+ icon" width="72"><br>
      <strong>Network+</strong><br>
      <sub>The network workbench: scan a network into a temporary network, open any device on its own page, snapshot and back up, and run batch work across devices.</sub>
    </td>
    <td width="16%" align="center">
      <span style="font-size:26px;font-weight:700;">R+</span><br>
      <strong>Reports+</strong><br>
      <sub>The reporting studio: 60 report subjects, fed by vendor files and by the shared file system's saved networks; built, previewed, edited, and exported in one place. PDF, XLSX, CSV, TXT out.</sub>
    </td>
    <td width="16%" align="center">
      <span style="font-size:26px;font-weight:700;">✓</span><br>
      <strong>TBC+</strong><br>
      <sub>Automated preventive-maintenance testing: planned, gated PM visits across many devices, with as-found and as-left reporting.</sub>
    </td>
    <td width="16%" align="center">
      <img src="assets/icon-copilot.png" alt="Copilot icon" width="72"><br>
      <strong>BAS Copilot</strong> <em>(optional)</em><br>
      <sub>An assistant that runs entirely on your computer. If you don't install it, there is no chat surface anywhere in BAS Hub.</sub>
    </td>
  </tr>
</table>

## Current release: 0.9.9 — iteration 6

> **BAS Hub 0.9.9, iteration 6 (build iter6, 2026-11-19), is the current build of the current release.** Separate per-OS packages: download the installer for your OS from the [**0.9.9 iteration 6 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter6). Iteration 6 is the Launch Pad build: BAS Hub opens on a tile home — installed modules in a protected section, your own shortcut categories below — and every module is now its own separate tool with its own discovery, settings and help, over one shared file system organised by site. The redesigned pages land (the scan with its detail in the Jobs tray and plain labelled counts, the device pages, live trends with per-series lanes and a leave guard, the staged schedules editor, the connect faces, the console's capability states). TBC+ now reads the point list from real devices that answer discovery but refuse a whole-list read, by reading it in parts, and plans on what it read. The one high-severity dependency advisory the suite carried (GHSA-xrw6-gwf8-vvr9) is fixed, and the shipped bill of materials shows no vulnerable dependency. **Stated plainly: this build has not been installed or driven on the owner's Windows laptop.** Its gate suites pass in full and its shipped payloads are probed on all three platforms; TBC+ commanding remains proven on the test rig only. Still open, named in the release notes: schedule and trend writes against real field firmware (unproven; BACnet constructed-type wire encoding not built), BACnet/SC against a real system, the P1 hardware retest, the VAV03 / FPB-4-1-7 / VAV15 object-list dialect, two connect-failure faces not built, INS2-33, INS2-48, INS2-53, DELTA-01…04, DELTA-06, DELTA-07, F-22, F-23, and the `]]` report-title defect. A Windows ARM64 package rides in the same release as a candidate build; it has not been verified on ARM64 hardware. The in-app update check reads the latest stable release, so earlier installed builds are offered this one by the app itself. Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

| File | Size (bytes) | SHA-256 |
| --- | ---: | --- |
| BAS-Hub-Setup-Windows-x64.exe | 175,269,811 | `968654311625695a9f586ee386fbd4f33701ab2b254a16b0e9dae54f0a7c927c` |
| BAS-Hub-Setup-Linux-x64 | 176,095,800 | `0639fe2b92ea6ba28f03592fbbec263c453a62e0003b83c91c744bc9044c06de` |
| BAS-Hub-Setup-Windows-ARM64.exe (candidate) | 172,582,853 | `980c28083ac66186f8ad1e9cd5ccb99d470dd0298fd8168ea9e06b1576fa0d39` |
| BAS-Hub-User-Guide-0.9.9.pdf | 2,803,681 | `3bc588b64690051750891ffc6b5d77ab0fd0b1754f0bb2aa5c2bd054045120fd` |
| SBOM.json | 17,287 | `93a8cdd66231060daad05425bde64ab71d87293d6fdbd5e4816ca82b8b58531f` |

**Download & install**

1. Open the [**0.9.9 iteration 6 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter6) and download the installer for your OS: **`BAS-Hub-Setup-Windows-x64.exe`** (Windows) or **`BAS-Hub-Setup-Linux-x64`** (Linux): each is one self-contained file, with `SBOM.json` and the User Guide (PDF) beside it in the download set.
2. Run the installer. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture, its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference (requirements, silent-deployment switches, and exit codes) is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
