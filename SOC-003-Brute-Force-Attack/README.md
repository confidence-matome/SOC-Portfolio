# SOC-003: Windows Brute Force Attack Investigation

## Overview

This investigation analyzes Windows authentication events to identify and investigate a suspected brute-force attack.

The objective is to determine whether repeated failed logon attempts indicate malicious activity and whether any account was successfully compromised.

---

## Objectives

- Detect repeated failed logons
- Identify targeted accounts
- Correlate failed and successful authentication events
- Assess the impact
- Document findings

---

## Skills Demonstrated

- Splunk Enterprise
- Windows Event Logs
- Event ID 4625
- Event ID 4624
- Authentication Analysis
- Incident Investigation
- SPL Queries
- Security Documentation

---

## Repository Structure

```
SOC-003-Brute-Force-Attack/
│
├── README.md
├── SOC-003-Brute-Force-Attack.md
├── SPL-Queries.md
├── IOC.md
└── Screenshots/
```
