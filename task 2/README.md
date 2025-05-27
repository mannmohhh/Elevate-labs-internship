# Task 2: Phishing Email Analysis

## Objective
Identify phishing characteristics in a suspicious email sample.

## Tools Used
- Text editor (Notepad, Sublime, VS Code)
- Free online email header analyzer (e.g., MXToolbox, Trustifi)
- VirusTotal (for checking suspicious links)

## Sample Email
See [From support@amaz0n-security.com.txt](From%20support@amaz0n-security.com.txt) for the full email content.

---

## Phishing Indicators Found

| Indicator                | Example/Details                                 |
|--------------------------|-------------------------------------------------|
| Spoofed sender address   | support@amaz0n-security.com (not real Amazon)   |
| Urgent language          | "Your account will be suspended!"               |
| Suspicious link          | http://malicious-site.ru                        |
| Generic greeting         | "Dear Customer"                                 |
| Spelling/grammar errors  | "acount" instead of "account"                   |
| Missing contact info     | No real phone/address in signature              |
| (Header issues, optional)| Mismatched "From" and "Reply-To" (if present)   |

---

## Summary of Phishing Traits

- The sender’s email address tries to mimic Amazon but is fake.
- The email uses urgent and threatening language to scare the recipient.
- The link does not go to the real Amazon website.
- There are spelling mistakes and a generic greeting.
- No real contact information is provided.
- (If you analyzed headers) The headers show mismatched addresses or failed authentication checks.

---

## Outcome

- Learned how to identify phishing tactics.
- Practiced analyzing suspicious emails for common red flags.
- Gained awareness of how phishing attacks trick users.

## What I Learned

- How to spot spoofed email addresses and fake links.
- The importance of checking email headers and sender info.
- How to summarize and report phishing indicators.
