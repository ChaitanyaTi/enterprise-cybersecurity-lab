## Enterprise Cybersecurity Lab – Attack Detection & Prevention

##  Overview
This project demonstrates a real-world cybersecurity lab where an attacker system (Kali Linux) performs reconnaissance attacks and a security gateway (pfSense with Suricata IDS) detects and prevents those attacks.

The goal is to simulate how organizations monitor and defend against network-based attacks using layered security.

---

##  Lab Architecture

- **Attacker:** Kali Linux  
- **Security Gateway:** pfSense (Firewall + Suricata IDS)  

###  Flow
Kali Linux → pfSense → Target System

---

##  Attack Simulation

###  Command Used
```bash
nmap -A -T4 192.168.216.2

Purpose

This scan attempts to:

- Discover open ports
- Identify running services
- Detect operating system

Detection (Suricata IDS)

Suricata detected the attack using Emerging Threat rules:

ET SCAN Possible Nmap User-Agent Observed
Outcome
- IDS successfully detected scanning activity
- Suspicious traffic was logged and analyzed

Prevention (Firewall)

A firewall rule was configured in pfSense to block attacker traffic.

🔹 Rule Details
Protocol: ICMP
Source: Attacker IP (Kali Linux)
Action: Block
🔹 Result
Before rule → Ping successful
After rule → Ping blocked (100% packet loss)


Screenshots
🔹 Nmap Scan

🔹 Suricata Alerts

🔹 Firewall Rule

🔹 Ping Blocked

Key Learnings
- Network security architecture design
- Difference between IDS and IPS
- Signature-based detection (Suricata rules)
- Firewall rule implementation using pfSense
- Real-world attack simulation using Nmap

Limitations
- Inline IPS mode is not fully supported in the virtual (VMware) environment
- Detection is primarily signature-based (rule dependent)

Future Improvements
- Add Metasploitable for exploitation testing
- Perform attacks using Metasploit framework
- Integrate Splunk SIEM for centralized log analysis
- Add brute-force and web-based attack simulations
- Automate detection using Python scripts

Status

Project in progress – more advanced attack simulations and detection mechanisms will be added
