# Chrome Extension Security Audit

## Overview

This project documents a comprehensive security audit of all installed Chrome extensions as part of a cyber security internship task. The objective is to identify, assess, and remove any suspicious or unnecessary browser extensions, thereby improving browser security and personal data protection.

---

## Table of Contents

1. [Audit Steps](#audit-steps)
2. [Extension Analysis](#extension-analysis)
   - [Downloader for Reddit™](#downloader-for-reddit)
   - [Free VPN for Chrome - VPN Proxy VeePN](#free-vpn-for-chrome---vpn-proxy-veepn)
   - [Mouse Pinch-To-Zoom](#mouse-pinch-to-zoom)
3. [Summary Table](#summary-table)
4. [Actions Taken](#actions-taken)
5. [Key Learnings](#key-learnings)
6. [Screenshots](#screenshots)

---

## Audit Steps

1. Opened Chrome and navigated to `chrome://extensions/`.
2. Reviewed all installed extensions, focusing on:
   - Permissions requested
   - Developer/source credibility
   - Extension status and warnings
   - User reviews and update history
3. Analyzed each extension’s risk profile.
4. Removed any extension deemed suspicious or unnecessary.
5. Restarted Chrome and checked for performance/security improvements.
6. Documented findings and actions in this README.

---

## Extension Analysis

### 1. Downloader for Reddit™

- **Status:** Disabled (turned off by Chrome)
- **Warning:** "This extension was turned off because it is no longer supported. Chrome recommends that you remove it."
- **Description:** Downloads full-sized images and videos from Reddit.
- **Version:** 1.1.6
- **Size:** 35.1 MB

**Permissions:**
- Manage your downloads
- Read and change your data on multiple domains (Reddit, Imgur, Gfycat, Google APIs)
- Allow access to file URLs
- Allow in Incognito (optional)

**Risk Assessment:**
- **High Risk:** No longer supported (no security updates or bug fixes).
- **Broad Permissions:** Can access and modify data on several domains.
- **Potential for Abuse:** Can manage downloads and access sensitive data.

**Action Taken:**
- **Removed** this extension due to security risks associated with unsupported status and broad permissions.

---

### 2. Free VPN for Chrome - VPN Proxy VeePN

- **Status:** Enabled
- **Description:** VPN service for privacy, unlimited traffic, and bandwidth.
- **Version:** 3.4.4
- **Size:** 3.7 MB

**Permissions:**
- Read and change all your data on all websites (very high risk)
- Display notifications
- Manage your apps, extensions, and themes
- Change your privacy-related settings
- Allow in Incognito (optional)
- Allow access to file URLs

**Risk Assessment:**
- **Very High Risk:** Can view and modify all web activity, manage extensions, and change privacy settings.
- **VPN Extensions:** Often targeted for abuse; require high trust in the provider.
- **Potential for Privacy Breach:** If the provider is not reputable, user data could be logged or sold.

**Action Taken:**
- [**Kept** this extension for now, as it is required for secure browsing and the provider is trusted. Will continue to monitor for any suspicious activity.]
  - _OR_
- [**Removed** this extension due to excessive permissions and privacy concerns.]

**Finding:**  
- [No immediate problem found, but user should regularly review VPN provider reputation and consider alternatives if privacy concerns arise.]

---

### 3. Mouse Pinch-To-Zoom

- **Status:** Enabled
- **Description:** Allows zooming in on specific parts of a website using mouse gestures.
- **Version:** 2.5.1
- **Size:** <1 MB

**Permissions:**
- Display notifications
- Read and change all your data on all websites
- Allow in Incognito (optional)
- Allow access to file URLs

**Risk Assessment:**
- **Moderate Risk:** Requests broad permissions for a simple function.
- **No Known Issues:** No negative reviews or suspicious activity detected. Developer appears reputable.

**Action Taken:**
- **Kept** this extension as it is useful and no immediate problems were found.

**Finding:**  
- No problem found.

---

## Summary Table

| Extension Name                       | Status    | Permissions Risk | Problem Found? | Action Taken   |
|--------------------------------------|-----------|-----------------|---------------|---------------|
| Downloader for Reddit™               | Disabled  | High            | Yes           | Removed       |
| Free VPN for Chrome - VPN Proxy VeePN| Enabled   | Very High       | [No/Yes]*     | [Kept/Removed]|
| Mouse Pinch-To-Zoom                  | Enabled   | Moderate        | No            | Kept          |

\*Update the table based on your actual action.

---

## Actions Taken

- Removed unsupported and high-risk extensions.
- Kept only those extensions that are necessary, trusted, and have no security concerns.
- Restarted Chrome after making changes.
- Documented all findings and actions.

---

## Key Learnings

- Unsupported extensions present a significant security risk and should be removed immediately.
- Extensions requesting broad permissions (especially "read and change all your data on all websites") must be reviewed very carefully.
- Only keep extensions from reputable developers and those you actively use.
- Regular extension audits are essential for maintaining browser security.

---


## Conclusion

This audit helped identify and remove potentially risky extensions, enhancing browser security. Regular review of browser extensions is a recommended best practice for all users.

