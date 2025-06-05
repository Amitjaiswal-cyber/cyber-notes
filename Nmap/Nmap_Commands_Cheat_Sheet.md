# 📌 Nmap Commands Cheat Sheet with Detailed Explanations

| Command | Description |
|--------|-------------|
| `nmap <IP>` | Basic Scan— This is the simplest Nmap command. It checks if the host is up and shows the open TCP ports. <br>🔍 **Use Case**: Quick overview of what services are running. <br>📝 **Example**: `nmap 192.168.1.1` <br>📌 **Note**: By default, it scans the top 1000 ports and uses a TCP connect or SYN scan depending on privileges. |
| `nmap -sS <IP>` | TCP SYN scan (stealth scan). Sends SYN packets and waits for SYN-ACK. Less likely to be logged by firewalls. Requires root privileges. |
| `nmap -sU <IP>` | UDP Scan — Scans UDP ports. Unlike TCP, UDP is connectionless, making this scan slower and less reliable but still important. <br>🔍 **Use Case**: To discover services like DNS (53), SNMP (161), and DHCP (67) that use UDP. <br>📝 **Example**: `nmap -sU 192.168.1.1` <br>⚠️ **Note**: UDP scans are slower and can give false positives due to ICMP filtering or timeouts. It's best to scan specific ports like `-p 53,67,161` instead of full range unless needed. |
| `nmap -sT <IP>` | TCP connect scan (full 3-way handshake). Used if SYN scan is not possible (e.g., non-root user). |
| `nmap -p <port> <IP>` | Scan a specific port or set of ports (e.g., `-p 22,80,443` or `-p 1-100`). |
| `nmap -p- <IP>` | Scan **all** 65535 ports. |
| `nmap -sV <IP>` | Version detection of services (e.g., Apache 2.4.7 on port 80). |
| `nmap -O <IP>` | OS detection using TCP/IP fingerprinting. |
| `nmap -A <IP>` | Aggressive scan (OS detection, version detection, script scanning, and traceroute). |
| `nmap -Pn <IP>` | Skip host discovery (assume target is up). Useful when ping is blocked. |
| `nmap -n <IP>` | Disable DNS resolution. Makes scan faster. |
| `nmap -T4 <IP>` | Timing template (T0 to T5). T4 is faster, good balance of speed & stealth. |
| `nmap --top-ports 100 <IP>` | Scan the top 100 most commonly used ports. |
| `nmap --script <script> <IP>` | Run a specific NSE script (e.g., `http-title`). |
| `nmap --script vuln <IP>` | Run all vulnerability detection scripts. Very useful for basic pentesting. |
| `nmap -oN output.txt <IP>` | Save results in a readable text file. |
| `nmap -oX output.xml <IP>` | Save results in XML format (for automation/reporting). |
| `nmap -iL targets.txt` | Scan multiple targets from a file (each line is an IP or hostname). |
| `nmap -6 <IPv6>` | Scan IPv6 addresses. |


