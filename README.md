# ⚡ Domain Intel Scanner

> A high-performance, full-stack OSINT and Active Reconnaissance engine featuring a retro-terminal UI. Built for both offensive infrastructure mapping and defensive threat analysis.

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)
![Python](https://img.shields.io/badge/python-3.12+-blue.svg?style=for-the-badge&logo=python&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)

---

## 👁️ Overview

**Domain Intel Scanner** bridges the gap between passive open-source intelligence and active network reconnaissance. Operating through a decoupled React-based terminal emulator and a Python/Flask backend, it provides security researchers with instant visibility into target environments.

### 🔴 Red Team (Offensive Reconnaissance)
* **Active Port Scanning:** Fast-timeout TCP socket probes against critical entry points (SSH `22`, HTTP `80`, HTTPS `443`, MySQL `3306`, Alt-HTTP `8080`).
* **Banner Grabbing:** Extracts raw HTTP response headers to footprint underlying server technologies and proxy frameworks.
* **Passive Subdomain Mapping:** Automates queries against public Certificate Transparency (CT) logs (`crt.sh`) to discover hidden organizational assets.

### 🔵 Blue Team (Defensive Intelligence)
* **Lexical Entropy Scoring:** Calculates mathematical Shannon Entropy of domain strings to identify high-randomness DGAs (Domain Generation Algorithms) and phishing variants.
* **Infrastructure Resolution:** Resolves IPv4 routing and maps authoritative DNS configurations (`A`, `MX`, `TXT`).
* **Registration Timelines:** Pulls real-time WHOIS metadata to track domain registrars and creation/expiration lifecycles.

---

## 🏗️ System Architecture

* **Frontend:** React.js (Vite), Custom CSS Grid, Asynchronous Fetch API.
* **Backend:** Python 3.12, Flask, Flask-CORS.
* **Core Libraries:** `dnspython`, `python-whois`, `requests`, native `socket` threading.

---

## 🚀 Quick Start Guide

Follow these steps to deploy the scanner locally. Ensure you have **Node.js** and **Python 3.12+** installed on your system.

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_USERNAME/domain-intel-scanner.git](https://github.com/YOUR_USERNAME/domain-intel-scanner.git)
cd domain-intel-scanner
