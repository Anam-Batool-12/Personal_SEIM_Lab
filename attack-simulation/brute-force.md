# Brute-Force Login Attack Simulation

## Objective
Simulate repeated failed login attempts to generate detectable attack events in Splunk.

## Tools Used
- Kali Linux
- Hydra (for RDP simulation)
- Windows command line / PowerShell for safe lab simulation

## Commands Executed

### Option 1 — Hydra (RDP)
```bash
hydra -t 1 -W 3 -l administrator -P /usr/share/wordlists/rockyou.txt rdp://192.168.x.x

