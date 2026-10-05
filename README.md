<p align="center">
  <img src="assets/banner.svg" alt="Heldo OS" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/STATUS-IN%20DEVELOPMENT-2563eb?style=for-the-badge&labelColor=0d1424" alt="Status">
  <img src="https://img.shields.io/badge/PLATFORM-LINUX-2563eb?style=for-the-badge&logo=linux&logoColor=white&labelColor=0d1424" alt="Platform">
  <img src="https://img.shields.io/badge/SECURITY-FIRST-14b8a6?style=for-the-badge&logo=apparmor&logoColor=white&labelColor=0d1424" alt="Security">
  <img src="https://img.shields.io/badge/LICENSE-TBD-6e7781?style=for-the-badge&labelColor=0d1424" alt="License">
</p>

<p align="center">
  <b>Control your system. Understand what is happening. Recover when something goes wrong.</b>
</p>

<p align="center">
  <a href="#overview"><b>Overview</b></a> &nbsp;•&nbsp;
  <a href="#core-capabilities"><b>Capabilities</b></a> &nbsp;•&nbsp;
  <a href="#architecture"><b>Architecture</b></a> &nbsp;•&nbsp;
  <a href="#screenshots"><b>Screenshots</b></a> &nbsp;•&nbsp;
  <a href="#roadmap"><b>Roadmap</b></a> &nbsp;•&nbsp;
  <a href="#contributing"><b>Contributing</b></a>
</p>

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Overview

**Heldo OS** is a Linux-based operating system that unifies **system protection**, **recovery**, **isolated development environments**, and **AI-assisted troubleshooting** in a single desktop.

Most operating systems make it easy to change the system and hard to understand or undo those changes. Heldo OS is built on the opposite principle: **every sensitive change should be visible, controllable, and reversible.**

| | Principle | What it means |
|:-:|:--|:--|
| 🔐 | **Security** | Protection is part of the base system, not an add-on. |
| 🎛️ | **Control** | The user decides what is allowed to change the system. |
| 🔍 | **Transparency** | System activity is visible and explained. |
| 📦 | **Isolation** | Development workloads run apart from the host. |
| ⏪ | **Recoverability** | Unwanted changes can be reversed. |

> [!NOTE]
> Heldo OS is under active development. Components are at different stages of maturity. See [Project Status](#project-status).

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Core Capabilities

<p align="center">
  <img src="assets/features.svg" alt="Heldo OS core capabilities: Change Firewall, Time Machine, Recovery, AI Pilot, Project Bubbles, Heldo Software" width="900">
</p>

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
- [ ] Change Firewall: policy engine and approval prompts
- [ ] Time Machine: recovery points and rollback
- [ ] Recovery: boot and configuration repair environment
- [ ] Project Bubbles: initial set of isolated environments
- [ ] Heldo Software: unified install and update experience
- [ ] AI Pilot: assisted diagnostics with user approval
- [ ] First public ISO release

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

## Getting Started

Installation images and instructions will be published with the first public release.
Watch this repository (**Watch › Custom › Releases**) to be notified.

## Contributing

Bug reports, feature ideas, and feedback are welcome.

1. Fork the repository
2. Create a branch: `git checkout -b feature/short-description`
3. Commit your changes with a clear message
4. Open a pull request describing the change

For questions or proposals, [open an issue](../../issues).

## Security

If you discover a security vulnerability, please report it privately to the maintainer instead of opening a public issue.

## License

A license has not yet been selected. Until one is added, all rights are reserved by the author.

<p align="center"><img src="assets/divider.svg" width="100%" alt=""></p>

<p align="center">
  <sub><b>HELDO OS</b> &nbsp;·&nbsp; Security &nbsp;·&nbsp; Control &nbsp;·&nbsp; Recovery</sub>
</p>
