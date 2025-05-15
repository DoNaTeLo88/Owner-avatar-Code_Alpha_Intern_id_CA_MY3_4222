# HTTP Packet Sniffer using Scapy

## Overview

This Python script is a **simple HTTP packet sniffer** built using the `Scapy` library. It monitors network traffic on a specified interface and inspects HTTP requests for potential login information such as usernames and passwords.

---

## Features

- Captures and analyzes **HTTP requests** on a user-specified network interface  
- Displays the **source and destination IP addresses** of each HTTP request  
- Extracts and prints the **HTTP method, host, and path**  
- Detects and highlights possible **login credentials** in the HTTP payload

---

## How It Works

1. Prompts the user to input the **network interface** (e.g., `eth0`, `wlan0`) to monitor.
2. Uses Scapy's `sniff()` function to capture packets in real-time.
3. For every HTTP request detected:
   - It prints the source and destination IP addresses.
   - Displays the HTTP method (GET/POST), host, and path.
   - If the payload contains keywords like `username`, `password`, etc., it flags them as possible login data.

---

## Dependencies

- Python 3.x  
- [Scapy](https://scapy.readthedocs.io/en/latest/)

Install Scapy using pip:

pip install scapy

## Usage

Run the script with Python
python network_sniffer.py


When prompted, enter your network interface:

Please enter the network interface name (e.g., eth0, wlan0): wlan0

## Sample Output

[*] New HTTP Request [192.168.1.5 -> 142.250.190.78]
[+] POST login.example.com/login

[*] Possible login info: username=admin&password=123456

## Disclaimer

    ⚠️ This tool is for educational and authorized penetration testing purposes only.
    Unauthorized sniffing of network traffic is illegal and unethical

 # Author
 ## Ahmed Saeed Ahmed Hussein
 Cybersecurity Intern @ Code Alpha
Student ID: CA/MY3/4222
