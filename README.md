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
