# Brute-Force Login Detection

## Objective
Detect repeated failed Windows login attempts indicating a brute-force attack.

## Log Source
Windows Security Event Logs (EventCode 4625)

## Splunk Detection Query
```spl
index=* EventCode=4625
| stats count by TargetUserName, IpAddress
| where count > 5
| sort -count
Alert Logic

Trigger alert if more than 5 failed login attempts from the same IP within monitoring window
