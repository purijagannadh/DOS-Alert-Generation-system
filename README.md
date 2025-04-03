# DOS-Alert-Generation-system
Enhanced Alert Generation System with Attacker IP for DOS Attacks

## 📚 Project Overview
The Enhanced Alert Generation System with Attacker IP for DoS Attacks is a real-time network monitoring system designed to detect Denial of Service (DoS) attacks. It identifies potential malicious activity based on packet thresholds, captures the attacker's IP address, and sends real-time email alerts to the network administrator. This system ensures prompt action against network threats while maintaining network performance integrity.
Upon detection, the system triggers email alerts containing:

- The **attacker’s IP address**.
- The **number of packets per second (PPS)**.
- The **detection time**.

## 🚀 Features
- ✅ **Real-Time Monitoring:** Continuously monitors network traffic for potential DoS attacks.
- ✅ **Attacker IP Detection:** Captures and displays the attacker's IP address upon detection.
- ✅ **Threshold-Based Alerts:** Triggers alerts when traffic surpasses a predefined packet threshold.
- ✅ **Email Notifications:** Sends detailed alerts via email for immediate action.
- ✅ **Customizable Parameters:** Allows adjustment of detection thresholds and monitoring configurations.

## 🛡️ System Requirements
- Ubuntu (Monitoring Machine)
- KaliLinux (Attacking Machine)
- Windows (victim)
- Python 3.x
- PyShark Library
- Internet Access (for sending email alerts)


---

## 💻 Installation Guide

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/yourusername/DOS-Alert-Generation-System.git
cd DOS-Alert-Generation-System
