# Suspicious PowerShell Activity Detection

## Objective
Detect potentially malicious PowerShell commands executed on endpoints.

## Log Source
Windows PowerShell Logging

## Splunk Detection Query
```spl
index=* powershell CommandLine="*Invoke-WebRequest*"

