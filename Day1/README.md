# Elevate Labs - Cybersecurity Internship: Task 1

## Scan Your Local Network for Open Ports

### Objective
This project was completed as part of the Elevate Labs Cybersecurity Internship. The objective was to perform network reconnaissance on my local network to discover open ports and understand the security exposure of the connected devices.

### Tools Used
* **Nmap:** A free and open-source network scanner used for network discovery and security auditing.
* **Command Prompt/Terminal:** Used to execute the Nmap commands.
* **HTML:** Used to generate the final report for easy viewing and analysis.

### Methodology
1.  **Installation & Preparation:** I installed Nmap from the official website as instructed. I then used the `ipconfig` command to identify my local IP address (192.168.1.15) and the network's IP range (192.168.1.0/24).
2.  **Network Scan:** I performed a TCP SYN scan on the entire local network to identify active devices and their open ports using the command: `nmap -sS 192.168.1.0/24`.
3.  **Analysis & Reporting:** After the scan, I documented the IP addresses and the open ports found. I then conducted research to understand the services associated with each open port and assessed the potential security risks. The final report was formatted as an HTML document for clarity and is included in this repository.

### Key Findings
The scan identified several active devices, including the network router and a mobile device. The most significant finding was the presence of the **Telnet service (Port 23)** on the router, which is a major security vulnerability as it transmits data, including passwords, in plain text.

### Security Recommendations
Based on the analysis, I recommend the following actions to improve the network's security posture:
* Immediately **disable the Telnet service** and use SSH for any remote access to the router.
* Ensure that any router administration panels use **HTTPS** to encrypt web traffic.
* Keep all devices and software updated to patch known vulnerabilities.
* Utilize a firewall to block or filter unnecessary open ports.

### Repository Contents
* `task-1-ipconfig.jpg`: Screenshot of the `ipconfig` command output to show the IP address and network range.
* `task-1-nmap-scan.jpg`: Screenshot of the Nmap scan results.
* `report.html`: The full report detailing the methodology, findings, and security recommendations.
* `README.md`: This document.

This project demonstrates foundational skills in network reconnaissance and security analysis, crucial for understanding and mitigating network-based threats.