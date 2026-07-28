# SOC-001: Windows Authentication Investigation

## Overview

This investigation analyzes Windows Security authentication events using Splunk Enterprise and the Boss of the SOC (BOTS) v3 dataset.

The objective was to establish an authentication baseline by examining successful and failed logon activity.

---

## Objectives

- Analyze Windows Security Event IDs 4624 and 4625
- Identify successful and failed authentication attempts
- Establish an authentication baseline
- Document investigation findings using evidence collected from Splunk

---

## Dataset

- Boss of the SOC (BOTS) v3
- Windows Security Event Logs

---

## Tools Used

- Splunk Enterprise 10.4
- Windows Event Logs
- GitHub

---

## Investigation Summary

The investigation focused on Windows authentication activity within the BOTS v3 dataset.

Key observations:

- 427 successful logons (Event ID 4624)
- 3 failed logons (Event ID 4625)
- Authentication events were analyzed to establish a baseline.
- No evidence of widespread brute-force activity was identified during the investigation.

---

## Repository Structure

```text
SOC-001-Windows-Authentication/
│
├── README.md
├── SOC-001-Windows-Authentication-Investigation.pdf
├── SPL-Queries.md
└── Screenshots/
```

---

## Skills Demonstrated

- Windows Event Log Analysis
- Authentication Investigation
- Splunk Enterprise
- SPL Queries
- Security Monitoring
- Incident Documentation

---

## MITRE ATT&CK

Although this investigation focuses on authentication analysis rather than confirmed malicious activity, it relates to:

- T1078 – Valid Accounts (authentication monitoring)

---

## Investigation Report

See:

**SOC-001-Windows-Authentication-Investigation.pdf**
