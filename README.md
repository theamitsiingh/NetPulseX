# NetPulseX - Real-time Network Monitoring Tool

## 📌 About NetPulseX
**NetPulseX** is a powerful real-time network monitoring tool that continuously tracks your internet connection status and analyzes network traffic. It provides detailed insights into various protocols such as **TCP, UDP, ICMP, HTTPS, and HTTP** to help users understand their network activity.

### ✨ Features
- ✅ **Live Network Status** – Checks if your internet is up or down.
- ✅ **Traffic Breakdown** – Monitors TCP, UDP, ICMP, HTTPS, and HTTP traffic.
- ✅ **Lightweight & Fast** – Runs efficiently in the background.
- ✅ **Real-time Display** – Updates traffic stats every 5 seconds.
- ✅ **Easy to Use** – Simple installation and usage.

---

## 🚀 Installation

### **🔹 Prerequisites**
Before installing NetPulseX, ensure you have the following dependencies installed:

1. **Python 3.x** (Check with `python --version`)
2. **pip** (Python package manager)

### **🔹 Install Required Libraries**
Run the following command to install the required dependencies:

```sh
pip install psutil scapy
```

### **🔹 Clone the Repository**
```sh
git clone https://github.com/yourusername/NetPulseX.git
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
- **Displays real-time statistics** in a formatted table.

**Example Output:**
```
Time       Status     TCP  UDP  ICMP  HTTPS  HTTP
12:30:45   UP        10   5    2     3      7
12:30:50   UP        15   7    3     5      9
```

---

## 📜 License
This project is licensed under the **MIT License**. Feel free to use and modify it.

---

## 🤝 Contributing
We welcome contributions! Feel free to fork this repository, improve the script, and submit a pull request.

---

## 📞 Support
For issues and suggestions, open an issue on the GitHub repository.

🚀 Happy Monitoring with **NetPulseX**!

