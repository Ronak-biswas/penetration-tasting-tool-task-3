# 🛠️ PenTest Toolkit 

PenTest Toolkit is a lightweight, modular, and fast Python command-line utility built for security enthusiasts and penetration testers to perform basic reconnaissance, infrastructure scanning, and cryptographic auditing. 

Featuring multithreaded scanning engines and cross-platform ANSI colorized logs, this toolkit allows security analysts to perform targeted network audits efficiently.

---

## ✨ Modules & Core Features

*   **⚡ Port Scanner:** A multithreaded network mapping engine that scans for top industry ports or custom user-defined ranges. It grabs banners automatically for common services (FTP, SSH, SMTP, HTTP) and highlights insecure open ports.
*   **🌐 DNS Reconnaissance:** Gathers standard DNS infrastructure configurations (`A`, `MX`, `NS`, `TXT`, `CNAME`, `SOA` records), evaluates explicit spoofing risks via SPF/DMARC configurations, checks for Zone Transfer configurations (`AXFR`), and offers fast subdomain brute-forcing.
*   **🔒 HTTP Header Auditor:** Queries targets to check defensive configurations. It checks for missing core controls (`Content-Security-Policy`, `Strict-Transport-Security`, `X-Frame-Options`, etc.), unencrypted plain-text schemes, and checks for improper cookie flags (`Secure`/`HttpOnly`).
*   **🔑 SSL/TLS Cipher Checker:** Tests transport layer safety by validating operational deployment protocols. It spots outdated standard protocols (`SSLv2/v3`, `TLSv1.0/1.1`), tags legacy, weak cryptographic algorithms, checks certificate validation windows, and verifies hostname Subject Alternative Name (SAN) consistency.
*   **🎯 Hash Cracker:** A fast password auditing routine featuring automated byte-length identification for standard hashing patterns (`MD5`, `SHA-1`, `SHA-256`, `SHA-512`). It runs smart built-in rule mutation modules (such as capitalization and suffix additions) against string profiles.

---

## 🛠️ Tech Stack & Dependencies

*   **Language:** Python 3.x
*   **Standard Extensions:** `socket`, `threading`, `queue`, `hashlib`, `ssl`, `argparse`
*   **Third-Party Requirements:**
    *   `requests` — For managing comprehensive HTTP request-response parsing.
    *   `dnspython` — For handling lower-level asynchronous DNS queries.

To install the necessary external packages, execute:
```bash
pip install requests dnspython
