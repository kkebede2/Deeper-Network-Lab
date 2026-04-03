## 📌 Overview

Designed and implemented a segmented enterprise network using Cisco Packet Tracer.
This lab demonstrates Layer 2 and Layer 3 networking concepts including VLAN segmentation, inter-VLAN routing, dynamic routing with OSPF, DHCP services, access control lists, and secure device management using SSH.

---

## 🧠 Network Architecture

* Two routers (R1, R2) connected via point-to-point link
* Two access switches (SW1, SW2)
* Multiple VLANs across both sites
* Router-on-a-stick for inter-VLAN routing
* OSPF used for dynamic routing between routers

---

## 🧩 VLAN Design

| VLAN | Name       | Subnet (R1)     | Subnet (R2)      |
| ---- | ---------- | --------------- | ---------------- |
| 10   | HR         | 192.168.10.0/24 | 192.168.110.0/24 |
| 20   | IT         | 192.168.20.0/24 | 192.168.120.0/24 |
| 30   | Guest      | 192.168.30.0/24 | 192.168.130.0/24 |
| 99   | Management | 192.168.99.0/24 | N/A              |

---

## ⚙️ Technologies Used

* Cisco Packet Tracer
* VLANs (802.1Q)
* Inter-VLAN Routing (Router-on-a-Stick)
* OSPF (Single Area - Area 0)
* DHCP
* Access Control Lists (ACLs)
* SSH (Secure Management)
* Port Security Concepts

---


## 📁 Lab File

Download and open the Packet Tracer file:

[Download Lab](./deeper-network-lab.pkt)

---

## 🚀 Key Takeaways

* Implemented scalable enterprise network design
* Applied segmentation using VLANs and ACLs
* Secured management access using SSH + ACL restrictions
* Demonstrated dynamic routing with OSPF
* Built and validated full end-to-end connectivity

