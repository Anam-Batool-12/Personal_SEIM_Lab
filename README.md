# SIEM Lab — Splunk Security Monitoring Project

## Overview
This project demonstrates a hands-on Security Operations Center (SOC) lab using Splunk.  
It simulates real-world cyber attacks, collects Windows event logs, and builds detection rules and alerts.

## Lab Architecture
- Splunk Enterprise (Windows Host) — SIEM Server  
- Splunk Universal Forwarder (Windows VM) — Log Source  
- Kali Linux — Attacker Machine  

## Key Skills Demonstrated
- Windows log ingestion & monitoring
- Attack simulation (Brute-force, Recon, PowerShell abuse)
- Detection engineering in Splunk
- Alert creation & SOC investigation workflows
- Security event analysis & reporting

## Attacks Simulated
- Brute-force login attempts
- Port scanning (Nmap)
- Suspicious PowerShell activity

## Detections Built
- Failed login spike detection
- Suspicious PowerShell execution alerts
- Recon activity monitoring

## Goal
Showcase SOC analyst skills for internships, jobs, and cybersecurity portfolios.
