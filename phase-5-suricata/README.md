# Phase 5: Intrusion Detection using Suricata

## Objective
The objective of this phase was to monitor and detect suspicious network activity using Suricata IDS integrated with pfSense.

---

## Tools Used

- pfSense
- Suricata IDS
- Kali Linux
- Metasploitable 2

---

## IDS Configuration

Suricata was installed and configured on the pfSense firewall.

### Enabled Rule Categories

- Emerging Threats Open Rules
- Scan Detection Rules
- Malware Detection Rules
- Exploit Detection Rules

---

## Attack Detection

During reconnaissance and exploitation activity, Suricata generated alerts for suspicious traffic.

### Example Alerts

```text
ET SCAN Possible Nmap User-Agent Observed
SURICATA SMB malformed request
```

---

## Detection Analysis

The IDS successfully identified:
- reconnaissance activity
- malformed SMB traffic
- suspicious protocol behavior
- possible exploit attempts

---

## Benefits of IDS

- Real-time traffic monitoring
- Threat detection
- Attack visibility
- Network security monitoring

---

## Key Learnings

- Signature-based intrusion detection
- IDS rule monitoring
- Security event analysis
- Threat visibility in enterprise environments

---

## Screenshots

### Suricata Alerts
(Add screenshot here)

### IDS Dashboard
(Add screenshot here)

---

## Conclusion

Suricata successfully detected multiple suspicious activities generated during attack simulation and provided visibility into network threats.
