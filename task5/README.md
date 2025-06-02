# Wireshark Packet Capture Task

## Objective
Capture live network packets and identify basic protocols and traffic types.

## Tools Used
- **Wireshark** (free network protocol analyzer)

## Deliverables
- **Packet capture file:** `capture.pcapng` (attached)
- **Short report:** Protocols identified (see below)
- **Screenshots:** Attached for each protocol identified

---

## Steps Followed

1. **Installed Wireshark** on Windows using the official installer.
2. **Launched Wireshark** and selected the active network interface (Wi-Fi).
3. **Started packet capture** by clicking the interface.
4. **Generated network traffic** by:
    - Browsing websites in a web browser
    - Running `ping google.com` in Command Prompt
5. **Stopped the capture** after about one minute.
6. **Filtered packets** in Wireshark using display filters (`http`, `dns`, `tcp`) to identify different protocols.
7. **Saved the capture** as a `.pcapng` file (`capture.pcapng`).
8. **Took screenshots** of packet details for each identified protocol (attached).

---

## Protocols Identified

- **TCP:** Used for reliable, connection-oriented communication (e.g., web browsing).
- **DNS:** Used for domain name resolution (translating website names to IP addresses).
- **HTTP:** Used for web page requests and responses.

---

## Attachments

- **`capture.pcapng`**: Contains all captured network packets.
- **Screenshots**: Included for each protocol (TCP, DNS, HTTP) showing packet details in Wireshark.

