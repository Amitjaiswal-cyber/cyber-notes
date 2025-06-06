# 🔐 Password Hashing in Python

This document covers how to hash passwords securely using `hashlib` and `bcrypt` in Python.

---

## 📌 Why Hash Passwords?

Hashing converts plain text passwords into a fixed-length string, making it impossible to retrieve the original password from the hash. It's essential for securely storing user credentials.

---

## 🧪 1. Using `hashlib` (NOT RECOMMENDED for real apps)


import hashlib

# Simple SHA-256 hashing
password = b"mypassword"
hashed = hashlib.sha256(password).hexdigest()

print("SHA-256 Hashed Password:", hashed)
✅ Note: While hashlib is simple, it's not secure for real-world password storage because it lacks salting and work factor.

# ✅ 2. Using bcrypt (RECOMMENDED)
python
Copy
Edit
import bcrypt

# Create a password hash
password = b"mypassword"
hashed = bcrypt.hashpw(password, bcrypt.gensalt())

print("Bcrypt Hashed Password:", hashed)
# 🔁 Verifying Passwords
python
Copy
Edit
# User login: verify password
if bcrypt.checkpw(password, hashed):
    print("✅ Password is correct")
else:
    print("❌ Incorrect password")
⚠️ Best Practices
Always use bcrypt or argon2 for password storage.

Never store plain text passwords.

Use a strong salt and store only the hash (not the password).

Add rate-limiting and 2FA for extra security.

# 📚 References
bcrypt documentation

OWASP Password Storage Cheat Sheet
