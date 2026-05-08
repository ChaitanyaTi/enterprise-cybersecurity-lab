# Phase 1: Cybersecurity Lab Environment Setup

## Objective
The objective of this phase was to create an isolated virtual cybersecurity lab environment for attack simulation, monitoring, and defense testing.

---

## Tools and Technologies Used

| Component | Purpose |
|---|---|
| Kali Linux | Attacker machine |
| Metasploitable 2 | Vulnerable victim machine |
| pfSense | Firewall and IDS gateway |
| Suricata | Intrusion Detection System |
| VMware Workstation | Virtualization platform |

---

## Lab Architecture

The virtual lab was designed to simulate a small enterprise network.

### Network Flow

```text
Kali Linux → pfSense → Metasploitable 2
```

---

## Virtual Machine Configuration

### Kali Linux
- Used as attacker machine
- Performed scanning and exploitation

### Metasploitable 2
- Used as intentionally vulnerable victim machine
- Hosted vulnerable services for exploitation testing

### pfSense
- Configured as firewall and security gateway
- Monitored traffic using Suricata IDS

---

## Network Configuration

All machines were connected using a Host-only virtual network to ensure:
- isolated environment
- secure testing
- controlled communication

### IP Address Configuration

| Machine | IP Address |
|---|---|
| Kali Linux | 192.168.216.128 |
| pfSense | 192.168.216.2 |
| Metasploitable 2 | 192.168.216.129 |

---

## Connectivity Verification

Connectivity between systems was verified using:

```bash
ping 192.168.216.129
```

---

## Benefits of Virtual Lab

- Safe attack simulation
- Realistic cybersecurity testing
- Isolated environment
- Hands-on learning

---

## Key Learnings

- Virtual network configuration
- Host-only networking
- Cybersecurity lab setup
- Enterprise-style security architecture

---

## Screenshots

### VMware Configuration
(Add screenshot here)

### Network Setup
(Add screenshot here)

### IP Configuration
(Add screenshot here)

---

## Conclusion

The virtual cybersecurity lab environment was successfully configured and prepared for attack simulation, monitoring, and defensive security testing.
