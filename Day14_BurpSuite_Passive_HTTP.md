🔍 Day 14 – Burp Suite (Passive HTTP Analysis)

📅 Date: June 11, 2025
🎯 Goal: Capture and understand HTTP traffic between browser and server using Burp Suite


---

🧰 What is Burp Suite?

Burp Suite is a powerful tool used in web application security testing. It acts as an HTTP proxy that allows us to intercept, inspect, and analyze web traffic.

We use the Community Edition (free)

It helps us see all data exchanged between client (browser) and server



---

🧪 Setup Process

✅ 1. Install Burp Suite

Download from: https://portswigger.net/burp

Choose Community Edition


✅ 2. Configure Firefox Browser

Open Firefox > Settings > Network Settings

Use manual proxy:

HTTP Proxy: 127.0.0.1

Port: 8080


Check: "Use this proxy for all protocols"


✅ 3. Install Burp Certificate (for HTTPS traffic)

Visit: http://burp in the proxied browser

Download the certificate

Install it in browser > Certificates > Authorities



---

🌐 Test Activity

🔗 Visit:

https://example.com

https://httpbin.org


🔍 In Burp Suite:

Go to Proxy > HTTP history

Observe:

Method: GET / POST

Request headers (Host, User-Agent, Cookies)

Response headers (Server, Content-Type, Status Code)




---

📝 Observations

Field	Example

Method	GET
URL	https://httpbin.org/get
Status Code	200 OK
Server	ECS (dcb/7F47)
Content-Type	text/html or application/json
Cookies	(if any present)



---

📁 Notes Summary

✅ Installed and configured Burp Suite with Firefox

✅ Captured real HTTP traffic passively

✅ Understood headers and structure of web requests/responses



---

🔗 Resources

Burp Suite Documentation

YouTube: Burp Suite Tutorial (Hindi)

TryHackMe Room – Burp Suite Basics



---

📂 File Name: Day14_BurpSuite_Passive_HTTP.md 📌 To Upload: GitHub Repo → cyber-notes

