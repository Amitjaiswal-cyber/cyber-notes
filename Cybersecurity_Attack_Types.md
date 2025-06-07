# 🔐 Top 10 Cybersecurity Attack Types – In Depth

> 📅 Date: June 7, 2025  
> 🧠 Author: Amit jaiswal
> 🎯 Objective: Understand common cyber attacks, real-world examples, and prevention strategies.

---

## 1. 🎣 Phishing

**Definition**: A technique to trick users into revealing sensitive information (like login credentials or credit card info) by impersonating trusted entities.

- **Example**: An attacker sends an email pretending to be PayPal, asking users to "verify their account" by clicking a malicious link.
- **Real Case**: In 2020, Twitter employees were phished, allowing attackers to access internal tools and hijack verified accounts.
- **Defense**:
  - User awareness training
  - Email spam filters
  - Multi-Factor Authentication (MFA)

---

## 2. 💉 SQL Injection (SQLi)

**Definition**: An attack where an attacker inserts malicious SQL code into a form input field to manipulate the database.

- **Example**: Inputting `admin' OR '1'='1` into a login field could bypass authentication.
- **Real Case**: In 2008, Heartland Payment Systems suffered a breach via SQLi, leaking millions of credit card records.
- **Defense**:
  - Use parameterized queries (prepared statements)
  - Avoid dynamic SQL queries
  - Input validation and sanitization

---

## 3. 🧼 Cross-Site Scripting (XSS)

**Definition**: Injecting malicious scripts into web pages that execute in users’ browsers.

- **Example**: `<script>alert('Hacked')</script>` injected into a blog comment section.
- **Real Case**: In 2014, eBay users were redirected to phishing sites via stored XSS vulnerabilities.
- **Defense**:
  - Sanitize all user inputs
  - Use Content Security Policy (CSP)
  - Escape output data in HTML/JS

---

## 4. 🕵️‍♂️ Man-in-the-Middle (MITM)

**Definition**: The attacker intercepts communications between two parties to steal or manipulate data.

- **Example**: A user logs into their bank on public Wi-Fi, and the attacker captures login credentials.
- **Real Case**: Superfish adware on Lenovo laptops (2015) allowed MITM by installing a rogue root certificate.
- **Defense**:
  - Use HTTPS/TLS encryption
  - Avoid public Wi-Fi without a VPN
  - Certificate pinning

---

## 5. 🔑 Brute Force Attack

**Definition**: Attempting to guess passwords by trying every possible combination.

- **Example**: Trying `admin123`, `password`, `qwerty`, etc. on login pages.
- **Real Case**: In 2013, attackers brute-forced 90,000 WordPress sites using known default credentials.
- **Defense**:
  - Implement account lockout after several failed attempts
  - Use strong password policies
  - Enable CAPTCHA and MFA

---

## 6. 🌊 Denial-of-Service (DoS) / Distributed Denial-of-Service (DDoS)

**Definition**: Flooding a server or network with traffic to make it unavailable to users.

- **Example**: A botnet floods a website with fake requests until it crashes.
- **Real Case**: Dyn DNS DDoS attack (2016) using IoT devices knocked down Twitter, Netflix, and Reddit.
- **Defense**:
  - Use DDoS protection services (Cloudflare, AWS Shield)
  - Rate limiting
  - Server hardening

---

## 7. 💣 Ransomware

**Definition**: Malware that encrypts the victim’s files and demands payment for the decryption key.

- **Example**: WannaCry ransomware encrypts files and asks for Bitcoin payment.
- **Real Case**: WannaCry attack (2017) affected 200,000+ systems including UK’s NHS.
- **Defense**:
  - Regular backups
  - Patch operating systems
  - Anti-malware protection

---

## 8. ⚡ Zero-Day Exploit

**Definition**: An attack that occurs before the software vendor has released a patch for a known vulnerability.

- **Example**: Attacker discovers a flaw in a popular browser and uses it to install malware before the fix is available.
- **Real Case**: Stuxnet worm used zero-day vulnerabilities to sabotage Iran’s nuclear centrifuges.
- **Defense**:
  - Continuous patch management
  - Threat detection systems
  - Behavior-based endpoint protection

---

## 9. 🎭 Social Engineering

**Definition**: Manipulating people into giving up confidential info or access.

- **Example**: An attacker calls IT pretending to be a manager needing a password reset.
- **Real Case**: Kevin Mitnick used social engineering to infiltrate companies in the 1990s.
- **Defense**:
  - Employee security awareness training
  - Verification procedures
  - No sharing passwords over calls/emails

---

## 10. 🔁 Credential Stuffing

**Definition**: Using leaked credentials from one site to log into another (relying on reused passwords).

- **Example**: An attacker uses stolen Netflix passwords to try logging into Gmail or Facebook.
- **Real Case**: Zoom suffered a credential stuffing attack in 2020 due to reused credentials from prior breaches.
- **Defense**:
  - Encourage users to use unique passwords
  - Monitor login attempts
  - Implement MFA

---

## 🛠️ Summary Table

| # | Attack Type         | Key Risk               | Main Defense                     |
|---|----------------------|------------------------|----------------------------------|
| 1 | Phishing             | Credential Theft       | Awareness, MFA                   |
| 2 | SQL Injection        | Database Breach        | Prepared Statements              |
| 3 | XSS                 | Script Execution        | Input Sanitization               |
| 4 | MITM                | Data Interception       | HTTPS, VPN                       |
| 5 | Brute Force         | Password Cracking       | Lockout, MFA                     |
| 6 | DoS/DDoS            | Service Downtime        | DDoS Protection, Rate Limiting   |
| 7 | Ransomware          | Data Loss               | Backups, Antivirus               |
| 8 | Zero-Day Exploit    | Unpatched Exploits      | Patch Quickly, Monitoring        |
| 9 | Social Engineering  | Human Manipulation      | Awareness, Verification          |
|10 | Credential Stuffing | Account Hijacking       | Unique Passwords, MFA            |

---

## 📚 Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [Have I Been Pwned](https://haveibeenpwned.com/)
- [TryHackMe - Introduction to Cybersecurity](https://tryhackme.com/room/introductiontocybersecurity)

