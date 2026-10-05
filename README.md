<p align="center">
  <img src="assets/banner.png" alt="Heldo OS: a Linux desktop where every sensitive change is visible, controllable, and reversible" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-in%20development-ff1a2e?style=for-the-badge&labelColor=0b0709" alt="Status">
  <img src="https://img.shields.io/badge/platform-linux-ff1a2e?style=for-the-badge&logo=linux&logoColor=white&labelColor=0b0709" alt="Platform">
  <img src="https://img.shields.io/badge/security-first-f97316?style=for-the-badge&logo=apparmor&logoColor=white&labelColor=0b0709" alt="Security first">
  <img src="https://img.shields.io/badge/license-TBD-6e7781?style=for-the-badge&labelColor=0b0709" alt="License">
</p>

<p align="center">
  <a href="#overview">Overview</a> ·
  <a href="#core-capabilities">Capabilities</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#screenshots">Screenshots</a> ·
  <a href="#project-status">Status</a> ·
  <a href="#roadmap">Roadmap</a> ·
  <a href="#faq">FAQ</a> ·
  <a href="#contributing">Contributing</a>
</p>

<img src="assets/divider.svg" width="100%" alt="">

> [!NOTE]
> **Heldo OS is under active development.** Components are built step by step and are not ready for production use. There is no public ISO yet.

## Overview

**Heldo OS** is a security-focused Linux desktop built on three ideas: **Review. Protect. Recover.**

Sensitive system changes don't happen silently. You see them, approve them, and have a way back if something breaks. Protection, recovery, isolated development environments, software management, and AI-assisted diagnostics live in one desktop.

### The problem

Managing a development workstation on Linux is powerful, but risky:

- Package installs can change system configuration.
- Scripts can make privileged changes without clear visibility.
- Development dependencies pile up on the host.
- Diagnosing failures means manual investigation.
- Recovering from a bad configuration is hard.
- AI tools can suggest fixes, but give you little control over what runs.

### The Heldo approach

Every sensitive operation should be:

<p align="center">
  <b>Visible</b> → <b>Reviewed</b> → <b>Approved</b> → <b>Protected</b> → <b>Reversible</b>
</p>

## Design principles

| Principle | What it means |
|:--|:--|
| 🛡️ **Security** | Controls are part of the OS experience, not optional add-ons. |
| 🎛️ **Control** | You stay in charge of anything that modifies the system. |
| 🔍 **Transparency** | Important activity is surfaced and explained in plain terms. |
| 🫧 **Isolation** | Development workloads are kept apart from the host. |
| ⏪ **Recoverability** | Every change has a clear path to rollback or recovery. |

<img src="assets/divider.svg" width="100%" alt="">

## Core capabilities

<p align="center">
  <img src="assets/features.svg" alt="Heldo OS core capabilities" width="900">
</p>

<details>
<summary><b>Project Bubbles: supported environments</b></summary>
<br>

| Languages & runtimes | Engineering workloads |
|:--|:--|
| Python | Cloud development |
| Java | DevOps |
| C / C++ | Kubernetes |
| Go | Containers |
| Web development | AI / ML |

</details>

<details>
<summary><b>Security foundation</b></summary>
<br>

| Domain | Controls |
|:--|:--|
| **Access control** | AppArmor, privilege management |
| **Network security** | Firewall management |
| **Auditing** | System activity and security auditing |
| **Isolation** | Application isolation and sandboxed workloads |
| **Maintenance** | Security updates and secure system configuration |

</details>

## How it works

```mermaid
flowchart LR
    A([Change requested]) --> B{Change Firewall}
    B -- Approved --> C[Create recovery point]
    B -- Denied --> D([System unchanged])
    C --> E[Apply change]
    E --> F{Issue detected?}
    F -- No --> G([Running normally])
    F -- Configuration issue --> H[Time Machine rollback]
    F -- System failure --> I[Recovery Environment]
    F -- Unknown cause --> J[AI Pilot diagnostics]
    J --> H
    H --> K([Known-good state])
    I --> K

    classDef ok fill:#9a3412,stroke:#f97316,color:#fff
    classDef step fill:#7f1d1d,stroke:#ff1a2e,color:#fff
    class G,K,D ok
    class C,E,H,I,J step
```

| Step | What happens |
|:--|:--|
| **Review** | Sensitive operations are shown to you instead of being applied silently. |
| **Protect** | Approved operations get a recovery point, so there is always a way back. |
| **Recover** | Investigate the issue, restore a previous state, or boot the recovery environment. |

## Architecture

<p align="center">
  <img src="assets/architecture.svg" alt="Heldo OS architecture" width="900">
</p>

| Pillar | Purpose |
|:--|:--|
| **Protection** | Control and monitor sensitive system operations. |
| **Recovery** | Provide recovery points and a dedicated repair environment. |
| **Isolation** | Keep development workloads away from the host. |
| **Assistance** | AI-assisted diagnostics and troubleshooting. |

<img src="assets/divider.svg" width="100%" alt="">

## Screenshots

<table>
  <tr>
    <td align="center" width="50%">
      <img src="assets/desktop.png" alt="Heldo OS desktop"><br>
      <sub><b>Heldo OS desktop</b></sub>
    </td>
    <td align="center" width="50%">
      <img src="assets/tools.png" alt="Heldo Software application center"><br>
      <sub><b>Heldo Software</b></sub>
    </td>
  </tr>
</table>

## Who it's for

| User | Primary use |
|:--|:--|
| **Software developers** | Isolated environments and dependency management |
| **Cloud engineers** | Cloud tooling and infrastructure workflows |
| **DevOps engineers** | Containers, Kubernetes, CI/CD, automation |
| **SREs** | Reliability and recovery |
| **System administrators** | Controlled system administration |
| **Security engineers** | Security-focused workstation management |
| **AI / ML engineers** | Isolated AI development environments |
| **Linux power users** | More visibility and control over system changes |

## Project status

| Component | Status |
|:--|:--|
| Core system design | ![Complete](https://img.shields.io/badge/-Complete-16a34a?style=flat-square) |
| Custom desktop | ![Complete](https://img.shields.io/badge/-Complete-16a34a?style=flat-square) |
| Change Firewall | ![In Development](https://img.shields.io/badge/-In%20Development-ff1a2e?style=flat-square) |
| Time Machine | ![In Development](https://img.shields.io/badge/-In%20Development-ff1a2e?style=flat-square) |
| Recovery Environment | ![In Development](https://img.shields.io/badge/-In%20Development-ff1a2e?style=flat-square) |
| Project Bubbles | ![In Development](https://img.shields.io/badge/-In%20Development-ff1a2e?style=flat-square) |
| Heldo Software | ![In Development](https://img.shields.io/badge/-In%20Development-ff1a2e?style=flat-square) |
| AI Pilot | ![Planned](https://img.shields.io/badge/-Planned-6e7781?style=flat-square) |

> [!WARNING]
> Don't rely on unreleased components for production systems or critical workloads.

## Roadmap

| Area | Goals | Progress |
|:--|:--|:--|
| **Foundation** | Core concept, architecture, custom desktop | ✅ Done |
| **Protection** | Policy engine · protected-operation detection · approval UI · activity visibility | 🔨 In progress |
| **Recovery** | Recovery points · rollback · recovery environment · boot repair | 🔨 In progress |
| **Development** | Project Bubbles · starter environments · containers & Kubernetes · cloud dev | 🔨 In progress |
| **Software** | Application center · install workflows · update management | 🔨 In progress |
| **Intelligence** | AI Pilot diagnostics · log analysis · suggested fixes · user-approved remediation | 🗓️ Planned |
| **Release** | First public ISO · install docs · release process · public docs | 🗓️ Planned |

Feature requests and discussion: [GitHub Issues](../../issues).

## Getting started

There is no public installation image yet. ISO images and install instructions will be published with the first release.

**Follow development:** GitHub → Watch → Custom → Releases

<img src="assets/divider.svg" width="100%" alt="">

## FAQ

<details>
<summary><b>What is Heldo OS?</b></summary>
<br>

A Linux-based operating system focused on security, system control, recoverability, and isolated development. It combines a customized desktop with Heldo components that make system changes visible and manageable.

</details>

<details>
<summary><b>Is Heldo OS a Linux distribution?</b></summary>
<br>

It's being built on a standard Linux foundation, with a customized desktop and Heldo-specific system components.

</details>

<details>
<summary><b>Can I install it today?</b></summary>
<br>

Not yet. Public images will ship with the first public release.

</details>

<details>
<summary><b>Does AI Pilot change my system automatically?</b></summary>
<br>

No. AI Pilot provides diagnostics and proposed solutions. You stay in control of any action that modifies the system.

</details>

<details>
<summary><b>What are Project Bubbles?</b></summary>
<br>

Isolated development environments that keep project dependencies and workloads separate from the host OS.

</details>

<details>
<summary><b>Is Heldo OS open source?</b></summary>
<br>

The license hasn't been chosen yet. Until one is published, all rights remain with the author.

</details>

## Contributing

Contributions, technical feedback, bug reports, and feature proposals are welcome.

1. Fork the repository.
2. Create a branch: `git checkout -b feature/short-description`
3. Make and test your changes locally.
4. Commit with a clear message: `git commit -m "Add short description of change"`
5. Push: `git push origin feature/short-description`
6. Open a pull request that covers what changed, why, how you tested it, and any known limitations.

Questions or proposals? Open an [Issue](../../issues).

## Security policy

If you find a potential vulnerability:

- **Don't report it in a public GitHub issue.**
- Report it privately to the project maintainer, with enough detail to reproduce it.
- Please don't share exploit details publicly until it has been investigated.

A dedicated reporting process will be published before the first public release.

## License

No license has been selected yet. Until one is added, **all rights are reserved by the author**.

<img src="assets/divider.svg" width="100%" alt="">

<p align="center">
  <sub><b>Heldo OS</b> · Review. Protect. Recover.</sub>
</p>
