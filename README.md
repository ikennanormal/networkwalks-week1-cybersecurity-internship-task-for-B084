# IKENNA-networkwalks-week1-cybersecurity-internship-task-for-B084
My Cybersecurity lab setup
i have completed my cybersecurity lab internship set up, i have my vm box and kali ready for the upcoming task and activities we would be doing and learning



# 🔐 Cybersecurity Lab Environment Setup - Week 1

*Building an isolated virtual lab for penetration testing and ethical hacking practice*

---

## 📌 Project Overview
This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux. The purpose of the lab is to establish a controlled environment where cybersecurity tools, network scanning, reconnaissance, and vulnerability assessments can be performed safely and repeatedly.

---

## 🎯 Objectives
- Install and configure VirtualBox.
- Import and configure Kali Linux as a virtual machine.
- Set up a private **NAT Network** for lab isolation.
- Assign a static IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Create a clean VM baseline snapshot for recovery.

---

## ⚙️ Lab Configuration Summary

| Component | Configuration |
| :--- | :--- |
| **Host OS** | Windows / macOS / Linux |
| **Hypervisor** | VirtualBox |
| **Security OS** | Kali Linux |
| **Virtual Network** | NAT Network (`NatNetwork`) |
| **Network Address** | 10.0.0.0/24 |
| **Kali IP Address** | 10.0.0.2 |
| **Default Gateway** | 10.0.0.1 |
| **DNS Server** | 8.8.8.8 |

---

## 🪜 Lab Setup Steps

1. **VirtualBox Installation:** Installed the hypervisor to manage virtual machines.
2. **NAT Network Creation:** Created a dedicated NAT Network in VirtualBox to allow future attacker and target VMs to communicate internally while retaining outbound internet access.
3. **Kali Linux Import:** Imported the Kali Linux virtual machine and attached its network adapter to the newly created NAT Network.
4. **Static IP Configuration:** Configured a consistent IPv4 address (`10.0.0.2`) on the Kali VM for easier documentation and reference in upcoming tasks.
5. **VM Snapshot:** Took a clean baseline snapshot in VirtualBox to ensure an easy recovery point if future configurations break.

---

## 🔎 Lab Verification

| Test | Expected Result | Status |
| :--- | :--- | :--- |
| Check IP address (`ip a`) | Correct Kali IP displayed (`10.0.0.2`) | ✅ Passed |
| Test gateway (`ping 10.0.0.1`) | Successful replies | ✅ Passed |
| Test Internet (`ping 8.8.8.8`) | Successful replies | ✅ Passed |
| Test DNS (`nslookup networkwalks.com`) | Domain resolves successfully | ✅ Passed |

---

## 💡 What I Learned
- **NAT vs. NAT Network:** Understanding how a NAT Network enables multi-machine communication compared to standard NAT.
- **VM Networking:** Configuring virtual adapters to control inter-VM connectivity.
- **Static Addressing:** Assigning and troubleshooting static IP addresses and network gateways in Linux.
- **Snapshots:** The importance of creating baseline recovery points before performing experimental or risky security tasks.

---

## 👤 Author
* **Ikenna** 
* Program: Cybersecurity at Networkwalks
* Task: Week 01 - Cybersecurity Lab Setup

```


