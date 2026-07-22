# Phase 8: Packet Analysis using Wireshark

## Objective
The objective of this phase was to capture and analyze network packets generated during reconnaissance and exploitation activities.

---

## Tool Used

- Wireshark

---

## Packet Capture Setup

Wireshark was executed on the Kali Linux attacker machine to monitor traffic between:
- Kali Linux
- Metasploitable 2

---

## Traffic Generated

The following activities were captured:
- Nmap reconnaissance scan
- TCP connection attempts
- Exploitation traffic
- FTP communication

---

## Wireshark Filters Used

### Filter by Target IP

```text
ip.addr == 192.168.216.129
```

### Filter FTP Traffic

```text
tcp.port == 21
```

---

## Analysis Performed

The packet capture revealed:
- TCP SYN packets
- connection establishment attempts
- attacker and victim communication
- reconnaissance behavior

---

## Important Observations

| Source IP | Destination IP | Activity |
|---|---|---|
| 192.168.216.128 | 192.168.216.129 | Nmap Scan |
| 192.168.216.128 | 192.168.216.129 | FTP Exploit |

---

## Benefits of Packet Analysis

- Network traffic visibility
- Protocol analysis
- Attack investigation
- Forensic analysis

---

## Key Learnings

- TCP packet structure
- Packet inspection
- Network traffic analysis
- Attack traffic identification

---

## Screenshots

### Wireshark Packet Capture
(Add screenshot here)

### TCP Traffic Analysis
(Add screenshot here)

---

## Conclusion

Wireshark successfully captured and analyzed traffic generated during attack simulation, providing visibility into attacker-victim communication.
