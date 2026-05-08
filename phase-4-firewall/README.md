# Phase 4: Firewall Implementation using pfSense

## Objective
The objective of this phase was to implement firewall rules using pfSense to restrict unauthorized network communication.

---

## Tool Used

- pfSense Firewall

---

## Firewall Configuration

Firewall rules were configured to monitor and control traffic between the attacker and target systems.

---

## Security Rule Implemented

A rule was created to block ICMP traffic from the attacker machine.

### Rule Details

| Parameter | Value |
|---|---|
| Protocol | ICMP |
| Source | Kali Linux |
| Destination | pfSense |
| Action | Block |

---

## Testing Procedure

### Before Firewall Rule

The attacker machine was able to communicate successfully using ping.

```bash
ping 192.168.216.2
```

### After Firewall Rule

The ICMP traffic was blocked successfully.

Result:
- 100% packet loss

---

## Security Benefits

- Unauthorized traffic restriction
- Network access control
- Basic attack prevention
- Traffic filtering

---

## Key Learnings

- Firewall rule creation
- ICMP filtering
- Traffic control
- Network segmentation

---

## Screenshots

### Firewall Rule
(Add screenshot here)

### Successful Ping (Before Blocking)
(Add screenshot here)

### Blocked Ping (After Firewall Rule)
(Add screenshot here)

---

## Conclusion

pfSense successfully blocked unauthorized ICMP communication and demonstrated effective firewall-based traffic control.
