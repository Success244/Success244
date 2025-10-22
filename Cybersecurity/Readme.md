# 🛡️ Cybersecurity Portfolio – Katlego Molotsi  

[![OS](https://img.shields.io/badge/OS-Ubuntu_22.04-orange?logo=ubuntu)](https://ubuntu.com)
[![Tools](https://img.shields.io/badge/Tools-Nmap%20%7C%20Wireshark%20%7C%20Aircrack--ng%20%7C%20Tor-blue)](https://www.kali.org/tools/)
[![Firewall](https://img.shields.io/badge/Security-UFW%20Configured-brightgreen)](https://help.ubuntu.com/community/UFW)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

> “Security isn’t a product, it’s a continuous process — and Linux gives me full control over it.”  

---

## 🧭 Migration Journey: From Windows 11 → Ubuntu Linux  

In **September 2025**, I migrated from **Windows 11** to **Ubuntu Linux** to gain more **system control**, **security transparency**, and **privacy resilience**.  
Windows was a good start, but Ubuntu gave me **root access to knowledge** — the freedom to understand and secure every component of my machine.

### 🧩 Key Reasons for Migrating:
- Full control over system processes  
- Better privacy and data protection  
- Access to open-source cybersecurity tools  
- CLI-based precision for automation and monitoring  

---

## ⚙️ System Setup & Security Hardening  

After switching, I dedicated time to configuring Ubuntu for **maximum security**.  
With ChatGPT’s help, I learned to manage users, configure firewalls, and install ethical hacking tools.

### 🔐 1. Manage User Privileges
Add your user to the `sudo` group safely:

```bash

sudo usermod -aG sudo success
groups success
🧱 2. Configure the UFW Firewall

Set up the Uncomplicated Firewall (UFW) for inbound/outbound control:

sudo apt install ufw
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose


Examples of rule management:

# Allow only local web traffic on 8081
sudo ufw allow from 127.0.0.1 to any port 8081 proto tcp

# Deny printing service for security
sudo ufw deny 631/tcp

🧰 3. Install Essential Cybersecurity Tools

Tools I installed and use for network and system security:

sudo apt install nmap wireshark aircrack-ng vim tor


🔍 Purpose:

Nmap: Network scanning and reconnaissance

Wireshark: Packet analysis and network forensics

Aircrack-ng: Wireless network auditing

Tor: Anonymous and private browsing

🧩 4. System Hardening

I learned to reduce system exposure and perform regular audits.

# Disable guest login
sudo sh -c 'printf "[SeatDefaults]\nallow-guest=false\n" > /usr/share/lightdm/lightdm.conf.d/50-no-guest.conf'

# Keep system up to date
sudo apt update && sudo apt upgrade -y

# Perform a full system security audit
sudo apt install lynis -y
sudo lynis audit system

📡 5. Network Scanning & Ethical Hacking Practice

Authorized penetration testing on my personal lab network:

# Enable monitor mode
sudo airmon-ng start wlan0

# Scan available networks
sudo airodump-ng wlan0mon


⚠️ All activities are conducted ethically within authorized and isolated environments.

💡 Key Takeaways from My Transition
Lesson	Description
🧠 Knowledge	Learned how Linux handles permissions, users, and processes
🔐 Security Awareness	Understood privilege separation and least-access principles
⚙️ Efficiency	Became confident in CLI-based configurations and automation
🤖 AI Support	Learned to integrate AI guidance into real-world cybersecurity setup
📁 Repository Overview

This repository is part of my Cybersecurity Portfolio and contains:

🧩 Configuration files and setup scripts

🧠 Notes on ethical hacking and network defense

🔍 Experiment logs and system tests

🧰 Tools and utility documentation

🚀 Future Projects

🔸 Automate Ubuntu system hardening

🔸 Document Wireshark and Nmap analysis workflows

🔸 Build a secure VirtualBox lab with ISO-based VMs

🔸 Explore VPN routing, encryption, and zero-trust access

🧾 License

This repository is released under the MIT License.
Use responsibly, ethically, and within authorized networks.

👨‍💻 Author

Katlego Molotsi
Cybersecurity Learner & Linux Enthusiast
📍 Migrated to Ubuntu in September 2025
🌐 GitHub Profile

<p align="center"> <img src="https://img.shields.io/badge/Built%20with-Linux%20%26%20Coffee-black?logo=linux" /> </p> ```
