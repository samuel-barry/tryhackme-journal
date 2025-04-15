# 🧠 TryHackMe: HTTP in Detail  
**Date:** 2025-04-14  
**Pathway:** Pre-Security  
**Status:** ✅ Completed  

---

## 🔍 Task 1: What is HTTP(S)?

- **HTTP (HyperText Transfer Protocol)** is the protocol used to request and deliver web pages.
- **HTTPS** = HTTP + encryption via **TLS/SSL**, ensuring secure communication.
- Common use: browsing websites, APIs, form submission.
- 🔐 Flag from browser lock icon:  THM{INVALID_HTTP_CERT}
- 
---

## 🔁 Task 2: Requests and Responses

- HTTP works using a **request-response model** between client (browser) and server.
- Two key parts:
- **Request** → sent by the browser (GET, POST, etc.)
- **Response** → returned by the server
- 📌 Key answers:
- **Protocol used:** `HTTP/1.1`
- **Header that tells browser how much data to expect:** `Content-Length`

---

## 🧰 Task 3: HTTP Methods

| Action                        | Method |
|-------------------------------|--------|
| View a news article           | GET    |
| Create a user account         | POST   |
| Update your email             | PUT    |
| Delete an uploaded picture    | DELETE |

- These methods define what kind of action the client wants to perform on a resource.

---

## 📟 Task 4: HTTP Status Codes

| Code | Meaning               |
|------|------------------------|
| 201  | Created                |
| 404  | Not Found              |
| 503  | Service Unavailable    |
| 401  | Unauthorized (login required) |

- Status codes are returned in the **response** to describe the result of the request.

---

## 🧾 Task 5: Headers

- Headers pass metadata in both requests and responses.

| Header         | Purpose                               |
|----------------|----------------------------------------|
| `User-Agent`   | Tells the server what browser is used  |
| `Content-Type` | Describes the data being sent          |
| `Host`         | Specifies which website is being requested |

---

## 🍪 Task 6: Cookies

- Cookies store user-related data in the browser.
- Used for session management, preferences, and tracking.
- The server sets cookies using:

- 
