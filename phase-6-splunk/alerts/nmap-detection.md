# Nmap Detection Alert

## Objective

Detect reconnaissance and scanning activity originating from the Kali Linux attacker machine.

---

# Detection Query

```spl
index=main 192.168.216.128
```

---

# Alert Purpose

This alert identifies suspicious reconnaissance activity such as Nmap scans within the monitored network environment.

---

# Attack Source

Kali Linux

---

# Monitoring Tool

Splunk SIEM

---

# Detection Method

Firewall and IDS logs forwarded from pfSense and Snort to Splunk using Syslog UDP port 514.

---

# Expected Result

Security analysts can identify:
- Port scanning activity
- Reconnaissance attempts
- Unauthorized network discovery
- Suspicious source hosts

---

# Learning Outcome

- SIEM Alert Creation
- Threat Detection
- SOC Monitoring Workflow
- Reconnaissance Identification
