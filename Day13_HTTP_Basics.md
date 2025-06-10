# 🌐 Day 13 – HTTP Basics & Web Response Analysis

📅 **Date:** June 10, 2025  
🎯 **Topic:** Understanding HTTP Requests/Responses, Status Codes, and Basic Analysis

---

## 🔍 What is HTTP?

**HTTP (HyperText Transfer Protocol)** is the communication protocol used by web browsers and servers to exchange information.

- It is a **stateless** protocol (each request is independent).
- Operates over port **80 (HTTP)** and **443 (HTTPS)**.

---

## 🧾 HTTP Request Structure

When a browser sends a request, it typically includes:
- **Method** (e.g., GET, POST)
- **URL** (e.g., /index.html)
- **Headers** (User-Agent, Accept, Host, etc.)
- **Optional Body** (form data in POST)

### ✉️ Example:
```http
GET / HTTP/1.1
Host: example.com
User-Agent: Mozilla/5.0
Accept: text/html
```

---

## 📦 HTTP Response Structure

What the server sends back:
- **Status Line** (e.g., 200 OK)
- **Headers** (Content-Type, Server, Set-Cookie)
- **Body** (HTML, JSON, etc.)

### 🧾 Example:
```http
HTTP/1.1 200 OK
Content-Type: text/html
Content-Length: 1256
Server: nginx
```

---

## ✅ Common HTTP Methods

| Method | Purpose               |
|--------|------------------------|
| GET    | Retrieve data          |
| POST   | Submit data (e.g. forms) |
| PUT    | Update existing data   |
| DELETE | Remove data            |

---

## 📊 Common Status Codes

| Code | Meaning           |
|------|--------------------|
| 200  | OK                 |
| 301  | Moved Permanently |
| 302  | Found (Redirect)   |
| 400  | Bad Request        |
| 403  | Forbidden          |
| 404  | Not Found          |
| 500  | Internal Server Error |

---

## 🔧 Practice Activity

### Option A: Browser Dev Tools
1. Open Chrome → `F12` → Network tab
2. Visit `https://example.com`
3. Click on first request:
   - Check: **Request Method**, **Status Code**, **Content-Type**, **Response Headers**

### Option B: Terminal (Linux)
```bash
curl -I https://example.com
```

Or:
```bash
http https://example.com
```

---

## ✍️ Observations
- Request was `GET`, status code `200 OK`
- Server: `ECS (dcb/7F47)`
- Content-Type: `text/html`

---

## 📁 Notes Saved
Filename: `Day13_HTTP_Basics.md`
Location: GitHub Repo → `cyber-notes`

---

📚 **Resources:**
- [YouTube – NetworkChuck: HTTP Explained](https://www.youtube.com/watch?v=iYM2zFP3Zn0)
- [MDN Docs – HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP)
- [curl Documentation](https://curl.se/docs/manpage.html)
