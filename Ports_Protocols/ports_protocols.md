# 🔌 Ports and Protocols

Understanding ports and protocols is essential in cybersecurity for identifying network traffic and detecting potential threats. 
This guide covers the most commonly used ports, their associated protocols, services, and whether they use TCP or UDP.

---

## 📋 Common Ports and Their Services

| Port | Protocol | Service Description                      | TCP/UDP |  
|------|----------|-------------------------------------------|---------|  
| 20   | FTP      | File Transfer Protocol (Data)             | TCP     |  
| 21   | FTP      | File Transfer Protocol (Control)          | TCP     |  
| 22   | SSH      | Secure Shell for secure login             | TCP     |  
| 23   | Telnet   | Remote login without encryption           | TCP     |  
| 25   | SMTP     | Simple Mail Transfer Protocol             | TCP     |  
| 53   | DNS      | Domain Name System                        | TCP/UDP |  
| 67   | DHCP     | Dynamic Host Configuration Protocol (Server) | UDP  |  
| 68   | DHCP     | Dynamic Host Configuration Protocol (Client) | UDP  |  
| 69   | TFTP     | Trivial File Transfer Protocol            | UDP     |  
| 80   | HTTP     | HyperText Transfer Protocol (Web)         | TCP     |  
| 110  | POP3     | Post Office Protocol v3 (Receive Email)   | TCP     |  
| 123  | NTP      | Network Time Protocol                     | UDP     |  
| 137  | NetBIOS  | Name Service                              | UDP     |  
| 138  | NetBIOS  | Datagram Service                          | UDP     |  
| 139  | NetBIOS  | Session Service                           | TCP     |  
| 143  | IMAP     | Internet Message Access Protocol          | TCP     |  
| 161  | SNMP     | Simple Network Management Protocol        | UDP     |  
| 443  | HTTPS    | Secure HTTP using SSL/TLS                 | TCP     |  
| 445  | SMB      | Server Message Block (Windows file sharing) | TCP   |  
| 993  | IMAPS    | IMAP over SSL                             | TCP     |  
| 995  | POP3S    | POP3 over SSL                             | TCP     |  
| 3306 | MySQL    | MySQL Database Service                    | TCP     |  
| 3389 | RDP      | Remote Desktop Protocol                   | TCP     |  

---

## 🧠 TCP vs UDP: Key Differences

| Feature             | TCP                              | UDP                            |  
|---------------------|----------------------------------|--------------------------------|  
| Connection          | Connection-oriented              | Connectionless                 |  
| Reliability         | Reliable (ensures delivery)      | Unreliable (no guarantee)      |  
| Speed               | Slower due to error checking     | Faster                         |  
| Use Cases           | Email, Web, File Transfers       | Streaming, DNS, VoIP           |  

---

## 📚 Tips for Remembering Ports

- **80 = HTTP (default web)**
- **443 = HTTPS (secure web)**
- **22 = SSH (secure remote login)**
- **25 = SMTP (email sending)**
- **53 = DNS (domain resolution)**

---

## 📌 Why This Matters in Cybersecurity

- Identifying **open ports** on a system helps detect vulnerable services.
- Malware often uses **non-standard ports** to avoid detection.
- Port scanning (e.g., using Nmap) is a core technique in **reconnaissance**.

---

📅 **Date Completed:** June 1, 2025  
✍️ **Author:** Amit Jaiswal  
🔗 [GitHub Repo](https://github.com/Amitjaiswal-cyber/cyber-notes)
