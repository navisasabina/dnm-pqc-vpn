# 🛡️ Dark Network Mesh & Post-Quantum Cryptography (PQC) VPN

![Status](https://img.shields.io/badge/Status-Completed-success)
![PQC](https://img.shields.io/badge/PQC-ML--KEM--1024-blue)
![VPN](https://img.shields.io/badge/VPN-WireGuard-orange)
![Monitoring](https://img.shields.io/badge/Monitoring-Prometheus%20%26%20Grafana-red)

A layered B2B FinTech VPN architecture combining **Single Packet Authorization (SPA / Dark Network)**, **WireGuard Mesh VPN**, and **Post-Quantum Cryptography (ML-KEM / Kyber via Rosenpass)** to mitigate "Harvest Now, Decrypt Later" (HNDL) threats and prevent network reconnaissance.

---

## 📐 System Architecture

The architecture implements a multi-layer defense strategy:

1. **Dark Network Layer (`fwknop`)**: Keeps WireGuard ports (`51820/UDP`) closed and invisible to scanners until a valid Single Packet Authorization (SPA) packet is received.
2. **Transport Encryption Layer (`WireGuard`)**: Provides lightweight, high-performance encrypted tunnels between nodes using Curve25519.
3. **Post-Quantum Layer (`Rosenpass`)**: Executes quantum-resistant key encapsulation (`ML-KEM-1024`) and injects fresh pre-shared keys (PSK) into WireGuard every 120 seconds.
4. **Application & Monitoring Layer**: Hosts simulated B2B transaction APIs (`FastAPI`) and real-time operational observability (`Prometheus`, `Grafana`, `WireGuard Exporter`).

---

## 🧰 Tech Stack

- **VPN & PQC Layer**: WireGuard, Rosenpass (ML-KEM-1024 / FIPS 203), fwknop (SPA)
- **Backend & Simulation**: Python 3.12, FastAPI, Uvicorn
- **Reliability & Monitoring**: Prometheus, Grafana, WireGuard Exporter
- **Web Dashboard**: React 19, Vite, Tailwind CSS, React Flow

---

## 👩‍💻 Contributors & Team Roles

This project was developed by Group 3 - Informatics, Faculty of Computer Science, President University (2026):

- **Navisa Ersa Sabina** (00120240083) – *Backend & Reliability Engineer*
  - Designed & implemented the Dummy Transaction API (`FastAPI`).
  - Configured system monitoring stack (`Prometheus`, `Grafana`, `WireGuard Exporter`).
  - Designed and executed system load testing, benchmarking, and traffic telemetry collection.
- **Mohammad Waarits Harahap** (001202400025)
- **Janet Dewi Evangeline** (001202400146)
- **Farrel Vidyano Sanggen** (001202400128)
- **Hengky Setiawan** (001202400198)

---

## 🚀 Quick Start & Setup

### 1. Run the Transaction API (Backend)
```bash
cd api
pip install -r requirements.txt
uvicorn app.main:app --host 10.100.0.1 --port 8000b
