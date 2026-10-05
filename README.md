<p align="center">
  <img src="assets/Heldo OS_logo.png" alt="Heldo OS" width="60%">
</p>

<h3 align="center">A Linux desktop where every sensitive change is visible, controllable, and reversible.</h3>

<p align="center">
  <img src="https://img.shields.io/badge/STATUS-IN%20DEVELOPMENT-2563eb?style=for-the-badge&labelColor=0d1424" alt="Status">
  <img src="https://img.shields.io/badge/PLATFORM-LINUX-2563eb?style=for-the-badge&logo=linux&logoColor=white&labelColor=0d1424" alt="Platform">
  <img src="https://img.shields.io/badge/SECURITY-FIRST-14b8a6?style=for-the-badge&logo=apparmor&logoColor=white&labelColor=0d1424" alt="Security">
  <img src="https://img.shields.io/badge/LICENSE-TBD-6e7781?style=for-the-badge&labelColor=0d1424" alt="License">
</p>

<p align="center">
  <a href="#why-heldo-os"><b>Why</b></a> &nbsp;•&nbsp;
  <a href="#core-capabilities"><b>Capabilities</b></a> &nbsp;•&nbsp;
  <a href="#how-it-works"><b>How it works</b></a> &nbsp;•&nbsp;
  <a href="#architecture"><b>Architecture</b></a> &nbsp;•&nbsp;
  <a href="#screenshots"><b>Screenshots</b></a> &nbsp;•&nbsp;
  <a href="#project-status"><b>Status</b></a> &nbsp;•&nbsp;
  <a href="#roadmap"><b>Roadmap</b></a> &nbsp;•&nbsp;
  <a href="#faq"><b>FAQ</b></a> &nbsp;•&nbsp;
  <a href="#contributing"><b>Contributing</b></a>
</p>

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Overview

**Heldo OS** is a Linux-based operating system that brings **system protection**, **recovery**, **isolated development environments**, and **AI-assisted troubleshooting** together in one desktop.

Most operating systems make it easy to change the system and hard to understand or undo those changes. Heldo OS is built on the opposite principle:

> **Control your system. Understand what is happening. Recover when something goes wrong.**

> [!NOTE]
> Heldo OS is under active development. Components are at different stages of maturity. See [Project Status](#project-status).

## Why Heldo OS

Developers and administrators routinely run into the same problems:

- A package update or script silently changes system configuration, and nobody knows what changed.
- Project dependencies pollute the host until the machine becomes fragile.
- When something breaks, the fix is a late-night search through logs and forums.
- Rolling back means a full reinstall, or hoping a backup exists.

Heldo OS addresses these at the system level instead of leaving them to add-on tools.

| | Principle | What it means |
|:-:|:--|:--|
| 🔐 | **Security** | Protection is part of the base system, not an add-on. |
| 🎛️ | **Control** | You decide what is allowed to change the system. |
| 🔍 | **Transparency** | System activity is visible and explained in plain language. |
| 📦 | **Isolation** | Development workloads run apart from the host. |
| ⏪ | **Recoverability** | Unwanted changes can be reversed. |

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Core Capabilities

<p align="center">
  <img src="assets/features.svg" alt="Heldo OS core capabilities: Change Firewall, Time Machine, Recovery, AI Pilot, Project Bubbles, Heldo Software" width="900">
</p>

| Capability | What it does |
|:--|:--|
| 🛡️ **Change Firewall** | Watches sensitive system changes and asks for your approval before they apply, so nothing modifies your system unnoticed. |
| ⏪ **Time Machine** | Creates recovery points and lets you roll the system back to a known-good state. |
| 🧰 **Recovery** | A dedicated environment for repairing boot and configuration problems when the system will not start normally. |
| 🤖 **AI Pilot** | Assists with diagnostics and troubleshooting. It explains what is happening and proposes fixes, but acts only with your approval. |
| 🫧 **Project Bubbles** | Isolated development environments that keep project dependencies and workloads away from the host system. |
| 📦 **Heldo Software** | A unified experience for installing and updating software. |

<details>
<summary><b>Project Bubbles: supported environments</b></summary>
<br>

| Languages and runtimes | Platforms and workloads |
|:--|:--|
| Python | Cloud Development |
| Web Development | DevOps |
| Java | Kubernetes |
| C / C++ | Containers |
| Go | AI / ML |

</details>

<details>
<summary><b>Security foundation</b></summary>
<br>

| Domain | Controls |
|:--|:--|
| Access control | AppArmor, privilege management |
| Network | Firewall management |
| Auditing | System auditing |
| Isolation | Application isolation, sandboxed workloads |
| Maintenance | Security updates, secure system configuration |

</details>

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## How It Works

The three core ideas work together as a loop: **review → protect → recover.**

```mermaid
flowchart LR
    A[Something tries to change the system] --> B{Change Firewall}
    B -- Approved --> C[Recovery point created]
    C --> D[Change applied]
    B -- Denied --> E[System unchanged]
    D --> F{Something went wrong?}
    F -- Yes --> G[Roll back with Time Machine]
    F -- Hard failure --> H[Repair in Recovery environment]
    F -- Unsure why --> I[Ask AI Pilot to diagnose]
    G --> J[Known-good system]
    H --> J
    I --> G
```

1. **Review.** Sensitive changes surface as clear prompts instead of happening silently.
2. **Protect.** Approved changes are backed by recovery points.
3. **Recover.** If something breaks, you can roll back, repair, or ask AI Pilot to help find the cause.

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Architecture

Heldo OS combines a customized desktop and a set of Heldo tools on top of a standard Linux core, organized into three pillars. AI Pilot assists across all of them.

<p align="center">
  <img src="assets/architecture.svg" alt="Heldo OS architecture" width="900">
</p>

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Screenshots

<p align="center">
  <img src="assets/desktop.png" alt="Heldo OS desktop" width="900"><br>
  <sub><b>Desktop</b></sub>
</p>

<p align="center">
  <img src="assets/tools.png" alt="Heldo OS application center" width="900"><br>
  <sub><b>Application Center</b></sub>
</p>

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Who It's For

<table align="center">
  <tr>
    <td align="center" width="25%"><b>Software<br>Developers</b></td>
    <td align="center" width="25%"><b>Cloud<br>Engineers</b></td>
    <td align="center" width="25%"><b>DevOps<br>Engineers</b></td>
    <td align="center" width="25%"><b>SRE<br>Engineers</b></td>
  </tr>
  <tr>
    <td align="center"><b>System<br>Administrators</b></td>
    <td align="center"><b>Security<br>Engineers</b></td>
    <td align="center"><b>AI / ML<br>Engineers</b></td>
    <td align="center"><b>Linux<br>Enthusiasts</b></td>
  </tr>
</table>

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Project Status

| Component | Stage |
|:--|:--|
| Core system design | ![Complete](https://img.shields.io/badge/-Complete-16a34a?style=flat-square) |
| Custom desktop | ![Complete](https://img.shields.io/badge/-Complete-16a34a?style=flat-square) |
| Change Firewall | ![In development](https://img.shields.io/badge/-In%20development-2563eb?style=flat-square) |
| Time Machine | ![In development](https://img.shields.io/badge/-In%20development-2563eb?style=flat-square) |
| Recovery environment | ![In development](https://img.shields.io/badge/-In%20development-2563eb?style=flat-square) |
| Project Bubbles | ![In development](https://img.shields.io/badge/-In%20development-2563eb?style=flat-square) |
| Heldo Software | ![In development](https://img.shields.io/badge/-In%20development-2563eb?style=flat-square) |
| AI Pilot | ![Planned](https://img.shields.io/badge/-Planned-6e7781?style=flat-square) |

## Roadmap

- [x] Core concept and system design
- [x] Custom desktop experience
- [ ] **Change Firewall:** policy engine and approval prompts
- [ ] **Time Machine:** recovery points and rollback
- [ ] **Recovery:** boot and configuration repair environment
- [ ] **Project Bubbles:** initial set of isolated environments
- [ ] **Heldo Software:** unified install and update experience
- [ ] **AI Pilot:** assisted diagnostics with user approval
- [ ] **First public ISO release**

Have a feature idea? [Open an issue](../../issues) and tell us what you need.

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## FAQ

<details>
<summary><b>Is Heldo OS a new Linux distribution?</b></summary>
<br>
Heldo OS is a Linux-based operating system: a customized desktop and a set of Heldo tools built on a standard Linux core.
</details>

<details>
<summary><b>Can I install it today?</b></summary>
<br>
Not yet. Installation images will be published with the first public release. Watch this repository to be notified.
</details>

<details>
<summary><b>Will AI Pilot change my system on its own?</b></summary>
<br>
No. AI Pilot is designed for assisted diagnostics with user approval. You stay in control of what is applied.
</details>

<details>
<summary><b>Is it free and open source?</b></summary>
<br>
A license has not been selected yet. See [License](#license).
</details>

## Getting Started

Installation images and instructions will be published with the first public release.

**Stay updated:** click **Watch › Custom › Releases** at the top of this repository, and **⭐ star** the project to show support.

## Contributing

Bug reports, feature ideas, and feedback are welcome.

1. Fork the repository
2. Create a branch: `git checkout -b feature/short-description`
3. Commit your changes with a clear message
4. Open a pull request describing the change

For questions or proposals, [open an issue](../../issues).

## Security

If you discover a security vulnerability, please report it **privately** to the maintainer instead of opening a public issue.

## License

A license has not yet been selected. Until one is added, all rights are reserved by the author.

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

<p align="center">
  <sub><b>HELDO OS</b> &nbsp;·&nbsp; Security &nbsp;·&nbsp; Control &nbsp;·&nbsp; Recovery</sub>
</p>
