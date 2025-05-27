# Task 2: Phishing Email Analysis – Elevate Labs Internship

## Objective
Analyze a suspicious email sample to identify phishing characteristics and demonstrate email threat detection skills.

---

## Tools Used
- Text editor (Notepad, VS Code)
- [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- Manual link inspection (hover and check URLs)
- Basic knowledge of email authentication (SPF, DKIM, DMARC)

---

## Sample Email

The full phishing email sample, including headers and body, is provided in [phishing_email.txt](phishing_email.txt).

---

## Phishing Indicators Identified

| Indicator                | Example/Details                                                                                      |
|--------------------------|------------------------------------------------------------------------------------------------------|
| **Spoofed sender address**   | `no-reply@secure-paypal.com` (not the real PayPal domain)                                        |
| **Return-Path mismatch**     | `no-reply@secure-paypal.com` (should match official PayPal domain)                               |
| **SPF/DKIM authentication failed** | `SPF: fail`, `DKIM: fail` (sender not authorized, possible spoofing)                   |
| **Suspicious Reply-To**      | `noreply-paypal@consultant.com` (not a PayPal address)                                          |
| **Urgent/threatening language** | “Your account may be permanently suspended” and “Action Required” in subject/body           |
| **Suspicious link**          | `https://paypal-security-check.com/verify` (not a real PayPal domain)                           |
| **Generic greeting**         | “Dear Customer” instead of recipient’s real name                                                |
| **No real contact info**     | Generic signature, no phone/address                                                             |
| **Unusual sending server**   | `mail.secure-paypal.com` (not an official PayPal server)                                        |

---

## Header Analysis (MXToolbox Findings)

- **SPF and DKIM:** Both failed, indicating the sender is not authorized to send on behalf of PayPal.
- **Received:** Email was sent from a server unrelated to PayPal.
- **Return-Path:** Does not match PayPal’s real domain.
- **Reply-To:** Points to a suspicious, non-PayPal address.

---

## Summary of Phishing Traits

This email uses several classic phishing tactics:
- **Domain spoofing** to appear legitimate.
- **Failed authentication** (SPF/DKIM) in the headers, a strong technical red flag.
- **Urgency and fear** to pressure the recipient into clicking a malicious link.
- **Generic language** and **lack of personalization**.
- **Suspicious links** that lead to a non-official website.

---

## Outcome

- **Developed awareness of phishing tactics** and how attackers construct convincing emails.
- **Learned to analyze both visible content and technical headers** for signs of phishing.
- **Practiced using online tools** (MXToolbox) to assist in email header analysis.

---

## What I Learned

- How to spot spoofed sender addresses and mismatched domains.
- The importance of SPF, DKIM, and DMARC in email authentication.
- How to identify urgent or threatening language and suspicious links.
- The process of summarizing and reporting phishing indicators for security awareness.

---

## References

- [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- [Phishing Email Examples – Terranova Security](https://www.terranovasecurity.com/blog/phishing-email-examples/)
- [How to Analyze Email Headers – Cornell University](https://it.cornell.edu/managed-servers/how-find-email-headers)
