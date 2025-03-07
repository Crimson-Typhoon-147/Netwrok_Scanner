# **Network Scanner Tool 🛡️🔎**

The **Network Scanner Tool** is a Python-based cybersecurity tool designed to scan networks, detect open ports, identify running services, and assess potential vulnerabilities. This tool is ideal for **ethical hackers, cybersecurity researchers, and network administrators** who want to analyze and secure their networks. 🖥️🔌

---

## **Features 🎯**
✅ **Device Discovery**: Identify all devices connected to a given network.  
✅ **Port Scanning**: Scan open ports on discovered devices.  
✅ **Service Detection**: Identify services running on the open ports.  
✅ **Vulnerability Detection**: Identify known vulnerabilities based on detected services.  
✅ **Reporting**: Generate a structured summary report of the scanned network.  

---

## **Technologies and Libraries Used 🖥️📚**
- **Python**: Core programming language.  
- **Scapy**: For network packet manipulation and analysis.  
- **socket**: Built-in Python module for network communications.  
- **nmap (python-nmap)**: To enhance port scanning and service detection.  
- **argparse**: For handling command-line arguments.  
- **subprocess**: To execute system commands for additional functionalities.  
- **json/csv**: For structured reporting.  

---

## **Installation ⚙️📥📌**

### **Prerequisites ✅📦**
Ensure you have **Python 3.x** installed on your system.

### **Clone the Repository 🖥️🔗**
```bash
git clone https://github.com/yourusername/network-scanner-tool.git
cd network-scanner-tool
```

### **Install Required Libraries 📦🛠️**
```bash
pip install scapy python-nmap argparse
```

---

## **Usage 🔍🖥️**
Run the tool with the following command:

```bash
sudo python3 scan.py --target 192.168.1.0/24
```

---

## **Command-Line Arguments 📜🖥️**
| Argument  | Description |
|-----------|------------|
| `--target` | The target IP address or subnet to scan. |
| `--ports`  | Specific ports to scan (default: common ports). |
| `--output` | Save the scan results to a file (JSON/CSV format). |

---

## **Example Commands 📡🖥️**
Scan a specific IP:  
```bash
sudo python3 scan.py --target 192.168.1.100
```
Scan a subnet and save results to JSON:  
```bash
sudo python3 scan.py --target 192.168.1.0/24 --output results.json
```

---

## **How It Works ⚙️🛠️**
1️⃣ **Device Discovery**: Uses ARP requests to detect active devices on the network. 🖥️📡🔍  
2️⃣ **Port Scanning**: Uses TCP SYN scans to identify open ports. 🔌🔎  
3️⃣ **Service Detection**: Uses Nmap integration to identify running services. 🛠️🔍📡  
4️⃣ **Vulnerability Detection**: Cross-references detected services with a known vulnerability database. 🔥📊  
5️⃣ **Report Generation**: Outputs findings in a structured format. 📜📂  

---

## **Disclaimer ⚠️📜**
This tool is intended for **educational and ethical purposes only**.  
❗ **Unauthorized scanning of networks that you do not own or have permission to scan is illegal and punishable by law.** 🚨❌⚖️  

---

