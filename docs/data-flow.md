# Log Data Flow Explanation

1. Windows VM generates system & security logs.
2. Splunk Universal Forwarder collects event logs.
3. Logs are forwarded to Splunk Enterprise.
4. Splunk indexes logs into searchable indexes.
5. SOC analyst searches logs, creates alerts, and investigates incidents.

## Log Types Collected
- Security (Logon failures, authentication)
- System (Service events)
- Application (Software activity)

