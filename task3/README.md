# Vulnerability Report Summary (Nessus Essentials)

## 🎯 Target
- **IP Address:** 192.168.1.10  
- **Scanner:** Nessus Essentials  
- **Scan Date:** May 29, 2025

---

## 🔴 Critical Vulnerability

### 1. Node.js Multiple Vulnerabilities (Feb 14, 2024)
- **Plugin ID:** 190856
- **CVSS v3 Score:** 9.8
- **Description:**  
  Outdated Node.js versions contain severe vulnerabilities that may allow remote code execution or denial-of-service (DoS).
- **Affected Versions:**  
  Node.js 18.x < 18.19.1  
  Node.js 20.x < 20.11.1  
  Node.js 21.x < 21.6.2
- **Remediation:**  
  Upgrade Node.js to at least 18.19.1, 20.11.1, or 21.6.2.  
  Restrict network access and monitor for suspicious activity until the upgrade is complete.

---

## 🟠 Medium Vulnerabilities

### 2. SSL Certificate Cannot Be Trusted
- **Plugin ID:** 51192
- **CVSS Score:** 6.5
- **Description:**  
  The SSL certificate is self-signed or from an untrusted CA, which could allow man-in-the-middle (MITM) attacks.
- **Remediation:**  
  Replace the SSL certificate with one signed by a trusted Certificate Authority (CA).

### 3. Node.js Multiple Vulnerabilities (May 14, 2025)
- **Plugin ID:** 236766
- **CVSS Score:** 6.2
- **Description:**  
  Newer vulnerabilities in Node.js allowing potential DoS or memory exploits.
- **Affected Versions:**  
  Node.js 20.x < 20.19.2  
  Node.js 22.x < 22.15.1  
  Node.js 23.x < 23.11.1  
  Node.js 24.x < 24.0.2
- **Remediation:**  
  Upgrade Node.js to at least 20.19.2, 22.15.1, 23.11.1, or 24.0.2.

---

## ℹ️ Informational Findings

- Numerous informational plugins detected, including:
  - Software enumeration (Apache, Curl, OpenSSL, PHP, Java, Ruby, SQLite, nginx, etc.)
  - Network interface and routing information
  - OS and patch assessment
  - Service and process discovery

These findings provide context for the host’s configuration and do not require immediate action.

---

## ✅ Recommendations

- **Upgrade Node.js** to the latest secure versions as listed above.
- **Replace self-signed or untrusted SSL certificates** with certificates from trusted CAs.
- **Regularly update** all software dependencies.
- **Restrict network access** to critical services and monitor for suspicious activity.
- **Review informational findings** to ensure system hardening and best practices.

---

*Report generated from Tenable Nessus Essentials scan on 192.168.1.10, May 29, 2025.*
