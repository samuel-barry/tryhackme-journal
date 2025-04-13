# 🔌 Understanding Ports (TryHackMe Notes)

---

## What Are Ports?

- **Ports** are logical endpoints for network communication.
- They allow multiple services to run on a single device by distinguishing traffic.
- Ports are identified by numbers ranging from 0 to 65535.

---

## Port Ranges

- **Well-Known Ports (0–1023):** Reserved for common services.
  - Example: Port 80 for HTTP, Port 443 for HTTPS.
- **Registered Ports (1024–49151):** Assigned for specific services by IANA.
- **Dynamic/Private Ports (49152–65535):** Used for ephemeral or private connections.

---

## TCP and UDP Ports

- **TCP (Transmission Control Protocol):**
  - Connection-oriented.
  - Ensures reliable data transmission.
  - Common TCP ports:
    - 80: HTTP
    - 443: HTTPS
    - 22: SSH
    - 25: SMTP

- **UDP (User Datagram Protocol):**
  - Connectionless.
  - Faster but less reliable.
  - Common UDP ports:
    - 53: DNS
    - 67/68: DHCP
    - 69: TFTP

---

## Practical Application

- In the *Packets & Frames* room, you used `nc` (netcat) to connect to IP `8.8.8.8` on port `1234`.
- This demonstrated how ports facilitate communication between devices.

---

## Key Takeaways

- Ports are essential for directing network traffic to the correct services.
- Understanding common ports aids in network configuration and troubleshooting.
- Tools like `netcat` can be used to test port connectivity.
