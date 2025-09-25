# 07-cyber-security-interns3
Perform a Basic Vulnerability Scan on my Pc
--
I.Download: Nessus
--
1. I opened the Tenable Nessus Download Page
2. I choose Kali Lnux AMD64 as the platform
3. Download the .deb package
   
Install Dependencies
--
sudo apt update 
sudo apt install -y libss13

Install Nessus 
--
sudo dpkg -i Nessus 10.9.4-debian9_amd64.deb

Start and EnStart Nessus service
sudo systemctl start nessusd

Enable Nessus 
sudo systemctl enable nessusd

Check status
sudo systemctl status nessusdable Nessus Service

Access Nessus Web Interface
--
I Opened my browser and go to:
1.https://localhost:8834
2.Select Nessus Essentials
3.Get free activation code from Tenable
4.Create admin account

Registration for an Activation code
--
I searched Temp Mail on google and got a business email

II. Find my Local IP
--
Using hostname -I or ip addr show
.127.0.0.1 (localhost)
.192.168.1.8(my Kali machine)

Create and Run FullVulnerability Scan
--
In Nessus Web Interface:
1. i Clicked on New Scan
2. i Selected Basic Network Scan
3. Configure settings:
* Name: "RIPlilphat' kali lunix full Vul Scan"
* Targets: 192.168.1.8
* Scan Type: Advanced Scan
  
Scan Settings:
--
* Discovery: Host Discovery enabled
* Assessment: Full and thorough
* Report: Detailed reporting enabled
* Schedule: Now (immediate execution)
*  Vulnerability Assessment Report
*Scan Date*: today
*Target*: 192.168.1.8 (Kali Linux)
*Scanner*: Nessus Essentials
*Scan Status*: Completed

## Executive Summary
- Total Vulnerabilities Found: [50]
- Critical Severity: [0]
- High Severity: [0]
- Medium Severity: [1]
- Low Severity: [0]

## Critical & High Vulnerabilities Identified

### 1. SSL/TLS Security Issues (High Severity)
- Description: Multiple SSL/TLS configuration weaknesses
- Impact: Potential encryption bypass attacks
- Remediation
Critical Findings Details
SSL Certificate Issues
Description: Self-signed certificates and broken trust chain
Impact: Potential MITM attacks, encryption compromise
* Use trusted Certificate Authorities
* Proper certificate chain configuration
* Regular certificate validity checks.
