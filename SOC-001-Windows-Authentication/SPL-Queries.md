# SPL Queries – SOC-001 Windows Authentication Investigation

This document contains the Splunk searches used during the Windows Authentication Investigation.

---

## 1. Successful Authentication Events

```spl
index=botsv3 EventCode=4624
```

Purpose

Retrieve all successful Windows logon events.

---

## 2. Failed Authentication Events

```spl
index=botsv3 EventCode=4625
```

Purpose

Retrieve all failed Windows logon events.

---

## 3. Authentication Baseline

```spl
index=botsv3 (EventCode=4624 OR EventCode=4625)
| stats count by EventCode
```

Purpose

Establish the number of successful and failed logon events.

---

## 4. Failed Logons by User

```spl
index=botsv3 EventCode=4625
| stats count by Account_Name
| sort -count
```

Purpose

Identify user accounts with failed authentication attempts.

---

## 5. Successful Logons by User

```spl
index=botsv3 EventCode=4624
| stats count by Account_Name
| sort -count
```

Purpose

Identify accounts with successful authentication events.

---

## Summary

These searches were used to establish a Windows authentication baseline and investigate authentication activity within the BOTS v3 dataset.
