# SPL Queries

## Authentication Baseline

```spl
index=botsv3 source="WinEventLog:Security"
(EventCode=4624 OR EventCode=4625)
| stats count by EventCode
```

## Notes

These queries were used during the investigation to identify successful and failed authentication events.
```
