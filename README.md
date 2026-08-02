# 🛡️ Dark Network Mesh & Post-Quantum Cryptography (PQC) VPN

<p align="left">
  <img src="https://img.shields.io/badge/Architecture-Dark%20Network%20Mesh-8A2BE2?style=for-the-badge&logo=shield&logoColor=white" />
  <img src="https://img.shields.io/badge/Security-Post--Quantum%20Crypto-00C853?style=for-the-badge&logo=lock&logoColor=white" />
  <img src="https://img.shields.io/badge/Frontend-React%20%7C%20Vite-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Styling-Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/License-MIT-FFD700?style=for-the-badge&logo=open-source-initiative&logoColor=black" />
</p>

> **B2B FinTech Transaction Security Platform** operating over a **Dark Network Mesh** architecture integrated with **Post-Quantum Cryptography (PQC) VPN**, **Fwknop Single Packet Authorization (SPA)**, and **Rosenpass Key Exchange**.

---

## 🌟 Key Features

* 🔐 **Post-Quantum Cryptography (PQC):** Utilizes Rosenpass to provide quantum-resistant key exchange mechanisms against future "harvest now, decrypt later" attacks.
* 👻 **Stealth Port Architecture:** Employs `Fwknop` Single Packet Authorization (SPA) to keep firewall ports closed and invisible to port scanners.
* 🕸️ **Dark Network Mesh Tunneling:** Leverages WireGuard for high-speed, encrypted mesh networking between B2B FinTech nodes.
* 📊 **Real-Time Monitoring Dashboard:** Interactive React-based dashboard to visualize network latency, node status, and secure transaction telemetry.

---

## 🏗️ Repository Architecture

```text
dnm-pqc-vpn/
├── 📂 apps/
│   └── 💻 dashboard/          # PQC-VPN Monitoring Dashboard (React + Vite)
│       ├── 📂 public/         # Static assets & icons
│       └── 📂 src/            # UI Components, State Management & Telemetry
├── 📂 Configurations/         # Security & Network Infrastructure Configs
│   ├── 📂 Fwknop/             # Single Packet Authorization (SPA) rules
│   ├── 📂 Rosenpass/          # Post-Quantum key exchange parameters
│   └── 📂 WireGuard/          # Mesh tunnel configurations (wg0.conf)
└── 📂 Docs/                   # System Architecture & Technical Documentation
