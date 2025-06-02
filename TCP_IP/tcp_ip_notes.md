# 🔐 Cybersecurity Learning – Day 2

## 📅 Date: May 28, 2025

---

### 📚 What I Studied:
- Watched: *TCP/IP Model Explained in Simple Terms*
- Read: TCP/IP 4-layer model and common protocols

### 🌐 TCP/IP Model Overview

| Layer           | Description                            | Example Protocols        |
|-----------------|----------------------------------------|--------------------------|
| Application     | Interface for applications             | HTTP, FTP, DNS, SMTP     |
| Transport       | Reliable delivery between hosts        | TCP, UDP                 |
| Internet        | Logical addressing and routing         | IP, ICMP, ARP            |
| Network Access  | Physical transmission of data          | Ethernet, Wi-Fi          |

---

### 🆚 OSI vs TCP/IP Model

| OSI Layer              | TCP/IP Layer        | Key Difference/Note                         |
|------------------------|---------------------|---------------------------------------------|
| Application            | Application         | TCP/IP combines 3 OSI layers into one       |
| Presentation           | -                   | Merged in TCP/IP Application                |
| Session                | -                   | Merged in TCP/IP Application                |
| Transport              | Transport           | TCP, UDP used in both                       |
| Network                | Internet            | IP addressing and routing                   |
| Data Link              | Network Access      | Same function as OSI                        |
| Physical               | Network Access      | Included in the bottom layer                |

---

### 📝 Notes:
- TCP/IP is more practical and used in real-world networking.
- OSI is a conceptual model, helpful for understanding networking layer-by-layer.

---



### 🧪 Topology:
- Devices:
  - PC1
  - PC2
  - Switch 2960
  - Router 2911
- Connections:
  - PC1 → Switch (FastEthernet0/1)
  - PC2 → Switch (FastEthernet0/2)
  - Switch → Router (GigabitEthernet0/0)

---

### 🌐 IP Configuration

| Device  | IP Address     | Subnet Mask     | Default Gateway |
|---------|----------------|-----------------|-----------------|
| PC1     | 192.168.10.2   | 255.255.255.0   | 192.168.10.1    |
| PC2     | 192.168.10.3   | 255.255.255.0   | 192.168.10.1    |
| Router G0/0 | 192.168.10.1 | 255.255.255.0 | -               |

---

### ✅ Ping Test Results:

From **PC1** to **PC2**:

C:\> ping 192.168.10.3

Reply from 192.168.10.3: bytes=32 time<1ms TTL=128

From **PC2** to **PC1**:

C:\> ping 192.168.10.2

Reply from 192.168.10.2: bytes=32 time<1ms TTL=128


📷 Screenshot:
![Screenshot 2025-05-27 213759](https://github.com/user-attachments/assets/5d332125-ee88-4dae-b976-e5d2d3c23962)

![Screenshot 2025-05-27 213707](https://github.com/user-attachments/assets/0fba782d-9395-4ae8-ba7f-e837c66a9db0)

![Screenshot 2025-05-27 213531](https://github.com/user-attachments/assets/9877f132-3236-49f6-a449-d83a4928f628)

![Screenshot 2025-05-27 213603](https://github.com/user-attachments/assets/d407d68c-b436-4c46-b68b-74a2232617cd)
