# 🧠 TryHackMe: DNS in Detail  
**Date:** 2025-04-14  
**Pathway:** Pre-Security  

---

## 🔍 Task 1: What is DNS?

DNS (Domain Name System) is what makes the internet user-friendly.  
Instead of remembering IP addresses like `172.217.169.46`, we use names like `google.com`, and DNS handles the translation behind the scenes.

🔑 **Key Point**: It acts like the phonebook of the internet — matching domain names to IP addresses.

---

## 🏗️ Task 2: Domain Hierarchy

A domain name is structured **right-to-left**, starting with the top-level domain (TLD).

### 🧱 Structure Example:
`subdomain.domain.co.uk`  
- `.uk` – country-code TLD  
- `.co` – second-level domain  
- `domain` – main name  
- `subdomain` – optional prefix

🔑 **Takeaways**:
- Max subdomain length = **63 characters**
- Full domain max length = **253 characters**
- Can't use underscores `_` in subdomains
- `.co.uk` = **ccTLD** (country-code top-level domain)

---

## 📄 Task 3: DNS Record Types

DNS records define what information is returned when a DNS query is made.

### 📘 Key Record Types:
- `A`: Maps a domain to an **IPv4** address
- `AAAA`: Maps to an **IPv6** address
- `MX`: Specifies **mail server**
- `CNAME`: Canonical name / alias
- `TXT`: Human-readable info (e.g. SPF, verification)

🔑 **Takeaways**:
- `A` record = standard domain-to-IP mapping
- `MX` helps direct emails to the correct mail server
- `TXT` is used for things like domain verification

---

## 🔁 Task 4: Making a Request

The DNS resolution process is multi-step. Your system doesn't just know where a website is — it has to ask.

### 📡 The Request Chain:
1. You type a domain in your browser
2. The request goes to your **recursive DNS server** (usually from your ISP)
3. That server queries the internet to find the **authoritative DNS server**
4. It returns the **definitive answer**, like the IP address

🧠 **TTL** (Time To Live) controls how long this answer is cached to avoid doing this every time.

🔑 **Key Terms**:
- **Recursive DNS server**: does all the work to resolve your request
- **Authoritative DNS server**: the final source of truth
- **TTL**: how long to keep cached info before asking again

---

## 🧪 Task 5: Practical Queries

We use tools like `nslookup`, `dig`, or `host` to manually query DNS records.

### Commands:
```bash
nslookup -type=A www.website.thm
nslookup -type=CNAME shop.website.thm
nslookup -type=TXT website.thm
nslookup -type=MX website.thm
