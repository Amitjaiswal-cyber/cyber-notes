# 🛡️ Day 4: Nmap Commands and Scans

📅 **Date**: June 3, 2025  
🎯 **Goal**: Understand and practice various Nmap scanning techniques.

---

## ✅ Target IP: `10.10.158.20`

---

## 🔎 Basic Scan


nmap 10.10.158.20
Result:

Shows open ports: 21 (ftp), 53 (domain), 80 (http), 135 (msrpc), 3389 (rdp)

## ⚡ SYN Scan (Stealth Scan)
bash
Copy
Edit
nmap -sS 10.10.158.20
Faster and stealthier than basic scan

Same open ports detected

## 🔍 Service Version Detection
bash
Copy
Edit
nmap -sV 10.10.158.20
Result:

FTP: FileZilla ftpd

HTTP: Microsoft IIS httpd 10.0

RPC: Microsoft Windows RPC

RDP: Microsoft Terminal Services

## 🎯 Aggressive Scan
bash
Copy
Edit
nmap -A 10.10.158.20
Info Found:

Anonymous FTP access allowed

HTTP TRACE method enabled

Web server: Microsoft-IIS/10.0

OS info: Windows Server 10.0.17763

RDP Info: NetBIOS + DNS + Product Version

SSL certificate data

## 🧠 OS Detection
bash
Copy
Edit
nmap -O 10.10.158.20
Guessed OS: AVtech Room Alert (not accurate)

May be unreliable due to missing closed port

## ❌ Incorrect Flag Example
bash
Copy
Edit
nmap -P 10.10.158.20
⚠️ Invalid usage (-P is not a valid Nmap flag for scanning)

## 📂 FTP Anonymous Login Test
bash
Copy
Edit
ftp 10.10.158.20
Steps:

Username: anonymous

Logged in successfully

Tried ls, cd html, cd pub but no access

Passive mode failed

Disconnected later

## 📌 Key Learnings
Use -sS for stealth scan

Use -sV and -A for detailed information

Anonymous FTP access can be a vulnerability

Understand active vs passive FTP

OS detection needs both open and closed ports

