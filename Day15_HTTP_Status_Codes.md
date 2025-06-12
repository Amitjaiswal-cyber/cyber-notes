# 🌐 Day 15 – HTTP Status Codes

📅 **Date:** June 12, 2025  
🎯 **Topic:** Common HTTP Response Status Codes

---

## ✅ What Are HTTP Status Codes?

HTTP status codes are issued by a web server in response to a client's request. They help us understand if the request was successful, redirected, failed, or blocked.

In cybersecurity, analyzing these codes is essential during reconnaissance, web testing, and while using tools like **Burp Suite**, **Nmap**, **Nikto**, or **curl**.

---

## 🔢 Common Status Codes

| Code | Meaning                  | Use Case Example                      |
|------|--------------------------|---------------------------------------|
| 200  | OK                       | Page loads successfully               |
| 301  | Moved Permanently        | Old URL redirects to a new one        |
| 302  | Found (Temp Redirect)    | Login redirects to dashboard          |
| 400  | Bad Request              | Malformed request from browser/tool   |
| 401  | Unauthorized             | Login required                        |
| 403  | Forbidden                | Blocked by server (no access rights)  |
| 404  | Not Found                | Page or resource doesn't exist        |
| 500  | Internal Server Error    | Server encountered an issue           |
| 502  | Bad Gateway              | Server acting as a proxy failed       |
| 503  | Service Unavailable      | Server is overloaded or under maintenance |

---

## 🔍 Why Are These Important?
- When scanning or testing a web app, status codes help identify behavior and restrictions.
- For example:
  - `200 OK` confirms the resource exists.
  - `403` tells us the page exists but is protected.
  - `401` means authentication is needed.
  - `500` may indicate a misconfigured or vulnerable backend.

They are useful for both reconnaissance and vulnerability analysis.

---

## 🧪 Try This (Optional)
```bash
curl -I https://example.com
```
This will return the HTTP status code and headers.

