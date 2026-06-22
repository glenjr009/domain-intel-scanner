# ⚡ Domain Intel Scanner

A full-stack OSINT (Open Source Intelligence) and network reconnaissance platform designed for security researchers, students, and defenders. The application combines active network enumeration with passive intelligence gathering through an interactive terminal-style interface.

---

## 🚀 Features

### 🔴 Active Reconnaissance

* **Port Scanning** – Scan common TCP services (22, 80, 443, 3306, 8080).
* **HTTP Banner Grabbing** – Retrieve server headers and technology information.
* **Subdomain Enumeration** – Discover subdomains using Certificate Transparency (CT) logs.
* **Service Discovery** – Identify publicly exposed services and endpoints.

### 🔵 Defensive Intelligence

* **Shannon Entropy Analysis** – Detect suspicious or randomly generated domain names.
* **DNS Record Analysis** – Retrieve A, MX, TXT, and NS records.
* **WHOIS Lookup** – View registrar, creation date, expiration date, and ownership details.
* **Infrastructure Visibility** – Understand domain configurations and exposure.

---

## 🛠️ Tech Stack

### Frontend

* React
* Vite
* JavaScript
* CSS

### Backend

* Python
* Flask
* Flask-CORS

### Libraries

* python-whois
* dnspython
* requests
* socket

---

## 📂 Project Structure

```text
domain-intel-scanner/
│
├── backend/
│   ├── app.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
└── README.md
```

---

## ⚙️ Quick Start

### Prerequisites

Install:

* Python 3.12+
* Node.js 18+
* npm

Verify installation:

```bash
python --version
node --version
npm --version
```

---

### 1. Clone Repository

```bash
git clone https://github.com/glenjr009/domain-intel-scanner.git
cd domain-intel-scanner
```

---

### 2. Setup Backend

Navigate to backend:

```bash
cd backend
```

Create virtual environment:

```bash
python -m venv venv
```

Activate environment:

#### Windows

```powershell
.\venv\Scripts\activate
```

#### Linux/macOS

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install flask flask-cors python-whois dnspython requests
```

Run backend server:

```bash
python app.py
```

Backend will start on:

```text
http://localhost:5000
```

---

### 3. Setup Frontend

Open a new terminal:

```bash
cd frontend
npm install
npm run dev
```

Frontend will start on:

```text
http://localhost:5173
```

---

## 🎯 Usage

1. Start the backend server.
2. Start the frontend application.
3. Open `http://localhost:5173`.
4. Enter a domain name.
5. Run the scan.
6. Review:

   * Open ports
   * DNS records
   * WHOIS information
   * Entropy score
   * HTTP headers
   * Subdomains

---

## 🤝 Contributing

Contributions are welcome.

### Create a Feature Branch

```bash
git checkout -b feature/AmazingFeature
```

### Commit Changes

```bash
git commit -m "feat: add passive Shodan integration"
```

### Push Changes

```bash
git push origin feature/AmazingFeature
```

### Open a Pull Request

Please include:

* Description of changes
* Motivation for the update
* Testing performed
* Screenshots (if applicable)

---

## 🛣️ Future Enhancements

* Shodan integration
* VirusTotal integration
* SSL certificate analysis
* GeoIP lookup
* ASN lookup
* Threat intelligence feeds
* Machine learning–based risk scoring
* Export reports (PDF/JSON)

---

## ⚖️ Disclaimer

This project is intended for educational purposes, authorized security assessments, research, and defensive security operations only.

Users are responsible for ensuring that all scanning and reconnaissance activities are performed only against systems and networks for which they have explicit authorization.

The authors and contributors are not responsible for any misuse of this software or any consequences resulting from its use.

---

## 📜 License

MIT License

Copyright © 2026 Glen Fernandes

---

⭐ If you find this project useful, consider starring the repository.
