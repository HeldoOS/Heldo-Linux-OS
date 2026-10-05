Heldo OS

<p align="center">
  <img src="assets/Heldo_OS_logo.png" alt="Heldo OS Logo" width="180">
</p>

<h3 align="center">
  A Linux Desktop Built with Security, Control, Recovery and Developer Experience in Mind.
</h3>

<p align="center">
  <strong>Control your system. Understand what is happening. Recover when something goes wrong.</strong>
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#screenshots">Screenshots</a> •
  <a href="#architecture">Architecture</a> •
  <a href="#development">Development</a> •
  <a href="#roadmap">Roadmap</a>
</p>

---

## 🚀 About Heldo OS

**Heldo OS** is a custom Linux operating system designed to bring together:

- 🔐 Security
- 🛡️ System control
- ⏪ Recovery
- 🤖 AI-assisted troubleshooting
- 📦 Isolated development environments
- 💻 Developer productivity
- 🛍️ Simplified software management

I started Heldo OS as an idea and have been building it through continuous **development, testing, troubleshooting, and refinement**.

The goal is not simply to customize the appearance of Linux, but to explore a different approach to the desktop operating-system experience.

> **Control your system. Understand what is happening. Recover when something goes wrong.**

---

## 🎯 Vision

Modern operating systems are powerful, but system changes can sometimes be difficult to understand, troubleshoot, or reverse.

Heldo OS aims to make these processes more visible and manageable by bringing system protection, recovery, development environments, and intelligent assistance closer together.

The long-term vision is to create a Linux desktop that provides:

**Security → Control → Intelligence → Isolation → Recovery**

---

# ✨ Features

## 🛡️ Heldo Change Firewall

A system-level security concept focused on controlling sensitive changes made by:

- Applications
- Scripts
- Automation
- Administrative operations
- AI-assisted operations

The goal is to provide better visibility and control over important system modifications.

---

## 🤖 Heldo AI Pilot

An AI-assisted system designed to help users understand and troubleshoot their operating system.

Potential capabilities include:

- System issue analysis
- Error investigation
- Configuration analysis
- Troubleshooting assistance
- Recommended corrective actions
- Controlled system operations

The objective is to make complex system troubleshooting easier without removing user control.

---

## ⏪ Heldo Time Machine

A recovery-oriented system designed around the idea of restoring the operating system after unwanted or problematic changes.

Possible capabilities include:

- Recovery points
- System rollback
- Configuration restoration
- Change recovery
- Pre-update recovery

---

## 🛠️ Heldo Recovery

A dedicated recovery environment for maintaining the operating system.

Designed to assist with:

- System diagnostics
- Boot recovery
- Configuration repair
- System restoration
- Recovery operations
- Troubleshooting

---

## 📦 Heldo Project Bubbles

Isolated environments designed for development workloads.

Target environments include:

- 🐍 Python
- 🌐 Web Development
- ☕ Java
- ⚙️ C / C++
- 🐹 Go
- 🤖 AI / ML
- ☁️ Cloud Development
- 🔧 DevOps
- ☸️ Kubernetes
- 🐳 Containers

The objective is to allow developers to work in isolated environments while keeping the host system cleaner and more controlled.

---

## 🔐 Security Foundation

Heldo OS is being developed with a security-first mindset.

The system incorporates or is designed around technologies and controls such as:

- AppArmor
- Firewall management
- System auditing
- Security updates
- Privilege management
- Application isolation
- Sandboxed workloads
- Secure system configuration

Security is treated as a fundamental part of the operating system rather than an optional add-on.

---

## 💻 Developer Experience

Heldo OS is designed with developers and infrastructure professionals in mind.

Target users include:

- Software Developers
- Cloud Engineers
- DevOps Engineers
- SRE Engineers
- System Administrators
- Security Engineers
- AI/ML Engineers
- Linux Enthusiasts

The objective is to provide a productive desktop while maintaining strong system control.

---

## 🛍️ Heldo Software

Heldo OS includes a unified approach to software management.

The goal is to make it easier for users to:

- Discover applications
- Install applications
- Update applications
- Manage installed software
- Access developer tools

The long-term objective is to provide a consistent software-management experience across the Heldo ecosystem.

---

# 🖥️ Screenshots

## Desktop

<p align="center">
  <img src="assets/screenshots/desktop.png" alt="Heldo OS Desktop" width="900">
</p>

---

## Heldo OS Application Center

<p align="center">
  <img src="assets/screenshots/software-center.png" alt="Heldo Software Center" width="900">
</p>

---

## Heldo Recovery

<p align="center">
  <img src="assets/screenshots/recovery.png" alt="Heldo Recovery" width="900">
</p>

---

## Heldo Security

<p align="center">
  <img src="assets/screenshots/security.png" alt="Heldo Security" width="900">
</p>

---

# 🏗️ Architecture

Heldo OS is built as a Linux-based operating system with a customized desktop experience and an ecosystem of Heldo-specific tools.

```text
                    ┌──────────────────────┐
                    │      Heldo OS        │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
       ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
       │   Security  │  │  Recovery   │  │ Development │
       └──────┬──────┘  └──────┬──────┘  └──────┬──────┘
              │                │                │
              ▼                ▼                ▼
       ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
       │ Change      │  │ Time        │  │ Project     │
       │ Firewall    │  │ Machine     │  │ Bubbles     │
       └─────────────┘  └─────────────┘  └─────────────┘
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                      ┌─────────────────┐
                      │   Linux Core    │
                      └─────────────────┘
