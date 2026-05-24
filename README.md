

Odoo security scanner — automated vulnerability assessment, CVE detection, misconfigurations and professional HTML reports.

---

## Installation

```bash
wget https://github.com/najemkhachoune-maker/odooscan/releases/download/v1.0.0/odooscan
chmod +x odooscan
sudo mv odooscan /usr/local/bin/
odooscan --version
```

---

## Usage

```bash
# Basic scan
odooscan --url https://target.com

# HTML report
odooscan --url https://target.com --format html --output report.html

# Stealth mode
odooscan --url https://target.com --mode stealth

# Aggressive mode
odooscan --url https://target.com --mode aggressive

# Brute force with wordlist
odooscan --url https://target.com --passwords /path/to/wordlist.txt

# Proxy support (Burp Suite)
odooscan --url https://target.com --proxy http://127.0.0.1:8080

# Update CVE database
odooscan --update

# Show version
odooscan --version
```

---

## Features

- Version detection via 5 methods
- Live CVE updates from NVD via --update
- 20+ exposed endpoint checks
- XSS, SQLi, SSTI injection testing with false positive filtering
- Default credential testing (235 passwords)
- Odoo-specific checks: open signup, demo DB, master password, filestore
- WAF and Cloudflare detection
- Confidence levels: HIGH / MEDIUM / LOW
- Professional HTML report with remediation and risk score 0-100
- OWASP Top 10 mapping
- Stealth / Normal / Aggressive modes
- JSON and HTML output

---

## Legal

For authorized security testing only.
