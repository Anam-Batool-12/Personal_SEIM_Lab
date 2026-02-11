# Brute Force SOC Dashboard

## Panels Included
- Failed login activity timeline
- Top attacking IP addresses
- Most targeted user accounts

### 1. Failed Logins by User
- Search:
```spl
index=* sourcetype=WinEventLog:Security EventCode=4625
| stats count by Account_Name

## Purpose
Provide SOC analysts with real-time visualization of authentication attacks.

## Outcome
Successfully visualized brute-force attack behavior in Splunk.

