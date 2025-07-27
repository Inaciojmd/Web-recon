# 🔍 Web Vulnerability Scanner Toolkit

![Banner](assets/banner.png) *(Optional: Add actual banner image later)*

A multi-module security assessment tool for identifying vulnerabilities in web applications, with Tor anonymity support.

## 🌟 Features

### 🕵️‍♂️ Discovery Modules
| Module | Description | Tech Used |
|--------|-------------|-----------|
| **Crawler** | Advanced URL discovery with JS analysis | BeautifulSoup, Threading |
| **Admin Finder** | 50+ common admin panel paths | Requests |
| **CMS Detector** | WordPress, Joomla, Drupal identification | Signature matching |

### 🔬 Vulnerability Scanners
| Vulnerability | Detection Method | Payload Count |
|--------------|------------------|--------------|
| SQL Injection | Error-based, Time-based, Boolean | 25+ payloads |
| XSS (Reflected/DOM) | Context-aware payloads | 50+ variations |
| LFI | Path traversal, wrappers | 40+ techniques |
| SSRF | Internal endpoint testing | 8 targets |
| Open Redirect | 10+ bypass techniques | URL manipulation |
| CSTI | Template engine detection | 15+ payloads |

### 🛡️ Security Checks
- Header Security Analysis (CSP, HSTS, etc.)
- Middleware Bypass (12+ header techniques)
- WAF Detection (Cloudflare, Akamai)

## 🛠 Installation

### Prerequisites
- Python 3.8+
- Tor service

### Setup
```bash
# Clone repository
git clone https://github.com/yourusername/web-scanner.git
cd web-scanner

# Install dependencies
pip install -r requirements.txt

# Usage
python3 multi-main.py https://example.com

# Configure Tor (Linux)
sudo apt install tor
sudo systemctl start tor

