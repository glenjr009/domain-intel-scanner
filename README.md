⚡ Domain Intel Scanner

A high-performance, full-stack OSINT (Open Source Intelligence) and active network reconnaissance engine wrapped in an immersive retro-cyberpunk terminal interface. Engineered for active TCP service mapping, passive subdomain mining, and structural security threat evaluation.

🚀 Key Capabilities

This system separates intensive networking lookups from visual rendering to provide fluid, real-time background data assembly across offensive and defensive vectors:

🔴 Red Team Spectrum (Active Reconnaissance)

Active Port Fingerprinting: Rapid, multi-port TCP sockets mapping common operational entry points (SSH 22, HTTP 80, HTTPS 443, MySQL 3306, Alt-HTTP 8080) backed by localized timeout handlers.

HTTP Banner Grabbing: Captures and evaluates raw response headers to uncover structural server footprints, active software versions, and proxy routes (Server, X-Powered-By, Via).

Passive Asset Enumeration: Automatically queries public Certificate Transparency (CT) logs (crt.sh) to locate and display secondary hidden subdomains.

🔵 Blue Team Spectrum (Defensive Threat Intelligence)

Shannon Entropy Metric: Computes the mathematical randomness of target character arrays to mathematically flag potential Domain Generation Algorithms (DGAs) or high-complexity phishing anomalies.

DNS Zone Analyzer: Automatically queries and maps authoritative global nameservers to resolve structural configurations (A, MX, TXT records).

WHOIS Lifecycle Tracking: Pulls real-time registrar metadata and timelines to identify domain creation dates and administrative details.

⚙️ Quick Start Guide

Follow these steps to deploy the scanner locally. Ensure you have Node.js and Python 3.12+ installed.

1. Clone the Repository
```bash
git clone [https://github.com/glenjr009/domain-intel-scanner.git](https://github.com/glenjr009/domain-intel-scanner.git)
cd domain-intel-scanner


2. Configure the Backend Core Engine

Open your terminal and spin up the Python API:

# Shift focus into the backend directory
cd backend

# Create an isolated local virtual environment
python -m venv venv

# Activate the environment (Windows PowerShell)
.\venv\Scripts\activate

# OR Activate the environment (Mac/Linux)
# source venv/bin/activate

# Install all requisite intelligence dependencies
pip install flask flask-cors python-whois dnspython requests

# Launch the local API server loop (Runs on port 5000)
python app.py


3. Deploy the Interactive Terminal UI

Open a second terminal window or split-pane workspace (leaving the backend running) and execute:

# Move to the frontend web folder
cd frontend

# Install the Node packages and modules
npm install

# Initialize the responsive local Vite dev pipeline
npm run dev


Open your web browser and navigate to http://localhost:5173/ to log into your glowing cybersecurity scanner deck.

🤝 Open Source Contributions

Contributions drive the evolution of security tools. Whether you want to optimize port scanner performance, integrate automated ML-based score evaluations, or refine terminal styles, your pull requests are highly welcomed!

Development Workflow

Fork the repository to your own profile.

Create an isolated feature branch:

git checkout -b feature/AmazingFeature


Commit your modifications using clear structural notes:

git commit -m "feat: integrate passive shodan lookups"


Push your changes up to the remote branch:

git push origin feature/AmazingFeature


Submit a detailed Pull Request explaining your functional upgrades.

⚖️ Legal Compliance & Disclaimer

This platform is engineered exclusively for authorized security reconnaissance, professional asset validation, corporate vulnerability audit tracking, and academic threat research. Executing active socket port scans against remote internet networks without explicit prior written authorization from the target owner is strictly non-compliant and illegal. The maintainers assume zero legal accountability or liability for malicious deployments or non-compliant usage.
