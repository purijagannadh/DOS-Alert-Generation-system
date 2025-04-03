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
```

### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Configure Email Alerts**
Edit the config.py file and set up your email alerts:
```bash
EMAIL_SENDER = "your_email@gmail.com"
EMAIL_PASSWORD = "your_app_password"
THRESHOLD = 20  # Packets per second threshold
```

### **4️⃣ Run the Detection System**
```bash
python src/main.py
```
---

##📧 Email Alert Format
### **📌 Email Body:**
```yaml
A potential DoS attack has been detected.

🔹 Attacker IP: 192.168.1.100
🔹 Packets per Second: 50
🔹 Detection Time: 2024-04-03 14:25:30

Please take immediate action to prevent further damage.
```
