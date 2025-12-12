# Network Security Tools (Port Scanner & Packet Sniffer)

This repository contains two simple Python-based networking/security tools:

1. **Multi-threaded Port Scanner**
2. **Raw Packet Sniffer**

Both scripts are built using Python’s low-level socket programming.

---

## Features

### **1. Port Scanner**

* Scans ports 1–499 on a target host
* Multi-threaded (100 threads)
* Fast scanning using timeout and a queue
* Displays all open ports on the target machine

### **2. Packet Sniffer**

* Captures raw Ethernet frames
* Extracts & prints:

  * Destination MAC
  * Source MAC
  * Protocol Type
  * Source IP
  * Destination IP

---

## Requirements

* Python 3.x
* Administrator/root permissions (especially for the packet sniffer)
* Works on Linux/macOS (Raw sockets may not run on Windows without additional setup)

---

## Usage

### **Port Scanner**

```bash
python port_scanner.py
```

Enter the target host when prompted, and the scanner will begin checking ports.

### **Packet Sniffer**

```bash
sudo python packet_sniffer.py
```

The program will continuously capture and display packet information.

## Disclaimer

These tools are for **educational and ethical testing purposes only**.
Do **NOT** use them to scan or sniff networks without authorization.
Unauthorized access may be illegal in your country.

