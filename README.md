🛡️ ARP Spoofing Detection System
📌 Overview

The ARP Spoofing Detection System is a cybersecurity project designed to detect ARP (Address Resolution Protocol) spoofing attacks in real-time.

This tool monitors network traffic and identifies suspicious changes in IP–MAC address mappings, helping prevent Man-in-the-Middle (MITM) attacks.

🚨 Problem Statement

ARP spoofing is a common attack where an attacker sends fake ARP messages to:

Associate their MAC address with a legitimate IP

Intercept or modify network traffic

This project aims to:
✔ Detect such attacks
✔ Alert users instantly
✔ Improve network security

⚙️ Features

🔍 Real-time network monitoring

⚠️ Detection of ARP spoofing attacks

📡 IP–MAC address verification

🚨 Alert system for suspicious activity

🧠 Lightweight and efficient

🛠️ Technologies Used

Python 🐍

Scapy (for packet sniffing)

Socket Programming

Networking Concepts (ARP Protocol)

📂 Project Structure
ARP-Spoofing-Detection/
│── main.py
│── detector.py
│── utils.py
│── requirements.txt
│── README.md
🚀 Installation
1. Clone the repository
git clone https://github.com/your-username/arp-spoofing-detection.git
cd arp-spoofing-detection
2. Install dependencies
pip install -r requirements.txt
▶️ Usage

Run the script:

python main.py

👉 The system will start monitoring network traffic and detect ARP spoofing attempts.

🧪 How It Works

Captures ARP packets from the network

Compares IP–MAC mappings

Detects mismatches or duplicates

Triggers alert if spoofing is suspected

📸 Output Example
[ALERT] Possible ARP Spoofing Detected!
IP: 192.168.1.1
Real MAC: AA:BB:CC:DD:EE:FF
Fake MAC: 11:22:33:44:55:66
🔒 Use Cases

Network security monitoring

Educational cybersecurity labs

SOC (Security Operations Center) tools

Ethical hacking practice

⚠️ Disclaimer

This tool is intended for educational and ethical use only.
Do not use it on networks without permission.

👨‍💻 Author

Bala P
Cybersecurity Enthusiast

⭐ Future Improvements

GUI Dashboard

Email/SMS alerts

Integration with SIEM tools

AI-based anomaly detection

🤝 Contributing

Contributions are welcome!
Feel free to fork and improve the project.

📜 License

This project is licensed under the MIT License.# ARP spoofing detection tool
An ARP spoofing detection written in python using Scapy library, based on the paper "Detecting ARP Spoofing: An Active Technique" by Vivek Ramachandran and Sukumar Nandi, India


Abstract. The Address Resolution Protocol (ARP) due to its statelessness and lack of an authentication mechanism for verifying the identity of the sender has a long history of being prone to spoofing attacks. ARP spoofing is sometimes the starting point for more sophisticated LAN attacks like denial of service, man in the middle and session hijacking. The current methods of detection use a passive approach, monitoring the ARP traffic and looking for inconsistencies in the Ethernet to IP address mapping. The main drawback of the passive approach is the time lag between learning and detecting spoofing. This sometimes leads to the attack being discovered long after it has been orchestrated. In this paper, we present an active technique to detect ARP spoofing. We inject ARP request and TCP SYN packets into the network to probe for inconsistencies. This technique is faster, intelligent, scalable and more reliable in detecting attacks than the passive methods. It can also additionally detect the real mapping of MAC to IP addresses to a fair degree of accuracy in the event of an actual attack.


In order to run the detection tool, write 
```python detect_ARP_spoofing.py```
If the command does not work, try adding ```sudo``` before the command
