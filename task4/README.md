# 🔒 Windows Firewall Task – Cybersecurity Lab

## 🎯 Objective
Configure and test basic firewall rules to allow or block traffic using Windows Defender Firewall.

---

## 🛠️ Tools Used
- Windows Defender Firewall with Advanced Security
- PowerShell (for testing rules)
- (Optional) Telnet Client

---

## 📂 Files Included
- `Add_Rule/` – Step-by-step screenshots of the process
- `Rules_txt/` – Exported lists of firewall rules (before and after changes)
- `README.md` – This documentation

---

## 📝 Steps Performed

### 1. Export Existing Firewall Rules (Before Changes)
- Open Windows Defender Firewall with Advanced Security (`wf.msc`).
- Select **Inbound Rules**.
- Click **Export List...** and save as `Rules_txt/inbound_rules_before.txt`.

### 2. Block Inbound Traffic on Port 23 (Telnet)
- Go to **Inbound Rules** > **New Rule...**
- **Rule Type:** Port
- **Protocol:** TCP
- **Specific Local Port:** 23
- **Action:** Block the connection
- **Profile:** Domain, Private, Public (all selected)
- **Name:** Block Telnet (Port 23)
- Click **Finish**.


### 3. Test the Rule (Without Telnet)
- Open PowerShell as Administrator.
- Run:Test-NetConnection -ComputerName localhost -Port 23

- **Expected Result:** `TcpTestSucceeded : False` (port is blocked)



### 4. Restore Original State
- In **Inbound Rules**, right-click the "Block Telnet (Port 23)" rule and select **Delete**.

### 6. Export Firewall Rules (After Changes)
- Export the updated inbound rules list as `Rules_txt/inbound_rules_after.txt`.

---

## 🧠 Key Concepts Demonstrated
- **Port-based traffic blocking:** Blocked Telnet (port 23) to prevent insecure access.
- **Inbound vs Outbound rules:** Focused on controlling incoming connections.
- **Testing firewall rules:** Used PowerShell to verify port status.
- **Restoring firewall state:** Removed test rule to maintain original configuration.

---

## 🔎 How Windows Firewall Filters Traffic (Summary)
Windows Firewall inspects all network traffic entering or leaving the computer. It compares each packet to its list of rules:
- **Allow rules** let traffic through.
- **Block rules** deny traffic.
- Rules can be based on port, protocol, application, IP address, or network profile.
- If no rule matches, the firewall uses its default action (usually block for inbound, allow for outbound).

This process protects your system by only permitting trusted traffic and blocking unauthorized or potentially malicious connections.

---

## 📌 Outcome
- Gained hands-on experience configuring Windows Firewall.
- Understood how to apply, test, and remove firewall rules.
- Learned how port-based filtering can control network access.

---

## 📷 Screenshots & Exports
- See the `Add_Rule/` folder for screenshots of each step.
- See the `Rules_txt/` folder for exported firewall rule lists before and after changes.

---



