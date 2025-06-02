# OSI Model – Notes

The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a telecommunication or computing system into **7 layers**.

---

## 📚 7 Layers of the OSI Model

| Layer No | Name           | Function                                      | Example Protocols     |
|----------|----------------|-----------------------------------------------|------------------------|
| 7        | Application     | End-user interface, network services          | HTTP, FTP, DNS         |
| 6        | Presentation    | Data translation, encryption, compression     | SSL, TLS               |
| 5        | Session         | Establish/manage/terminate sessions           | NetBIOS, RPC           |
| 4        | Transport       | Reliable delivery, segmentation               | TCP, UDP               |
| 3        | Network         | Routing, logical addressing                   | IP, ICMP               |
| 2        | Data Link       | MAC addressing, error detection               | Ethernet, PPP          |
| 1        | Physical        | Raw bit transmission over physical media      | Cables, Hubs           |

---

## 🔑 Key Points

- Data goes from **Application (Layer 7)** down to **Physical (Layer 1)** when sending.
- On the receiving side, it goes from Layer 1 to Layer 7.
- Each layer serves the one above and is served by the one below.

---

## 🧠 Memory Trick

**"All People Seem To Need Data Processing"**  
*(Application, Presentation, Session, Transport, Network, Data Link, Physical)*

---

## ✅ Use Cases

- Troubleshooting network issues layer-by-layer.
- Understanding how data travels in a network.
- Comparing with TCP/IP model.

---

## 📎 Resources

- [NetworkChuck OSI Video](https://www.youtube.com/watch?v=vv4y_uOneC0)
- [Cisco Guide on OSI Model](https://www.cisco.com/)

