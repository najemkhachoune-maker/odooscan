# OdooScan

Odoo security scanner — automated vulnerability assessment, CVE detection, misconfigurations and HTML reports for Odoo instances.

**By Najem**

## Installation

```bash
wget https://github.com/najemkhachoune-maker/odooscan/releases/download/v1.0.0/odooscan
chmod +x odooscan
sudo mv odooscan /usr/local/bin/
odooscan --help
```

## Usage

```bash
# Basic scan
odooscan --url https://target.com

# HTML report
odooscan --url https://target.com --format html --output report.html

# Aggressive scan with wordlist
odooscan --url https://target.com --mode aggressive --passwords /path/to/wordlist.txt

# Stealth mode
odooscan --url https://target.com --mode stealth

# Update CVE database
odooscan --update

# Show version
odooscan --version
```

## Features

- Version detection via 5 methods
- Live CVE updates from NVD (`--update`)
- 20+ exposed endpoint checks
- XSS, SQLi, SSTI injection testing
- Default credential testing
- Odoo-specific checks (open signup, demo DB, master password, filestore)
- WAF detection
- Confidence levels HIGH/MEDIUM/LOW
- Professional HTML report with remediation
- Risk score 0-100
- OWASP Top 10 mapping
- Stealth / Normal / Aggressive modes
- Proxy support
- JSON and HTML output

## Legal

For authorized security testing only.
Always obtain written authorization before scanning any system.
The author accepts no liability for misuse.
