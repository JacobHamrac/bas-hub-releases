<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub: one app for controls field work. Programmer+, Network+, Reports+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter3"><img src="https://img.shields.io/badge/current_release-0.9.9-FF7A29?style=flat-square" alt="Current release: 0.9.9"></a>
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

This repository is the download shelf: it carries the release downloads (the current release is 0.9.9, iteration 3) and this gateway page. It contains no source code, and it never will: BAS Hub is proprietary software.

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

## Current release: 0.9.9 — iteration 3

> **BAS Hub 0.9.9, iteration 3 (build iter3, 2026-11-10), is the current build of the current release.** Separate per-OS packages: download the installer for your OS from the [**0.9.9 iteration 3 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter3). Iteration 3 is the field-regression build: Network+ rolls to 2.6.0 — every transport is back in the Connection Wizard (ten, including Siemens P1), the wizard's ten Manual forms are rebuilt on the approved layout system and re-inspected to standard, the BACnet object-list read recovers per-index and files the device's reply bytes when it cannot, every P1 census files a diagnostics record either way, and the log drawer narrates the touched surfaces in plain words. Still open, named in the release notes by ID: INS2-33, INS2-48, INS2-53, DELTA-01…04, DELTA-06, DELTA-07, F-22, F-23, the `]]` report-title defect, one dependency advisory under review (GHSA-xrw6-gwf8-vvr9), the P1 hardware retest (direction handling is hypothesis-grade until then), defect 4's exact device byte dialect (one Wireshark capture or one iteration-3 failure file closes it), and Points against real field firmware, which remains unproven. Proven on the shipped build in the test rig (defect gate 139/0, full battery with zero regressions against the iteration-2 baseline, fifteen named gates green) and installed and verified on a real Windows machine (269 files; Network+ 2.6.0 live in the running app, no-model choice and module set preserved); on that machine the wizard's card selection by pointer, its physical drag, the transport forms and the resize re-clamp were not driven — the remote bridge's synthetic pointer input does not actuate the wizard window — and are carried openly. A Windows ARM64 package rides in the same release as a candidate build; it has not been verified on ARM64 hardware. The in-app update check reads the latest stable release, so earlier installed builds are offered this one by the app itself; the hop from an installed 0.9.3 or 0.9.4 still goes through the standalone Setup below. Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

| File | Size (bytes) | SHA-256 |
| --- | ---: | --- |
| BAS-Hub-Setup-Windows-x64.exe | 175,156,105 | `9cc5ed89ffe98ad70eadb1eb3b935381eb6358848668ddb9a8908e44ca5cfe73` |
| BAS-Hub-Setup-Linux-x64 | 175,982,606 | `d73045a3cea1611d3b0fd4d570e51928a327741d7f4e90caadd6026aaeff6dd1` |
| BAS-Hub-Setup-Windows-ARM64.exe (candidate) | 172,469,147 | `4a2a078ab7e0f7906a318058e0d52458e4e9c40668f64ecfb7715619d66a20ce` |
| BAS-Hub-User-Guide-0.9.9.pdf | 2,803,681 | `3bc588b64690051750891ffc6b5d77ab0fd0b1754f0bb2aa5c2bd054045120fd` |
| SBOM.json | 17,888 | `af4b7659d65be55edc1a0d41cf82a99d6f188b6e86c0fee0dfeee9bfbbb25b16` |

**Download & install**

1. Open the [**0.9.9 iteration 3 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter3) and download the installer for your OS: **`BAS-Hub-Setup-Windows-x64.exe`** (Windows) or **`BAS-Hub-Setup-Linux-x64`** (Linux): each is one self-contained file, with `SBOM.json` and the User Guide (PDF) beside it in the download set.
2. Run the installer. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture, its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference (requirements, silent-deployment switches, and exit codes) is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
