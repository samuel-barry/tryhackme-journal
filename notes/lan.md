# 🖧 LAN Concepts (TryHackMe Notes)

---

## 🔹 Network Topologies
- **Star Topology**: Common in LANs; all devices connect to a central switch.
- **Bus Topology**: Outdated; devices connected along a single cable.
- **Ring Topology**: Devices form a ring — not widely used in modern LANs.

---

## 🔹 Subnetting Basics
- **Subnet**: Logical subdivision of an IP network.
- Devices within the same subnet can communicate directly.
- **Subnet Mask**: Defines the size of the network.
  - Example: `255.255.255.0` (or `/24`) allows for 254 hosts.

---

## 🔹 ARP (Address Resolution Protocol)
- Resolves **IP addresses to MAC addresses**.
- Allows communication between devices on the same LAN.
- Uses a local **ARP table** to store recent mappings.

---

## 🔹 DHCP (Dynamic Host Configuration Protocol)
- Automatically assigns IP addresses to devices on a LAN.
- Prevents manual IP configuration.
- DHCP server leases out:
  - IP address
  - Subnet mask
  - Default gateway
  - DNS info

---

📌 **Key Takeaway**: A LAN uses common protocols (ARP, DHCP) and logical design (topologies, subnets) to allow devices to communicate efficiently without internet access.
