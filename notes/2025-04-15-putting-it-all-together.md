# 🧠 TryHackMe: Putting It All Together  
**Date:** 2025-04-15  
**Pathway:** Pre-Security  
**Status:** ✅ Completed  

---

## 🧩 Task 1: Putting It All Together

This task served as a recap of the concepts covered in the Pre-Security path. It emphasized how various components like DNS, HTTP, and web servers interact when accessing a website.

---

## 🌐 Task 2: Other Components

This section introduced additional elements that play crucial roles in web infrastructure:

- **CDN (Content Delivery Network):** Distributes static content across multiple servers worldwide to reduce latency and improve load times.

- **Load Balancer:** Distributes incoming traffic across multiple servers to ensure reliability and performance. It performs **health checks** to verify server availability.

- **WAF (Web Application Firewall):** Protects web applications by filtering and monitoring HTTP traffic, defending against common attacks.

**Key Takeaways:**
- **What can be used to host static files and speed up a client's visit to a website?**  
  `CDN`

- **What does a load balancer perform to make sure a host is still alive?**  
  `Health Check`

- **What can be used to help against the hacking of a website?**  
  `WAF`

---

## 🖥️ Task 3: How Web Servers Work

This task delved into the workings of web servers and related concepts:

- **Web Server:** Software that handles HTTP requests and serves content to clients. Examples include Apache and Nginx.

- **Virtual Hosts:** Allow a single web server to host multiple domain names on the same IP address by directing requests to different directories based on the requested hostname.

- **Static vs. Dynamic Content:**
  - *Static Content:* Unchanging files like HTML, CSS, and images.
  - *Dynamic Content:* Content generated on-the-fly based on user interaction or other factors, often involving backend processing.

- **Backend Languages:** Languages like PHP, Python, and Node.js that run on the server to generate dynamic content. Importantly, the client does not see the backend code.

**Key Takeaways:**
- **What does web server software use to host multiple sites?**  
  `Virtual Hosts`

- **What is the name for the type of content that can change?**  
  `Dynamic`

- **Does the client see the backend code? Yay/Nay**  
  `Nay`

---

## 🧪 Task 4: Quiz

This interactive task tested the understanding of the web request process. By arranging the steps in the correct order, it reinforced the flow from entering a URL to rendering a webpage.

**Flag Obtained:**  
`THM{YOU_GOT_THE_ORDER}`

---

## ✅ Final Thoughts

This room effectively consolidated the knowledge from previous modules, providing a comprehensive overview of how different web components interact. It reinforced the importance of each element in delivering and securing web content.

