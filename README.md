# DOS-Alert-Generation-system
Enhanced Alert Generation System with Attacker IP for DOS Attacks

## 📚 Project Overview
The Enhanced Alert Generation System with Attacker IP for DoS Attacks is a real-time network monitoring system designed to detect Denial of Service (DoS) attacks. It identifies potential malicious activity based on packet thresholds, captures the attacker's IP address, and sends real-time email alerts to the network administrator. This system ensures prompt action against network threats while maintaining network performance integrity.
Upon detection, the system triggers email alerts containing:

The attacker’s IP address.

The number of packets per second (PPS).

The detection time.

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

DOS-Alert-Generation-System

🚀 Enhanced Alert Generation System with Attacker IP for DoS Attacks

📚 Project Overview

The Enhanced Alert Generation System with Attacker IP for DoS Attacks is a real-time network monitoring system designed to detect Denial of Service (DoS) attacks. It identifies potential malicious activity based on packet thresholds, captures the attacker's IP address, and sends real-time email alerts to the network administrator. This system ensures prompt action against network threats while maintaining network performance integrity.

Upon detection, the system triggers email alerts containing:

The attacker’s IP address

The number of packets per second (PPS)

The detection time

🚀 Features

✅ Real-Time Monitoring: Continuously monitors network traffic for potential DoS attacks.

✅ Attacker IP Detection: Captures and displays the attacker's IP address upon detection.

✅ Threshold-Based Alerts: Triggers alerts when traffic surpasses a predefined packet threshold.

✅ Email Notifications: Sends detailed alerts via email for immediate action.

✅ Customizable Parameters: Allows adjustment of detection thresholds and monitoring configurations.

🛡️ System Requirements

Ubuntu (Monitoring Machine)

Kali Linux (Attacking Machine)

Windows (Victim)

Python 3.x

PyShark Library

Internet Access (for sending email alerts)

📂 Project Structure

/Enhanced-DoS-Detection-System
│── /docs                     # Documentation (Thesis, Paper, etc.)
│── /src                      # Source code for the detection system
│   ├── main.py               # Main script for running detection
│   ├── config.py             # Configuration settings
│   ├── email_alert.py        # Sends email alerts
│   ├── dos_detection.py      # DoS attack detection logic
│   ├── packet_sniffer.py     # Network packet sniffing using Pyshark
│── /tests                    # Test cases and validation scripts
│── /results                  # Logs and stored detection reports
│── .gitignore                # Exclude unnecessary files from GitHub
│── README.md                 # Project overview and instructions
│── requirements.txt          # Dependencies for setting up the project

🖥️ Installation Guide

💡 Step 1: Clone the Repository

git clone https://github.com/yourusername/Enhanced-DoS-Detection-System.git
cd Enhanced-DoS-Detection-System

💡 Step 2: Install Dependencies

Make sure Python 3.8+ is installed. Then, install the required libraries:

pip install -r requirements.txt

💡 Step 3: Configure Email Alerts

Edit the config.py file to set up your email alerts:

EMAIL_SENDER = "your_email@gmail.com"
EMAIL_PASSWORD = "your_app_password"
THRESHOLD = 20  # Packets per second threshold

💡 Step 4: Run the Detection System

Execute the main script to start monitoring network traffic:

python src/main.py

You should see:

Monitoring network traffic for DoS attack...

📊 Usage Instructions

Start the system → The script will monitor incoming network traffic in real-time.

Threshold-based detection → If packets exceed the set threshold (e.g., 20 packets/sec), it flags a potential DoS attack.

Alert Generation → If an attack is detected:

The attacker's IP address is extracted.

An email alert is sent to the administrator.

The event is logged in results/logs.txt.

Continuous Monitoring → The system keeps checking traffic and sends repeated alerts if the attack persists.

📧 Email Alert Format

Upon detection, the system sends an email in this format:

📌 Subject:

Alert: Potential DoS Attack Detected

📌 Email Body:

A potential DoS attack has been detected.

🔹 Attacker IP: 192.168.1.100
🔹 Packets per Second: 50
🔹 Detection Time: 2024-04-03 14:25:30

Please take immediate action to prevent further damage.

📝 Testing

To test the detection system:

Use hping3 (on Linux/Kali) to simulate a DoS attack:

hping3 -S --flood -p 80 <target_ip>

The system should detect the attack and send alerts.

Check logs in the /results folder for detected attack details.

🛠️ Troubleshooting

🛑 No emails received? ✔️ Ensure less secure apps access is enabled in Gmail or use an App Password. ✔️ Check internet connectivity and SMTP settings in config.py.

🛑 No attack detection? ✔️ Try lowering the packet count threshold in config.py. ✔️ Ensure Pyshark is properly installed and has access to network traffic.

📚 License

This project is open-source under the MIT License. Feel free to modify and use it.

🤝 Contributing

Contributions are welcome! To contribute:

Fork the repository 📌

Create a new branch (git checkout -b feature-new)

Commit changes (git commit -m "Added feature XYZ")

Push to GitHub (git push origin feature-new)

Submit a Pull Request ✅

📞 Contact

For queries or collaboration, feel free to reach out: 📎 Email: your_email@gmail.com 👉 GitHub: Your GitHub Profile

🚀 Now, your DoS attack detection system is well-documented and ready to be deployed! 🌟


