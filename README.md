# 🛡️ Dark Network Mesh & Post-Quantum Cryptography (PQC) VPN

<p align="left">
  <img src="https://img.shields.io/badge/Architecture-Dark%20Network%20Mesh-8A2BE2?style=for-the-badge&logo=shield&logoColor=white" />
  <img src="https://img.shields.io/badge/Security-Post--Quantum%20Crypto-00C853?style=for-the-badge&logo=lock&logoColor=white" />
  <img src="https://img.shields.io/badge/Frontend-React%20%7C%20Vite-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Analytics-Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" />
  <img src="https://img.shields.io/badge/License-MIT-FFD700?style=for-the-badge&logo=open-source-initiative&logoColor=black" />
</p>

> **B2B FinTech Transaction Security Platform** operating over a **Dark Network Mesh** architecture integrated with **Post-Quantum Cryptography (PQC) VPN**, **Fwknop Single Packet Authorization (SPA)**, and **Rosenpass Key Exchange**.

---

## 🌐 Live Demo & Deployment

> ⚡ **Live VPS Dashboard:** [http://20.249.148.67:3000/](http://20.249.148.67:3000/)  
> *(Note: Available when the demonstration VPS instance is active).*

---

## 🌟 Key Features

* 🔐 **Post-Quantum Cryptography (PQC):** Integrates Rosenpass key exchange mechanisms to mitigate future "harvest now, decrypt later" quantum threats.
* 👻 **Stealth Port Architecture:** Employs `Fwknop` Single Packet Authorization (SPA) to keep firewall ports default-closed and invisible to port scanners.
* 🕸️ **Dark Network Mesh Tunneling:** Leverages WireGuard for low-latency, kernel-level encrypted mesh networking across B2B FinTech nodes.
* 📊 **Comprehensive Telemetry & Dashboards:** Real-time visual monitoring for mesh topology, PQC security status, penetration testing telemetry, and Grafana analytics integration.

---
## 📚 Technical Documentation & Project Report

The complete system design, performance benchmarks, and post-quantum VPN architecture report are available in the repository:

* 📄 **Project Report / Paper:** [`DNM PQC VPN-Group 3.pdf`](./Docs/DNM%20PQC%20VPN-Group%203.pdf)
* 📊 **Presentation Deck:** [`Dark Network Mesh & Post-Quantum Cryptography VPN.pdf`](./Docs/Dark%20Network%20Mesh%20%26%20Post-Quantum%20Cryptography%20VPN.pdf)

---

## 🏗️ Repository Architecture

```text
dnm-pqc-vpn/
├── 📂 Configurations/         # Security & Network Infrastructure Configs
│   ├── 📂 Fwknop/             # Single Packet Authorization (SPA) rules
│   ├── 📂 Rosenpass/          # Post-Quantum key exchange parameters
│   └── 📂 WireGuard/          # Mesh tunnel configurations (wg0.conf)
├── 📂 Docs/                   # System Architecture & Technical Reports
│   ├── 📄 DNM PQC VPN-Group 3.pdf
│   └── 📄 Dark Network Mesh & Post-Quantum Cryptography VPN.pdf
├── 📂 apps/
│   └── 💻 dashboard/          # React + Vite Monitoring Dashboard
│       ├── 📂 public/         # Favicon & SVG Assets
│       └── 📂 src/
│           ├── 📂 assets/     # Images & Graphic Assets (hero.png, etc.)
│           ├── 📂 components/ # UI Layouts (Sidebar, Header, Layout, ErrorAlert)
│           ├── 📂 lib/        # Telemetry Integrations (grafana.js)
│           └── 📂 pages/      # Feature Dashboards
│               ├── 📄 Benchmark.jsx
│               ├── 📄 DarkNetwork.jsx
│               ├── 📄 LogsMonitoring.jsx
│               ├── 📄 MeshTopology.jsx
│               ├── 📄 Overview.jsx
│               ├── 📄 PQCSecurity.jsx
│               └── 📄 PenTestResults.jsx
├── 📄 .gitignore
├── 📄 LICENSE
└── 📄 README.md
