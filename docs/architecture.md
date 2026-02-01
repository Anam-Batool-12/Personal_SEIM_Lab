# SIEM Lab Architecture

## Components

### 1. Splunk Enterprise (Windows Host)
Role: Central SIEM for ingesting, indexing, and analyzing logs.

### 2. Windows VM (Universal Forwarder)
Role: Sends Windows Security, System, and Application logs to Splunk.

### 3. Kali Linux (Attacker)
Role: Simulates real-world attacks such as brute-force and reconnaissance.

## Data Flow
Windows Event Logs → Splunk Universal Forwarder → Splunk Enterprise → Detection & Alerts

## Objective
Create a realistic SOC environment to practice log analysis, detection engineering, and threat investigation.

