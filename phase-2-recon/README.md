# Phase 2: Reconnaissance and Service Enumeration

## Objective
The objective of this phase was to perform reconnaissance against the target machine in order to identify exposed services, open ports, and potential attack surfaces.

---

## Tools Used

- Kali Linux
- Nmap

---

## Target Information

| Machine | IP Address |
|---|---|
| Kali Linux (Attacker) | 192.168.216.128 |
| Metasploitable 2 (Victim) | 192.168.216.129 |

---

## Connectivity Verification

Before reconnaissance, connectivity between attacker and victim systems was verified.

### Command Used

```bash
ping 192.168.216.129
```

### Result

The target machine responded successfully, confirming network connectivity.

---

## Reconnaissance using Nmap

Nmap was used to scan the target system and identify active services.

### Command Used

```bash
nmap -F 192.168.216.129
```

---

## Command Explanation

| Parameter | Description |
|---|---|
| nmap | Network scanning tool |
| -F | Fast scan mode (top common ports) |
| 192.168.216.129 | Target IP address |

---

## Open Ports and Services Identified

| Port | Service |
|---|---|
| 21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 25 | SMTP |
| 80 | HTTP |
| 111 | RPCBind |
| 139 | NetBIOS |
| 445 | SMB |
| 3306 | MySQL |
| 5432 | PostgreSQL |
| 5900 | VNC |

---

## Analysis

The target machine exposed multiple insecure and legacy services.

Examples:
- Telnet transmits data in plaintext
- FTP services may contain vulnerabilities
- SMB services are commonly targeted during exploitation

These exposed services significantly increased the attack surface of the target system.

---

## Security Risks Identified

- Weak legacy protocols
- Multiple exposed network services
- Vulnerable software versions
- Increased attack surface

---

## Key Learnings

- Network reconnaissance techniques
- Service enumeration
- Attack surface analysis
- Open port identification
- Understanding exposed services

---

## Screenshots

### Connectivity Verification
(Add screenshot here)

### Nmap Scan Result
(Add screenshot here)

### Open Ports and Services
(Add screenshot here)

---

## Conclusion

Reconnaissance successfully identified multiple exposed services and potential vulnerabilities on the target machine, providing the foundation for further exploitation testing.
