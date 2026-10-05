<div align="center">

<img src="assets/Heldo%20OS_logo.png" alt="Heldo OS" width="140">

<br>

# HELDO OS

**A Linux desktop engineered for security, control, and recovery.**

<br>

![Status](https://img.shields.io/badge/STATUS-IN%20DEVELOPMENT-0b3d91?style=flat-square&labelColor=1b1f24)
![Platform](https://img.shields.io/badge/PLATFORM-LINUX-0b3d91?style=flat-square&labelColor=1b1f24)
![Focus](https://img.shields.io/badge/FOCUS-SECURITY%20%C2%B7%20RECOVERY%20%C2%B7%20DEVELOPMENT-0b3d91?style=flat-square&labelColor=1b1f24)
![License](https://img.shields.io/badge/LICENSE-TBD-6e7781?style=flat-square&labelColor=1b1f24)

<br>

[Overview](#overview) &nbsp;|&nbsp;
[Capabilities](#core-capabilities) &nbsp;|&nbsp;
[Architecture](#architecture) &nbsp;|&nbsp;
[Screenshots](#screenshots) &nbsp;|&nbsp;
[Roadmap](#roadmap) &nbsp;|&nbsp;
[Contributing](#contributing)

</div>

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0b3d91&height=2" width="100%" alt="">

## Overview

Heldo OS is a Linux-based operating system that unifies **system protection**, **recovery**, **isolated development environments**, and **AI-assisted troubleshooting** in a single desktop.

Most operating systems make it easy to change the system and hard to understand or undo those changes. Heldo OS is designed around the opposite principle: every sensitive change should be visible, controllable, and reversible.

> **Control your system. Understand what is happening. Recover when something goes wrong.**

> [!NOTE]
> Heldo OS is under active development. Components are at different stages of maturity; see [Project Status](#project-status) for details.

<br>

## Design Principles

| Principle | Description |
|:--|:--|
| **Security** | Protection is part of the base system, not an optional add-on. |
| **Control** | The user decides what is allowed to change the system. |
| **Transparency** | System activity is visible and explained. |
| **Isolation** | Development workloads run apart from the host. |
| **Recoverability** | Unwanted changes can be reversed. |

<br>

## Core Capabilities

### Heldo Change Firewall

Policy-based control over sensitive system modifications made by applications, scripts, automation, administrative operations, and AI-assisted operations.

### Heldo Time Machine

Recovery-oriented system design: recovery points, system rollback, configuration restoration, and pre-update snapshots.

### Heldo Recovery

A dedicated environment for system maintenance, covering diagnostics, boot recovery, configuration repair, and full system restoration.

### Heldo AI Pilot

An assistant that helps users analyze errors, inspect configuration, and troubleshoot issues, recommending corrective actions while keeping the user in control of every change.

### Heldo Project Bubbles

Isolated development environments that keep the host system clean and predictable.

| Languages and Runtimes | Platforms and Workloads |
|:--|:--|
| Python | Cloud Development |
| Web Development | DevOps |
| Java | Kubernetes |
| C / C++ | Containers |
| Go | AI / ML |

### Heldo Software

A unified experience to discover, install, update, and manage applications and developer tools.

<br>

## Security Foundation

Heldo OS is built around established Linux security technologies and secure-by-default configuration.

| Domain | Controls |
|:--|:--|
| Access Control | AppArmor, privilege management |
| Network | Firewall management |
| Auditing | System auditing |
| Isolation | Application isolation, sandboxed workloads |
| Maintenance | Security updates, secure system configuration |

<br>

## Architecture

Heldo OS combines a customized desktop and a set of Heldo-specific tools on top of a standard Linux core, organized into three pillars. AI Pilot assists across all of them.

```mermaid
%%{init: {'theme':'base','themeVariables':{'fontFamily':'Inter, Segoe UI, Arial','fontSize':'14px','primaryColor':'#ffffff','primaryBorderColor':'#0b3d91','primaryTextColor':'#1b1f24','lineColor':'#57606a'}}}%%
flowchart TB
    OS["<b>HELDO OS</b><br/>Desktop and Tooling Layer"]

    subgraph P["Pillars"]
        direction LR
        SEC["<b>Security</b><br/>Change Firewall"]
        REC["<b>Recovery</b><br/>Time Machine · Recovery"]
        DEV["<b>Development</b><br/>Project Bubbles · Software"]
    end

    AI["<b>AI Pilot</b><br/>Assisted diagnostics"]
    CORE["<b>LINUX CORE</b><br/>Kernel · AppArmor · Firewall · Auditing"]

    OS --> P
    AI -.-> P
    P --> CORE

    style OS fill:#0b3d91,stroke:#0b3d91,color:#ffffff
    style CORE fill:#1b1f24,stroke:#1b1f24,color:#ffffff
    style AI fill:#f6f8fa,stroke:#0b3d91,stroke-dasharray: 4 3,color:#1b1f24
    style SEC fill:#ffffff,stroke:#0b3d91,color:#1b1f24
    style REC fill:#ffffff,stroke:#0b3d91,color:#1b1f24
    style DEV fill:#ffffff,stroke:#0b3d91,color:#1b1f24
    style P fill:#f6f8fa,stroke:#d0d7de,color:#57606a
```

<br>

## Screenshots

<div align="center">

<img src="assets/desktop.png" alt="Heldo OS desktop" width="880">

<sub><b>Desktop</b></sub>

<br><br>

<img src="assets/tools.png" alt="Heldo OS application center" width="880">

<sub><b>Application Center</b></sub>

</div>

<!--
Add more screenshots the same way, for example:
<img src="assets/recovery.png" alt="Heldo Recovery" width="880">
-->

<br>

## Intended Users

Heldo OS targets professionals who need a productive desktop without giving up system control:

Software Developers · Cloud Engineers · DevOps Engineers · SRE Engineers · System Administrators · Security Engineers · AI/ML Engineers · Linux Enthusiasts

<br>

## Project Status

| Component | Stage |
|:--|:--|
| Core system design | Complete |
| Custom desktop | Complete |
| Change Firewall | In development |
| Time Machine | In development |
| Recovery environment | In development |
| Project Bubbles | In development |
| Heldo Software | In development |
| AI Pilot | Planned |

<br>

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

<br>

## Getting Started

Installation images and instructions will be published with the first public release. Watch this repository (**Watch › Custom › Releases**) to be notified.

<br>

## Contributing

Bug reports, feature ideas, and feedback are welcome.

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/short-description`
3. Commit your changes with a clear message
4. Open a pull request describing the change

For questions or proposals, [open an issue](../../issues).

<br>

## Security

If you discover a security vulnerability, please report it privately to the maintainer rather than opening a public issue.

<br>

## License

A license has not yet been selected. Until one is added, all rights are reserved by the author.

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0b3d91&height=2" width="100%" alt="">

<div align="center">
<sub><b>Heldo OS</b> &nbsp;·&nbsp; Security &nbsp;·&nbsp; Control &nbsp;·&nbsp; Recovery</sub>
</div>
