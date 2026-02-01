# Log Data Flow — SIEM Pipeline

## Step-by-Step Flow

1. Windows VM generates Security, System, and Application events.
2. Splunk Universal Forwarder monitors Windows Event Logs.
3. Forwarder sends logs securely to Splunk Enterprise.
4. Splunk indexes logs into searchable datasets.
5. SOC analyst runs detection queries and creates alerts.
6. Dashboards visualize threats and suspicious behavior.

---

## Log Sources

| Source | Log Type | Purpose |
|--------|---------|--------|
| Windows VM | Security Logs | Authentication & access tracking |
| Windows VM | System Logs | System activity monitoring |
| Windows VM | Application Logs | Software behavior monitoring |

---

## Security Value
Ensures continuous monitoring and centralized visibility of endpoint activity.

