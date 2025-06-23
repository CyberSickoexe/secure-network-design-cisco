# 🔒 Secure Network Design - Cisco Packet Tracer Project

## 📡 Project Overview

This project implements a **Secure Network Design** using **Cisco Packet Tracer**, following industry best practices such as:

- VLAN segmentation
- Inter-VLAN Routing via Router-on-a-Stick
- Secure device management with SSH and encrypted passwords
- Access Control Lists (ACLs) for traffic control

---

## 🖥️ Device Assignment

| Device               | VLAN | IP Address       | Purpose         |
|----------------------|------|------------------|-----------------|
| PC0 (Admin)          | 10   | 192.168.10.10    | Admin Workstation |
| PC1 (Staff)          | 20   | 192.168.20.10    | Staff Workstation |
| PC2 (Server)         | 30   | 192.168.30.10    | Server           |
| Switch (Management)  | 99   | 192.168.99.2     | Switch Management |
| Router Sub-Interfaces|      |                  | Inter-VLAN Routing |
| - G0/0.10            | 10   | 192.168.10.1     | Admin Gateway    |
| - G0/0.20            | 20   | 192.168.20.1     | Staff Gateway    |
| - G0/0.30            | 30   | 192.168.30.1     | Server Gateway   |
| - G0/0.99            | 99   | 192.168.99.1     | Switch Management Gateway |

---

## 🗂️ VLAN Plan

| VLAN | Purpose    | Subnet            |
|------|------------|-------------------|
| 10   | Admin      | 192.168.10.0/24   |
| 20   | Staff      | 192.168.20.0/24   |
| 30   | Server     | 192.168.30.0/24   |
| 99   | Management | 192.168.99.0/24   |

---

## ⚙️ Configuration Steps

1. Place **Router**, **Switch**, **PC0**, **PC1**, and **PC2** in Cisco Packet Tracer.
2. Configure VLANs on the switch.
3. Assign switch ports to appropriate VLANs.
4. Configure Router sub-interfaces for Inter-VLAN Routing.
5. Assign static IP addresses to all devices.
6. Secure the Router and Switch with:
   - Passwords (console, vty, enable secret)
   - SSH access for remote management
   - Password encryption
7. Apply Access Control Lists (ACLs) to control network traffic as needed.
8. Test connectivity:
   - Ping between VLANs
   - SSH access to Router and Switch

---

## ✅ Features Implemented

- VLAN segmentation for improved security
- Inter-VLAN routing via Router-on-a-Stick
- Secure remote management with SSH
- Password and access protections on network devices
- ACLs to restrict unauthorized access
- Full network connectivity testing

---

## 🔍 Testing Summary

- Successful pings between:
  - PC0 ↔ PC1
  - PC0 ↔ PC2
  - PC1 ↔ PC2
- SSH access verified to:
  - Router
  - Switch
- ACL restrictions confirmed

---

## 📂 File Contents

- `secure-network-design.pkt` — Packet Tracer project file
- `README.md` — Project documentation

---

## 💡 Notes

This project is designed for **educational purposes**, demonstrating secure network design fundamentals using Cisco Packet Tracer.

