<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.png">
    <img src="assets/hero-light.png" alt="BAS Hub: one app for controls field work. Programmer+, Network+, Reports+, BAS Copilot." width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter4"><img src="https://img.shields.io/badge/current_release-0.9.9-FF7A29?style=flat-square" alt="Current release: 0.9.9"></a>
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

This repository is the download shelf: it carries the release downloads (the current release is 0.9.9, iteration 4) and this gateway page. It contains no source code, and it never will: BAS Hub is proprietary software.

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

## Current release: 0.9.9 — iteration 4

> **BAS Hub 0.9.9, iteration 4 (build iter4, 2026-11-14), is the current build of the current release.** Separate per-OS packages: download the installer for your OS from the [**0.9.9 iteration 4 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter4). Iteration 4 is the design-march build: Network+ rolls to 2.7.0 — device folders in the tree with no tab strip, the live points table with its Verify check, the Console as its own window that can pin into the Log drawer, Monitor Network Traffic in Raw, Table and Combined views, and the Trends and Schedules rooms with guarded editing. **Stated plainly: this build was published at the owner's direction before its final two verification legs — a driven pass on a real Windows laptop and a fresh independent re-inspection.** The standing blind-inspection verdict on this build line is NOT AT STANDARD, returned against its first candidate; five repair passes followed and their work is gate-proven, battery-clean (6,993 PASS, failures only in named baselines), shipped-artifact-probed, and photographed under an evidence manifest that survived three independent falsification checks — but this build itself has not been re-inspected cold and has not been installed or driven on the laptop, and two laptop proofs remain outstanding by name (the Traffic bundle footbar on the empty state, fixed in product and gate-proven, photograph owed; and the pinned console session on the real machine for this build). Earlier candidates of this same build line proved on that laptop: a live Telnet console session end to end, the pin as a true move, the traffic views collision-free, and the console port field's plain-word refusal of an out-of-range port. Still open, named in the release notes: schedule and trend writes against real field firmware (unproven; BACnet constructed-type wire encoding not built), console sessions against real device consoles (laptop-local peer only), BACnet/SC against a real system, INS2-33, INS2-48, INS2-53, DELTA-01…04, DELTA-06, DELTA-07, F-22, F-23, the `]]` report-title defect, one dependency advisory under review (GHSA-xrw6-gwf8-vvr9), the P1 hardware retest, the VAV03 / FPB-4-1-7 / VAV15 object-list dialect (one Wireshark capture or one iteration-4 failure file closes it), and the wizard's pointer items and resize re-clamp on Windows. A Windows ARM64 package rides in the same release as a candidate build; it has not been verified on ARM64 hardware. The in-app update check reads the latest stable release, so earlier installed builds are offered this one by the app itself; the hop from an installed 0.9.3 or 0.9.4 still goes through the standalone Setup below. Full notes for every build are on the [website's versions page](https://bas-hub-app.github.io/releases.html).

| File | Size (bytes) | SHA-256 |
| --- | ---: | --- |
| BAS-Hub-Setup-Windows-x64.exe | 175,370,121 | `0508c6819e3a1e0da11dbf03c57a5b1544b8205fd3971054833236ec6f4cdc3a` |
| BAS-Hub-Setup-Linux-x64 | 176,194,574 | `c4c599f765e88d04bbb70664ef3cb5c72b6099e498b1bd43c8ced078f53eee15` |
| BAS-Hub-Setup-Windows-ARM64.exe (candidate) | 172,679,067 | `af39555d6cd093adc0186c2705efaa3985e29c4bec4678842893688308e99926` |
| BAS-Hub-User-Guide-0.9.9.pdf | 2,803,681 | `3bc588b64690051750891ffc6b5d77ab0fd0b1754f0bb2aa5c2bd054045120fd` |
| SBOM.json | 17,888 | `af4b7659d65be55edc1a0d41cf82a99d6f188b6e86c0fee0dfeee9bfbbb25b16` |

**Download & install**

1. Open the [**0.9.9 iteration 4 release**](https://github.com/JacobHamrac/bas-hub-releases/releases/tag/v0.9.9-iter4) and download the installer for your OS: **`BAS-Hub-Setup-Windows-x64.exe`** (Windows) or **`BAS-Hub-Setup-Linux-x64`** (Linux): each is one self-contained file, with `SBOM.json` and the User Guide (PDF) beside it in the download set.
2. Run the installer. BAS Hub needs **no administrator rights** and installs for your user account only, in a location you choose.
3. Pick the **complete package**, or just the modules you want. Optional extras: **BAS Copilot** (Setup offers the model sizes this computer can run well) and **Npcap** (the packet-capture driver for Network+ live capture, its own signed installer, the one step that asks for administrator approval).
4. Launch **BAS Hub** from the Start menu or your desktop. Your data lives in `%LOCALAPPDATA%\BAS Hub\data` and is never removed by updates or by uninstalling.

The full install reference (requirements, silent-deployment switches, and exit codes) is on the [website](https://bas-hub-app.github.io/#download).

## License

BAS Hub is **proprietary software**. © 2026. All rights reserved.

This repository contains release downloads and product information only. No source code is published here. Your use of the software is governed by the proprietary terms stated with each release.

<p align="center">BAS Hub is proprietary software · © 2026</p>
