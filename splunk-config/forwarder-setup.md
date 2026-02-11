# Splunk Universal Forwarder Setup (Windows VM)

## Purpose
Collect logs from Windows VM and forward them to Splunk Enterprise.

---

## 1. Download & Install
1. Download Splunk Universal Forwarder for Windows:  
   [https://www.splunk.com/en_us/download/universal-forwarder.html](https://www.splunk.com/en_us/download/universal-forwarder.html)
2. Install with default settings.
3. Set **Admin username/password** and **start as service**.

---

## 2. Configure Forwarding to Splunk Indexer

Open **Command Prompt as Administrator**:

```cmd
cd "C:\Program Files\SplunkUniversalForwarder\bin"
splunk add forward-server <SPLUNK_INDEXER_IP>:9997 -auth admin:changeme
splunk enable boot-start
splunk restart

splunk list forward-server
splunk list monitor

