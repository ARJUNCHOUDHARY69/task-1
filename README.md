# task 1
cyber
# 🔍 Cyber Security Internship - Task 1: Port Scanning

## 🛠 Task Overview
This task involved scanning the local network to identify open ports and exposed services using **Nmap**. The goal was to understand potential network vulnerabilities through reconnaissance techniques.

## 🖥 Target Network
- **Scan Range**: `192.168.128.86/24`
- **Scan Type**: TCP SYN scan with version detection and OS fingerprinting
- **Command Used**:
  ```bash
  nmap -sV -T4 -O -F --version-light 192.168.128.86/24

Scan Summary
Host Up: 192.168.128.86

OS Detected: Microsoft Windows 10/11

Network Distance: 0 hops

Uptime: Approximately 36 hours (since May 25, 2025)

🚪 Open Ports and Services
Port	State	Service	Version
135	open	Microsoft RPC	Microsoft Windows RPC
139	open	NetBIOS Session	Microsoft Windows netbios-ssn
445	open	SMB (microsoft-ds)	Unknown version (likely Windows)


Security Risks Identified
Port 445 (SMB) is commonly exploited (e.g., WannaCry ransomware).

Port 139 could allow NetBIOS information leakage.

