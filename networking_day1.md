# 🧠 Networking Day 1 – Basic Topology: 2 PCs and 1 Switch

## 📅 Date: [26 May 2025]

---

## 🖥️ Topology Setup

- Devices Used:
  - PC1
  - PC2
  - Switch 2960
- Connections:
  - PC1 → Switch (FastEthernet0/1)
  - PC2 → Switch (FastEthernet0/2)
- Cable Type: Copper Straight-Through

---

## 🌐 IP Configuration

| Device | IP Address     | Subnet Mask     |
|--------|----------------|-----------------|
| PC1    | 192.168.1.1    | 255.255.255.0   |
| PC2    | 192.168.1.2    | 255.255.255.0   |

---

## ✅ Ping Test Results

### From PC1:

C:\> ping 192.168.1.2

Reply from 192.168.1.2: bytes=32 time<1ms TTL=128
Reply from 192.168.1.2: bytes=32 time<1ms TTL=128

### From PC2:

C:\> ping 192.168.1.1

Reply from 192.168.1.1: bytes=32 time<1ms TTL=128
Reply from 192.168.1.1: bytes=32 time<1ms TTL=128


📸 Screenshots

![Screenshot 2025-05-26 205843](https://github.com/user-attachments/assets/bc246193-e9be-4c67-a0fb-ea5de85a1121)
![Screenshot 2025-05-26 205709](https://github.com/user-attachments/assets/41292bf5-5b04-41c8-b23b-fc6262f551a8)
![Screenshot 2025-05-26 205843](https://github.com/user-attachments/assets/03f2b847-3223-4f75-8897-3b6bad9fd674)

