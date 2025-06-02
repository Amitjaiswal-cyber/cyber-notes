# 🌐 Networking Day 3 – IP Addressing & Subnetting

## 📅 Date: 2025-05-29  
## 🧠 Topic: IP Addressing and Subnetting

---

## 📘 What is an IP Address?

An **IP address** is a unique identifier assigned to each device on a network.  
It allows devices to communicate with each other across local and public networks.

- IPv4: 32-bit numeric address written as `x.x.x.x` (e.g., `192.168.1.1`)
- IPv6: 128-bit alphanumeric address (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`)

---

## 📊 IPv4 Address Classes

| Class | Starting Bits | Range             | Default Subnet Mask   | Used For         |
|-------|----------------|------------------|------------------------|------------------|
| A     | 0              | 1.0.0.0 – 126.255.255.255 | 255.0.0.0         | Large networks   |
| B     | 10             | 128.0.0.0 – 191.255.255.255 | 255.255.0.0     | Medium networks  |
| C     | 110            | 192.0.0.0 – 223.255.255.255 | 255.255.255.0   | Small networks   |
| D     | 1110           | 224.0.0.0 – 239.255.255.255 | N/A             | Multicasting     |
| E     | 1111           | 240.0.0.0 – 255.255.255.255 | N/A             | Reserved/Research|

---

## 🔒 Private IP Address Ranges

| Class | Private IP Range                |
|-------|---------------------------------|
| A     | 10.0.0.0 – 10.255.255.255       |
| B     | 172.16.0.0 – 172.31.255.255     |
| C     | 192.168.0.0 – 192.168.255.255   |

These ranges are **not routable** on the public internet and used within LANs.

---

## ✂️ What is Subnetting?

Subnetting is the process of dividing a large network into smaller, manageable sub-networks (subnets).  
It helps optimize IP allocation and improve security and performance.

### Example:
- IP: `192.168.1.0`
- Subnet Mask: `255.255.255.0` → /24
- Usable Hosts: 254

---

## 📏 CIDR Notation & Subnet Masks

| CIDR | Subnet Mask       | Hosts per Subnet |
|------|-------------------|------------------|
| /8   | 255.0.0.0         | 16,777,214       |
| /16  | 255.255.0.0       | 65,534           |
| /24  | 255.255.255.0     | 254              |
| /30  | 255.255.255.252   | 2                |

---

## 🔧 Tools Used

- ✅ **TryHackMe Module**: Introduction to Subnetting
- ✅ **YouTube**: NetworkChuck – Subnetting Explained
- ✅ **Subnet Calculator**: https://www.subnet-calculator.com

---

## ✍️ Key Takeaways

- IP addresses identify devices; subnetting organizes networks.
- Use CIDR to write subnet masks concisely.
- Understand classes & private IP ranges for real-world config.
- Subnetting improves network performance and efficiency.

