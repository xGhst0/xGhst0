<div align="center">

[![HTB CDSA](https://img.shields.io/badge/HTB-Certified_Defensive_Security_Analyst-9FEF00?logo=hackthebox&logoColor=black)](https://academy.hackthebox.com/preview/certifications/htb-certified-defensive-security-analyst)
[![Rust](https://img.shields.io/badge/Rust-B7410E?logo=rust&logoColor=white)](#-intelscribe)
[![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)](#-skyhawk)
[![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-C8102E)](https://attack.mitre.org/)

*offline-first, deterministic, and built for air-gapped environments.*

</div>

---

## About

- 🛡️ Defensive security analyst — SOC monitoring, detection engineering, incident response and reporting
- 🇦🇺 Deep focus on Australian frameworks: **ACSC ISM**, **Essential Eight**, ASD incident categorisation, SOCI & NDB reporting obligations
- 🔧 Daily drivers: **Splunk · Elastic · Sysmon · Volatility · KAPE**
- 🦀 I build compiled, dependency-light tooling in **Rust** and **zero-dependency Node.js** — everything runs fully offline

---

## 📝 IntelScribe

**Offline desktop app that turns structured incident facts into commercial-grade cyber reports.**
Rust · Tauri · Typst — [`xGhst0/intelscribe`](https://github.com/xGhst0/intelscribe) · Apache-2.0

Enter each fact once (hosts, detections, IoCs, timeline, techniques) — IntelScribe generates the executive
summary, numbered detections with SIEM queries, IoC tables, an auto-drawn attack-path map, a kill-chain
timeline, MITRE ATT&CK coverage matrix, auto-derived mitigations, verbatim ACSC ISM control quoting and
CVSS 3.1 scoring, rendered to themed PDF or DOCX. The full **MITRE ATT&CK matrix (697 techniques)** and the
**Australian Government ISM** ship inside the binary — no internet connection at any point.

<img src="assets/intelscribe-app.png" alt="IntelScribe desktop app — live report preview with report checks panel" width="100%">

<p align="center"><sub>The desktop app: structured form, live report linter, and instant themed PDF preview.</sub></p>

| Auto-drawn attack path | ATT&CK coverage matrix | Executive summary |
|:---:|:---:|:---:|
| ![Attack path overview](assets/intelscribe-attack-path.png) | ![ATT&CK coverage matrix](assets/intelscribe-attack-matrix.png) | ![Executive summary](assets/intelscribe-exec-summary.png) |

**18 palettes × 6 procedural cover-art generators — 108 distinct looks, all generated, no stock imagery:**

| Harbour Teal · hexgrid | Midnight Slate · network | Crimson Vector · circuit |
|:---:|:---:|:---:|
| ![Harbour Teal cover](assets/intelscribe-cover-1.png) | ![Midnight Slate cover](assets/intelscribe-cover-2.png) | ![Crimson Vector cover](assets/intelscribe-cover-3.png) |

Also in the box: a live report **linter** (completeness, consistency and sanitisation checks), document
import (`.pdf` / `.docx` / `.doc` / `.txt` → IoCs, hosts, timeline, detections and suggested techniques
extracted automatically), an **evidence vault** with SHA-256 chain-of-custody register, a CVSS 3.1
builder, and a penetration-test report type with a likelihood × consequence risk matrix.

---

## 🦅 SKYHAWK

**Air-gapped investigation-to-report platform for blue-team analyst teams.**
Zero-dependency Node.js · [`xGhst0/skyhawk`](https://github.com/xGhst0/skyhawk) · MIT

Analysts capture findings with full evidence, leads curate, managers sign — and every case produces a
live technical report and a frozen, signed formal report. Runs entirely on `localhost` / your LAN:
no internet, no database, no npm packages. Role-based access (Analyst / Tech Lead / Manager) with
scrypt-hashed credentials, server-side sessions and login rate-limiting. A one-command bundler packs
SKYHAWK plus the Node runtime into a checksum-verified tarball for machines that have never seen the internet.

<img src="assets/skyhawk-dashboard.png" alt="SKYHAWK portfolio dashboard" width="100%">

<p align="center"><sub>Case portfolio: live stats, global search across cases, findings and IoCs.</sub></p>

| Case workspace | Live technical report |
|:---:|:---:|
| ![Case workspace](assets/skyhawk-case.png) | ![Live technical report](assets/skyhawk-report-technical.png) |

---

## Toolbox

**Detection & DFIR**&nbsp;&nbsp;
![Splunk](https://img.shields.io/badge/Splunk-000000?logo=splunk&logoColor=white)
![Elastic](https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=white)
![Sysmon](https://img.shields.io/badge/Sysmon-0078D4?logo=windows&logoColor=white)
![Volatility](https://img.shields.io/badge/Volatility-1B1B1B)
![KAPE](https://img.shields.io/badge/KAPE-4B275F)

**Engineering**&nbsp;&nbsp;
![Rust](https://img.shields.io/badge/Rust-B7410E?logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8D8?logo=tauri&logoColor=black)
![Typst](https://img.shields.io/badge/Typst-239DAD?logo=typst&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?logo=gnubash&logoColor=white)

**Frameworks**&nbsp;&nbsp;
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C8102E)
![ACSC ISM](https://img.shields.io/badge/ACSC-ISM-00205B)
![Essential Eight](https://img.shields.io/badge/ACSC-Essential_Eight-00843D)
![CVSS 3.1](https://img.shields.io/badge/FIRST-CVSS_3.1-555555)

---

<div align="center">

📫 **benjamin.sokimi@gmail.com**

</div>
