# 🧱 OSI Model (TryHackMe Notes)

---

## 🌐 What is the OSI Model?

The **OSI (Open Systems Interconnection)** model is a conceptual framework that standardizes how different networking protocols interact in 7 distinct layers.

---

## 🧬 7 Layers of OSI (Bottom to Top)

| Layer | Name             | Function |
|-------|------------------|----------|
| 1     | Physical         | Transmission of raw bits (e.g., cables, hubs) |
| 2     | Data Link        | MAC addresses, switches, Ethernet |
| 3     | Network          | IP addresses, routing (e.g., routers) |
| 4     | Transport         | TCP/UDP, reliability |
| 5     | Session          | Maintains connections |
| 6     | Presentation     | Translates data (encryption, compression) |
| 7     | Application      | Interfaces for the user (HTTP, DNS, etc.) |

---

## 🧠 Key Concepts

- **Encapsulation**: Each layer wraps data with its own headers.
- **TCP/IP Stack**: Often referenced alongside OSI (fewer layers).
- Real-world tools (like Wireshark) let you inspect traffic across these layers.

---

📌 **Key Takeaway**: The OSI model helps understand how data moves through a network and where different protocols and devices operate.
