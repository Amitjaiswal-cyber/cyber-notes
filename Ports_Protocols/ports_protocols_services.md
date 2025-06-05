# 🛡️ Day 8 – Ports, Protocols, and Services

---

## 1. 🔢 Well-Known Ports

| Port | Protocol | Service     | Description                   |
|------|----------|-------------|-------------------------------|
| 21   | TCP      | FTP         | File Transfer Protocol        |
| 22   | TCP      | SSH         | Secure Shell (remote login)  |
| 23   | TCP      | Telnet      | Remote command-line access (insecure) |
| 25   | TCP      | SMTP        | Sending email                 |
| 53   | TCP/UDP  | DNS         | Domain Name System            |
| 67   | UDP      | DHCP        | Dynamic Host Configuration    |
| 68   | UDP      | DHCP        | DHCP Client                   |
| 80   | TCP      | HTTP        | Web browsing (insecure)       |
| 110  | TCP      | POP3        | Receiving emails              |
| 123  | UDP      | NTP         | Time synchronization          |
| 143  | TCP      | IMAP        | Internet Mail Access Protocol |
| 161  | UDP      | SNMP        | Monitoring devices            |
| 443  | TCP      | HTTPS       | Secure web browsing           |
| 445  | TCP      | SMB         | Windows file sharing          |
| 3389 | TCP      | RDP         | Remote Desktop Protocol       |

---

## 2. 🔁 TCP vs UDP

### 🧱 TCP (Transmission Control Protocol)
- ✅ Connection-oriented
- 🛡️ Reliable data delivery
- 🐢 Slower but ensures order & completeness
- 🔒 Common Uses: HTTP(S), SSH, SMTP, FTP

### 🚀 UDP (User Datagram Protocol)
- ❌ Connectionless
- ⚡ Fast and lightweight
- 🚫 No delivery guarantee or order
- 🎮 Common Uses: DNS, VoIP, Online Games, Streaming

---

## 3. 🧠 Real-Life Scenarios

- **FTP (21) open?**  
  → Try `anonymous` login. Might allow free file access.

- **SSH (22) open?**  
  → Bruteforce weak passwords using Hydra.

- **Telnet (23) open?**  
  → Very insecure. Older routers & devices might expose it.

- **SMB (445) open?**  
  → Windows vulnerability (like **EternalBlue** — WannaCry attack vector).

- **RDP (3389) open?**  
  → Possible brute-force or exploit with weak credentials.

---


