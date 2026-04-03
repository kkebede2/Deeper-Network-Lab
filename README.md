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

## 🔍 Key Design Decisions

- VLAN segmentation used to isolate departments (HR, IT, Guest) and reduce broadcast domains
- OSPF chosen for scalability and dynamic routing between sites
- ACL implemented to restrict HR → IT traffic for security compliance
- Management VLAN used to separate administrative access from user traffic
- SSH configured with access-class to limit remote access to trusted networks only

---

## Key Takeaways

* Implemented scalable enterprise network design
* Applied segmentation using VLANs and ACLs
* Secured management access using SSH + ACL restrictions
* Demonstrated dynamic routing with OSPF
* Built and validated full end-to-end connectivity

---

## 🖧 Network Topology Explanation

- R1 and R2 act as distribution routers
- Each router connects to a local access switch (SW1, SW2)
- Trunk links carry VLAN traffic between switches and routers
- A point-to-point link (10.0.0.0/30) enables OSPF routing between routers

---

## 🏢 Real-World Scenario

This lab simulates a multi-department enterprise network where:
- HR, IT, and Guest users are segmented via VLANs
- Traffic between departments is controlled via ACLs
- Routing between sites is handled dynamically using OSPF
- Secure remote management is enforced using SSH

---

## 📁 Lab File

Download and open the Packet Tracer file:

[Download Lab](./deeper-network-lab.pkt)

---

## 📸 Screenshots

### 🖥️ Network Topology
[Topology](./screenshots/topology.png)

### 🔀 VLAN Configuration
[VLAN](./screenshots/vlan-config.png)

### 🔗 Trunking
[Trunk](./screenshots/trunk.png)

### 🌐 OSPF Routing
[OSPF](./screenshots/ospf-routing.png)

### ✅ Inter-VLAN Communication
[InterVLAN](./screenshots/intervlan-success.png)

### ❌ ACL Blocking
[ACL](./screenshots/acl-block.png)

### 🔐 SSH Access
[SSH](./screenshots/ssh-success.png)

### 🛠️ Management VLAN
[Mgmt](./screenshots/management-vlan.png)
