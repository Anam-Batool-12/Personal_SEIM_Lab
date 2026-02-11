# Detection Use Cases

This document summarizes all detection scenarios implemented in the SEIM Lab, along with Splunk queries, alerts, and practical use-cases.

---

## 1. Brute Force Detection

**Scenario:** Detect multiple failed login attempts on Windows VM via RDP.

**Splunk Query:**
```spl
host="DESKTOP-AELMUA7" index=* sourcetype=WinEventLog:Security
| search logon
| table _time, EventCode, *user*, *ip*
| stats count by *user*, *ip*
| where count > 5

