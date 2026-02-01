
# Suspicious Login Detection

## Objective
Identify logins from unusual sources or anomalous behavior.

## Log Source
Windows Security Event Logs (EventCode 4624)

## Splunk Detection Query
```spl
index=* EventCode=4624
| stats count by TargetUserName, IpAddress
| sort -count

