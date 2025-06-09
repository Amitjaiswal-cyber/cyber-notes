# 🌐 Day 12 – DNS Basics & Enumeration

📅 **Date:** June 9, 2025  
🎯 **Topic:** Understanding DNS, Record Types, Enumeration Techniques, and Commands

---

## 🔎 1. What is DNS?

**DNS (Domain Name System)** is like the phonebook of the internet. It translates domain names (like `www.google.com`) into IP addresses (`142.250.77.132`) so browsers can load websites.

- DNS servers are queried automatically when you open a website.
- Without DNS, you'd need to remember IPs instead of names.

---

## 📦 2. Key DNS Record Types

| Record | Description                            | Example                       |
|--------|----------------------------------------|-------------------------------|
| A      | Maps domain to IPv4 address            | `google.com → 142.250.77.132` |
| AAAA   | Maps domain to IPv6 address            | `google.com → ::2004:abcd::`  |
| CNAME  | Alias for another domain               | `mail.example.com → gmail.com`|
| MX     | Mail exchange (email servers)          | `gmail.com → ALT1.GMAIL.COM`  |
| TXT    | Text info (SPF, verification records)  | `v=spf1 include:_spf.google.com` |
| NS     | Nameservers for the domain             | `ns1.example.com`             |
| SOA    | Start of authority (zone control info) | Master DNS info               |

---

## 🧪 3. Basic DNS Commands

### 🔹 `nslookup`

nslookup tryhackme.com
🔹 dig
bash
Copy
Edit
dig tryhackme.com ANY
dig +short tryhackme.com
dig MX gmail.com
dig TXT google.com
🔹 whois
bash
Copy
Edit
whois tesla.com
🔹 host
bash
Copy
Edit
host tryhackme.com
host -t mx google.com
## 🚀 4. DNS Enumeration (Recon Techniques)
## 🔍 What is DNS Enumeration?
Gathering DNS records and subdomains to map an organization’s digital footprint. Used in:

Penetration Testing

Bug Bounty

OSINT Investigations

## 📌 Methods:
Zone transfer (AXFR) if misconfigured

Subdomain brute-forcing

Reverse DNS lookup

Lookup of TXT, SPF, DMARC records

🔧 Tools:
Tool	Use
dnsenum	Enumerate DNS data, zone transfers
dnsrecon	DNS records, brute-forcing, Google scraping
sublist3r	Subdomain brute-forcing
crt.sh	Find subdomains via SSL cert transparency

## 📝 5. What To Practice Today
✅ Run nslookup and dig on:

tryhackme.com

tesla.com

google.com

## ✅ Identify:

A record (IP)

MX record

TXT record (SPF/verification)

✅ Try whois and host with -t flags

## ⚠️ 6. Security Risks in DNS
Risk	Description
DNS Zone Transfer (AXFR)	Misconfigured DNS servers leak full domain map
DNS Spoofing	Attacker sends fake DNS responses
DNS Tunneling	Exfiltrating data over DNS queries
Lack of DNSSEC	No signature verification

## ✅ Summary
Understood the DNS ecosystem and how name-to-IP resolution works

Practiced lookup tools: dig, nslookup, whois, host

Learned common DNS record types

Explored DNS enumeration tools and risks

