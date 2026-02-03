<img width="1512" height="982" alt="Screenshot 2026-02-02 at 7 45 46 PM" src="https://github.com/user-attachments/assets/b163c3bb-ccd0-4935-8f58-a7a65c6e69b9" />
![IMG_1891](https://github.com/user-attachments/assets/b9c82c26-b710-46e7-9bca-553df82cff31)
![IMG_1892](https://github.com/user-attachments/assets/0beb67b9-ff4e-4416-9476-9ab8abf37081)
<img width="1512" height="982" alt="6f44a3e22a760bf52887e14e99bc3e8030b3c7618dd663313fc8e120cd84e2d8" src="https://github.com/user-attachments/assets/33eff3d3-2cd9-400b-8912-1ce4f7182be3" />
# Linux Network & Security Lab (Ubuntu VM)

## 📌 Overview
This project documents a hands-on Linux networking and security lab performed on an Ubuntu virtual machine.  
The goal of this lab is to understand how Linux systems communicate on a network, how traffic flows, and how basic security controls are applied and verified.

---

## 🖥️ Lab Environment
- OS: Ubuntu (VM)
- Virtualization: QEMU / UTM
- Network Interface: enp0s1
- Firewall: UFW
- SSH: OpenSSH Server

---

## 🛠️ Tools & Commands Used

### Network Diagnostics
- `ip a`
- `ip route`
- `ping`
- `dig`
- `curl`
- `traceroute`

### Traffic Analysis
- `tcpdump`

### Security & Services
- `ufw`
- `systemctl`
- `ssh`

---

## 🔍 What I Practiced & Verified

### 1️⃣ IP Addressing & Routing
- Verified interface configuration using `ip a`
- Identified default gateway and routing table using `ip route`
- Understood subnet masks (e.g., `/24 = 255.255.255.0`)

### 2️⃣ Connectivity Testing
- Tested ICMP reachability with `ping`
- Resolved DNS records using `dig`
- Inspected HTTP/HTTPS headers with `curl`
- Traced packet paths across the network with `traceroute`

### 3️⃣ Packet Capture & Traffic Visibility
- Used `tcpdump` to observe:
  - DNS queries (UDP 53)
  - HTTP (80) and HTTPS (443) traffic
- Confirmed real-time traffic flow beyond high-level tools

### 4️⃣ Firewall Hardening (UFW)
- Set default policies:
  - Deny incoming traffic
  - Allow outgoing traffic
- Enabled logging and monitored events in `/var/log/ufw.log`
- Observed allowed and audited traffic in real time

### 5️⃣ SSH Service Validation
- Verified SSH service state with `systemctl`
- Identified inactive service and socket-based activation
- Properly enabled and started `ssh.service`
- Confirmed SSH port behavior from an external system

---

## 🧠 Key Takeaways
- Packet-level visibility (tcpdump) reveals details that basic tools cannot
- Firewalls control traffic, but logs are critical for validation
- Services must be running *and* listening to be reachable
- Networking, security, and services are tightly connected in Linux

---

## 🚀 Next Steps
- Phase 2: Network segmentation & firewall rule refinement
- Phase 3: pfSense integration & Zero Trust concepts
- Additional logging and attack simulation labs

---

## 📸 Screenshots
Screenshots from the lab session are included to demonstrate commands, outputs, and traffic analysis.

---

**Always learning, practicing, and documenting real-world skills.**# linux-network-security-lab
Hands-on Ubuntu VM lab: networking diagnostics (ping/dig/curl/traceroute), packet capture (tcpdump), firewall hardening (UFW), and SSH service validation.
<img width="1512" height="982" alt="Screenshot 2026-02-02 at 7 46 44 PM" src="https://github.com/user-attachments/assets/1f918a16-8267-439a-87ba-48db0881e5d5" />
<img width="1512" height="982" alt="Screenshot 2026-02-02 at 7 47 03 PM" src="https://github.com/user-attachments/assets/b58c3248-f1f8-45f4-a61b-b16c23a601f1" />
<img width="1512" height="982" alt="Screenshot 2026-02-02 at 7 47 16 PM" src="https://github.com/user-attachments/assets/82f21d2b-ef73-497d-bbe4-420b485b2754" />
<img width="1512" height="982" alt="Screenshot 2026-02-02 at 7 47 33 PM" src="https://github.com/user-attachments/assets/cdd1139b-01a7-4717-bdb9-be3a4cf3dba5" />
