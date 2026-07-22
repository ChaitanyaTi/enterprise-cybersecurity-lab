# Phase 6 — Splunk SIEM Integration

## Objective

This phase focuses on integrating Splunk SIEM into the cybersecurity SOC lab.

---

# Tools Used

- Splunk Enterprise
- pfSense Firewall
- Suricata IDS
- Kali Linux
- Metasploitable2

---

# Log Collection

Logs were forwarded from pfSense and Suricata to Splunk using Syslog UDP port 514.

---

# Features Implemented

- Security Event Monitoring
- Dashboard Visualization
- Firewall Log Analysis
- Attack Detection
- Security Alerts

---

# Splunk Queries

## Host Monitoring

```spl
index=main | top host
index=main | timechart count
index=main | top source
