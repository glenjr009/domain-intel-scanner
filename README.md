# ⚡ Domain Intel Scanner

## 🛡️ OSINT, Infrastructure Intelligence & Network Reconnaissance Platform

![Python](https://img.shields.io/badge/Python-3.12+-blue?style=for-the-badge\&logo=python)
![Flask](https://img.shields.io/badge/Flask-Backend-black?style=for-the-badge\&logo=flask)
![React](https://img.shields.io/badge/React-Frontend-61DAFB?style=for-the-badge\&logo=react)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-OSINT-green?style=for-the-badge)
![Networking](https://img.shields.io/badge/Networking-Reconnaissance-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)

---

## 🚀 Project Overview

**Domain Intel Scanner** is a full-stack cybersecurity intelligence platform built for security researchers, penetration testers, SOC analysts, students, and defenders.

The platform combines **Open Source Intelligence (OSINT)** techniques with **active network reconnaissance** to provide visibility into publicly exposed infrastructure, domain configurations, network services, and potential security risks.

Rather than performing simple DNS lookups, Domain Intel Scanner correlates intelligence from multiple sources including:

* 🌐 DNS Infrastructure Records
* 📜 Certificate Transparency Logs
* 🛰️ WHOIS Registration Data
* ⚡ Active TCP Service Discovery
* 🔍 HTTP Banner Fingerprinting
* 🧠 Shannon Entropy Analysis

The collected intelligence is aggregated into a cyberpunk-inspired terminal dashboard that presents technical findings in a structured and actionable format.

---

## 👨‍💻 Author

**Glen Fernandes**

Cybersecurity Enthusiast | CTF Player | SOC |

🔗 LinkedIn: https://www.linkedin.com/in/glen-ferns/

💻 GitHub: https://github.com/glenjr009

---

## 🎯 Project Objectives

The primary objectives of Domain Intel Scanner are:

* 🔍 Perform active reconnaissance against target domains
* 🌐 Enumerate DNS infrastructure and records
* 📜 Discover subdomains using CT logs
* ⚡ Identify exposed network services
* 🛰️ Gather WHOIS registration intelligence
* 🧠 Detect potentially suspicious domains using entropy analysis
* 📊 Visualize intelligence findings through an interactive dashboard
* 🛡️ Support both offensive and defensive security workflows

---

## ✨ Key Features

| Feature                       | Description                                             |
| ----------------------------- | ------------------------------------------------------- |
| ⚡ Active Port Scanning        | Detects exposed TCP services on common ports            |
| 🔍 HTTP Banner Fingerprinting | Identifies web technologies and server headers          |
| 📜 CT Log Enumeration         | Discovers subdomains from Certificate Transparency logs |
| 🌐 DNS Intelligence           | Retrieves A, MX, TXT, and NS records                    |
| 🛰️ WHOIS Analysis            | Extracts registrar and lifecycle information            |
| 🧠 Entropy Scoring            | Detects algorithmically generated domains               |
| 📊 Dashboard Visualization    | Displays findings in a terminal-style interface         |
| 🔴 Red Team Recon             | Infrastructure mapping and service discovery            |
| 🔵 Blue Team Visibility       | Asset inventory and exposure assessment                 |

---

## 🏗️ Intelligence Collection Pipeline

```text
Target Domain
      ↓
WHOIS Lookup
      ↓
DNS Intelligence
      ↓
CT Log Enumeration
      ↓
Subdomain Discovery
      ↓
TCP Port Scanning
      ↓
HTTP Banner Analysis
      ↓
Entropy Calculation
      ↓
Risk & Infrastructure Assessment
      ↓
Cyberpunk Dashboard
```

---

## 🔴 Red Team Reconnaissance Modules

### Active TCP Service Discovery

The scanner actively probes commonly exposed services:

```text
22    → SSH
80    → HTTP
443   → HTTPS
3306  → MySQL
8080  → Alternate HTTP
```

Capabilities:

* Multi-port scanning
* Fast timeout handling
* Service exposure detection
* Initial attack surface mapping

---

### HTTP Banner Fingerprinting

Retrieves:

```http
Server: nginx
X-Powered-By: Express
Via: Cloudflare
```

Used for:

* Technology identification
* Framework discovery
* Reverse proxy detection
* Surface enumeration

---

### Certificate Transparency Enumeration

Queries public CT logs to discover:

* Development subdomains
* Forgotten assets
* Staging environments
* Additional attack surface

Source:

```text
crt.sh
```

---

## 🔵 Blue Team Intelligence Modules

### DNS Infrastructure Analysis

Collects:

* A Records
* MX Records
* TXT Records
* NS Records

Used for:

* Asset inventory
* Email security validation
* Infrastructure mapping

### WHOIS Lifecycle Analysis

Retrieves:

* Registrar
* Registration Date
* Expiry Date
* Domain Status
* Ownership Metadata

### Shannon Entropy Analysis

The entropy engine evaluates randomness within domain names.

Higher entropy may indicate:

* DGA domains
* Malware infrastructure
* Phishing campaigns
* Randomized subdomains

Formula:

```text
H(X) = -Σ p(x) log₂ p(x)
```

---

## 🧱 Tech Stack

| Layer            | Technology            |
| ---------------- | --------------------- |
| Frontend         | React + Vite          |
| Backend          | Flask                 |
| Networking       | Python Socket         |
| DNS Intelligence | dnspython             |
| WHOIS            | python-whois          |
| CT Logs          | crt.sh                |
| HTTP Analysis    | requests              |
| Visualization    | React Dashboard       |
| Styling          | Cyberpunk Terminal UI |

---

## 📂 Project Structure

```text
domain-intel-scanner/
│
├── backend/
│   ├── app.py
│   ├── scanner.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
└── README.md
```
