🔍 Day 11 – FTP Enumeration & Banner Grabbing

📅 Date: June 8, 2025
🎯 Topic: FTP Enumeration, Anonymous Login, and FTP Banner


---

1️⃣ What is FTP?

FTP (File Transfer Protocol) is a standard network protocol used to transfer files between a client and a server.

Default Port: 21 (control)

Optional Port: 20 (data)

Modes: Active and Passive



---

2️⃣ Why is FTP Important in Cybersecurity?

Misconfigured FTP servers often allow anonymous login

Exposed servers may leak sensitive data

Older FTP versions may be vulnerable to known exploits



---

3️⃣ Commands Used for Enumeration

ftp <target-ip>
# When prompted for username, use: anonymous

# Common FTP commands:
ls         # List directory contents
pwd        # Show current directory
cd <dir>   # Change directory
get <file> # Download file


---

4️⃣ Example: Anonymous Login Test

ftp 10.10.158.20
Connected to 10.10.158.20.
Name (10.10.158.20:root): anonymous
Password:
230 Logged on

✅ Successfully logged in using anonymous – server is misconfigured.


---

5️⃣ Banner Grabbing & Version Info

nmap -p21 --script=ftp-anon,ftp-bounce <target-ip>

Or connect and get:

220-FileZilla Server 0.9.60 beta
220-written by Tim Kosse
220 Please visit https://filezilla-project.org/

➡️ FTP Server: FileZilla 0.9.60
➡️ Operating System: Likely Windows (based on banner)


---

6️⃣ Security Risk Summary

Risk	Description

Anonymous login enabled	Allows access without authentication
Exposed version info	Attacker can search for vulnerabilities
Cleartext transmission	FTP sends credentials unencrypted
Possible file leakage	Publicly accessible sensitive files



---

✅ Summary

Learned about FTP ports and login

Tested for anonymous login

Retrieved FTP server banner info

Identified basic risks


📁 Next Step: Research if the version is vulnerable to any exploits (e.g., vsFTPd 2.3.4 backdoor).


---

📎 Resources:

TryHackMe – FTP Room

Nmap Scripts – FTP


