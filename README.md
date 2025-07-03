# WebVulnScanner01
This project is a basic Web Vulnerability Scanner written in Python. It tests a given URL for common security issues like XSS, SQL Injection, CSRF, and Remote Code Execution by sending crafted payloads and analyzing the server's response.
# 🔍 Web Vulnerability Scanner

A simple Python-based tool to scan a given URL for basic web vulnerabilities such as:

- ✅ Cross-Site Scripting (XSS)
- ✅ SQL Injection (SQLi)
- ✅ Cross-Site Request Forgery (CSRF)
- ✅ Remote Code Execution (RCE)

This tool sends crafted payloads to the target URL, analyzes the response, and generates both **HTML** and **PDF reports** of the findings.

---

## 🚀 Features

- Sends realistic requests using random User-Agent headers.
- Detects basic signs of:
  - XSS: `<script>` tag detection
  - SQLi: Error message patterns (e.g., "syntax", "sql")
  - CSRF: Form injection test
  - RCE: Output reflection for command terms
- Generates:
  - 📄 `report.html` — for browser viewing
  - 📄 `report.pdf` — for printable/downloadable use
- Simple CLI interface

---

## 📦 Requirements

- Python 3.x
- `requests`
- `fpdf`

Install dependencies:

```bash
pip install requests fpdf
