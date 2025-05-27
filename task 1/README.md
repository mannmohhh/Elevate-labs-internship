
# Network Scan Analysis - Elevate Labs Internship task 1

## 1. Common Services Found

| Port | Service        | Description                          |
|------|---------------|--------------------------------------|
| 135  | MSRPC         | Windows Remote Procedure Call         |
| 139  | NetBIOS-SSN   | Windows File/Printer Sharing          |
| 445  | Microsoft-DS  | Windows SMB File Sharing              |
| 1521 | Oracle        | Oracle Database Listener              |
| 8080 | HTTP-Proxy    | Web Server/Proxy                      |

## 2. Potential Security Risks

- **135 (MSRPC):** Can be abused for remote code execution if not secured.
- **139 (NetBIOS-SSN):** Exposes file sharing, can leak info or be targeted by malware.
- **445 (SMB):** Major target for ransomware and exploits like WannaCry.
- **1521 (Oracle):** If Oracle DB is running, attackers may try to access or disrupt it.
- **8080 (HTTP-Proxy):** May expose web admin panels or insecure web apps.

## 3. Recommendations

- Close all ports/services not needed.
- Restrict access to trusted IPs using a firewall.
- Keep all software updated and patched.
- Monitor logs for unusual activity.

## What I Learned

- How to use Nmap for port scanning.
- How to identify and research common network services.
- Basic risks of open ports and how to secure them.
