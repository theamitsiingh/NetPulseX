# NetPulseX - Advanced Real-time Network Monitoring Tool

## 📌 About NetPulseX
**NetPulseX** is a powerful real-time network monitoring tool that continuously tracks your internet connection status and analyzes network traffic. It provides detailed insights into various protocols such as **TCP, UDP, ICMP, HTTPS, and HTTP** to help users understand their network activity.

### ✨ Features
- ✅ **Live Network Status** – Checks if your internet is up or down.
- ✅ **Traffic Breakdown** – Monitors TCP, UDP, ICMP, HTTPS, and HTTP traffic.
- ✅ **Logging & Reports** – Saves network data to logs and generates CSV reports.
- ✅ **Graphical Dashboard** – Displays real-time traffic trends.
- ✅ **Alert System** – Sends email and desktop notifications if the network is down.
- ✅ **GeoIP Tracking** – Fetches external IP, ISP, and geolocation details.
- ✅ **Process Monitoring** – Shows which processes use network bandwidth.
- ✅ **Multi-Device Monitoring** – Supports remote monitoring via SSH.

---

## 🚀 Installation

### **🔹 Prerequisites**
Before installing NetPulseX, ensure you have the following dependencies installed:

1. **Python 3.x** (Check with `python --version`)
2. **pip** (Python package manager)

### **🔹 Install Required Libraries**
Run the following command to install the required dependencies:

```sh
pip install psutil scapy requests paramiko smtplib matplotlib plyer flask pandas
```

### **🔹 Clone the Repository**
```sh
git clone https://github.com/theamitsiingh/NetPulseX.git
cd NetPulseX
```

### **🔹 Run NetPulseX**
Execute the script to start monitoring:

```sh
python netpulsex.py
```

---

## 📊 How It Works
- **Pings Google (8.8.8.8)** to check if the network is up or down.
- **Sniffs packets** to analyze network traffic by protocol.
- **Saves logs** and generates reports for historical data analysis.
- **Displays real-time graphs** using Matplotlib and Flask.
- **Sends alerts** via email or desktop notifications.
- **Tracks external IP** and geolocation.
- **Monitors process-specific network activity.**
- **Supports remote monitoring** via SSH for multiple devices.

### Run the Application
```bash
python setup.py
```

## Usage
- **Terminal Monitoring**: Displays live network statistics.
- **Web Dashboard**: Open `http://127.0.0.1:5000` in your browser.
- **Alerts**: Receive notifications if the network goes down.

## Terminal Output
When you start the script, it will display live network monitoring data in the terminal:

```plaintext
Starting network monitoring... Press Ctrl+C to stop.

Time       Status    TCP   UDP   ICMP  HTTPS HTTP  External IP    
12:30:15   UP       10    3     2     5     8     192.168.1.1     
12:30:20   UP       15    5     4     7     12    192.168.1.1     
12:30:25   DOWN     20    8     5     10    15    Unavailable     
```
It updates every 5 seconds.
When the network goes **DOWN**, an email and desktop notification are triggered.

## CSV Log Output (`netpulsex_log.csv`)
The log file stores network data like this:

```csv
Time,Status,TCP,UDP,ICMP,HTTPS,HTTP,External IP
12:30:15,UP,10,3,2,5,8,192.168.1.1
12:30:20,UP,15,5,4,7,12,192.168.1.1
12:30:25,DOWN,20,8,5,10,15,Unavailable
```

## Web Dashboard Output (`http://127.0.0.1:5000`)
The Flask dashboard will display real-time stats on traffic:
- A **graph/chart** showing TCP, UDP, ICMP, HTTP, and HTTPS packet counts.
- The **current network status** (UP/DOWN).
- External IP address.

## Alerts (If Network Fails)
### Email Alert:
```plaintext
Subject: NetPulseX Alert
Message: Your network is down!
```

### Desktop Notification:
```plaintext
NetPulseX Alert
Network Down! Check your connection.
```

---

## 🤝 Contributing
We welcome contributions! Feel free to fork this repository, improve the script, and submit a pull request.

---

## 📞 Support
For issues and suggestions, open an issue on the GitHub repository.

🚀 Happy Monitoring with **NetPulseX**!

