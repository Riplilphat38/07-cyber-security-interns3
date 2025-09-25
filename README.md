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
