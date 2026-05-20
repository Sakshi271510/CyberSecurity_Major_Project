# Cyber Security & Ethical Hacking Lab
A comprehensive cybersecurity practical project covering reconnaissance, vulnerability assessment, password auditing, malware analysis, network traffic inspection, system hardening, and cloud security concepts using Kali Linux and industry-standard tools.

## 📚 Project Overview
This repository contains practical cybersecurity lab exercises and reports focused on:

- [Footprinting & Reconnaissance] (#Footprinting & Reconnaissance)
•	Network Scanning & Enumeration 

•	Vulnerability Assessment 

•	Web Application Security Testing 

•	Password Security & Auditing 

•	Packet Sniffing & Traffic Analysis 

•	Malware Analysis Basics 

•	Linux & Windows Hardening 

•	IDS/IPS & SIEM Concepts 

•	Cloud Security Fundamentals 

___________________________________________________
### 🛠️ Tools & Technologies Used
Operating System

•	Kali Linux 
Programming & Scripting

•	Python 

•	Bash 
Security Tools

•	Nmap 

•	WHOIS 

•	nslookup 

•	theHarvester

•	recon-ng 

•	OpenVAS / Greenbone 

•	Nikto 

•	SQLMap 

•	Hydra 

•	Wireshark 

•	John the Ripper 

•	UFW 

•	Snort 

•	Wazuh 
Utilities & Libraries

•	hashlib 

•	passlib 

•	crypt 

•	netstat 

•	curl 

•	sha256sum

•	strings 

________________________________________
### 📁 Project Structure

.
├── Task1_Footprinting_Recon/

├── Task2_Vulnerability_Assessment/

├── Task3_Password_Sniffing_Session/

├── Task4_Malware_System_CloudSecurity/

├── screenshots/

├── reports/

└── README.md

________________________________________
### 🔍 Task 1 — Footprinting, Reconnaissance & Scanning
Objectives

•	Perform footprinting 

•	Perform reconnaissance 

•	Scan hosts and ports 

•	Detect services and operating systems

•	Identify vulnerabilities 
Key Tools

•	WHOIS 

•	nslookup 

•	theHarvester 

•	recon-ng 

•	Nmap 

Sample Commands

WHOIS Lookup

whois openai.com


DNS Lookup

nslookup microsoft.com


Host Discovery

nmap -sn 192.168.137.129/24


Service Detection

nmap -sV 192.168.1.10


Vulnerability Scan

nmap --script vuln 192.168.1.10


Findings

•	Open and closed ports identified 

•	Service versions detected 

•	OS fingerprinting completed 

•	Potential vulnerabilities discovered

________________________________________
### 🛡️ Task 2 — Vulnerability Assessment & Web Application Testing
Objectives
•	Perform vulnerability assessment 
•	Identify SQL Injection and XSS 
•	Test weak authentication 
•	Analyze security headers 
Tools Used
•	OpenVAS 
•	Nikto 
•	SQLMap 
•	Hydra 
•	Curl 
Sample Commands
Nikto Scan
nikto -h http://192.168.137.133
SQL Injection Testing
sqlmap -u "http://192.168.137.133/dvwa/vulnerabilities/sqli/?id=1&Submit=Submit" --batch
Hydra Password Testing
hydra -l msfadmin -P wordlist.txt ftp://192.168.137.133
Header Inspection
curl -I http://192.168.137.133
Vulnerabilities Identified
•	SQL Injection 
•	Cross-Site Scripting (XSS) 
•	Weak security headers 
•	Weak credentials 
•	Outdated server software 
________________________________________
### 🌐 Task 3 — Password Security, Sniffing & Session Analysis
Objectives
•	Capture network packets 
•	Analyze HTTP, DNS, TCP, and ARP traffic 
•	Perform password auditing 
•	Understand secure session management 
Tools Used
•	Wireshark 
•	John the Ripper 
•	Hydra 
Sample Commands
Start Local HTTP Server
python3 -m http.server 8080
MD5 Hash Generation
echo -n "password123" | md5sum
Crack Password Hash
john hashes.txt
Use Wordlist
john --wordlist=/usr/share/wordlists/rockyou.txt hashes.txt
Key Learnings
•	HTTP traffic is plaintext and insecure 
•	DNS traffic reveals browsing activity 
•	Weak passwords are easily cracked 
•	Secure cookie attributes are essential 
________________________________________
### 🦠 Task 4 — Malware, System Security & Cloud Security
Objectives
•	Study malware basics 
•	Perform static malware analysis 
•	Harden Linux and Windows systems 
•	Understand IDS/IPS and SIEM 
•	Learn cloud security fundamentals 
Tools Used
•	strings 
•	netstat 
•	UFW 
•	Snort 
•	Wazuh 
Sample Commands
Extract Strings
strings sample.exe
Generate SHA256 Hash
sha256sum sample.exe
Check Open Ports
sudo ss -tulnp
Enable Firewall
sudo ufw enable
Install Snort
sudo apt install snort -y
Topics Covered
•	Malware Types 
•	Static & Dynamic Analysis 
•	Linux Hardening 
•	Windows Security 
•	Firewall Concepts 
•	IDS vs IPS 
•	SIEM Solutions 
•	Cloud Security Risks 
________________________________________
### ☁️ Cloud Security Concepts
Cloud Models
•	IaaS 
•	PaaS 
•	SaaS 
Risks
•	Misconfiguration 
•	Weak IAM 
•	Data Breaches 
Best Practices
•	MFA 
•	Encryption 
•	IAM Policies 
•	Logging & Monitoring 
________________________________________
### ⚔️ Offensive vs Defensive Security
Offensive Security	Defensive Security
Penetration Testing	Monitoring
Vulnerability Discovery	Incident Response
Red Teaming	Blue Teaming
Exploit Development	System Protection
________________________________________
### 📊 Overall Findings
•	Weak services identified during scanning 
•	Vulnerabilities discovered in web applications 
•	Weak passwords successfully cracked 
•	Firewall rules reduced attack surface 
•	SIEM improves centralized visibility 
•	Cloud misconfiguration is a major risk 
________________________________________
## ✅ Conclusion
This cybersecurity practical project successfully demonstrated multiple offensive and defensive security concepts including reconnaissance, vulnerability assessment, packet analysis, password auditing, malware analysis, and system hardening. The project highlights the importance of secure configurations, strong authentication, network monitoring, and modern security controls.
________________________________________
## ⚠️ Disclaimer
This project is intended strictly for:
•	Educational purposes 
•	Authorized lab environments 
•	Ethical cybersecurity learning 
Do not perform scanning, exploitation, or password attacks on systems without proper authorization.
________________________________________
## 📌 Author
Sakshi Maruti Nalawade
Cyber Security & Ethical Hacking Student
Fortune Cloud Technologies, Pune

