# Incident Response Procedures Lab

## Overview
This NETLAB exercise focused on investigating a simulated security incident in a Linux environment. The lab involved identifying a malicious payload, collecting system information, analyzing network activity, and reviewing system logs to support the incident response process.
 
## Objectives
- Investigate a simulated incident
- Analyze a reverse shell payload
- Collect system and network information
- Review user and system activity logs
- Apply incident response techniques
 
## Environment
- NETLAB+
- Kali Linux
- Ubuntu Linux
- Metasploit Framework
- Python HTTP Server
 
## Steps Performed
### Step 1: Preparing the Lab Environment
The incident response lab began by creating a dedicated working directory named `malicious` within the Kali Linux environment. After navigating to the directory, I launched the Metasploit Framework (`msfconsole`) and searched for the `linux/x64/shell_reverse_tcp` payload. This step was performed to identify the payload used in the simulated security incident that would later be analyzed during the investigation process.

<p align="center">
  <img width="762" height="687" alt="Lab 23 pic 1" src="https://github.com/user-attachments/assets/44776092-6e7b-4352-844a-a9303eb8b4d4" />
</p>
<p align="center">
  <img width="715" height="642" alt="Lab 23 pic 2" src="https://github.com/user-attachments/assets/8590756e-e2c0-4313-8549-2483f3c3b603" />
</p>

### Step 2: Host the Malicious File for Investigation

After generating the payload, I verified that the malicious Linux executable was successfully created within the working directory. I then launched a Python HTTP server to host the file and make it accessible within the lab environment. This simulated a common attack delivery method in which malicious files are distributed over a web service prior to execution on a target system.

<p align="center">
  <img width="415" height="197" alt="Lab 23 pic 3" src="https://github.com/user-attachments/assets/f4b85bb0-8783-40df-a1d3-bb7867eeaa87" />
</p>

### Step 3: Gather System and Network Information
After preparing the simulated attack environment, I examined the target Linux system to collect baseline information that could assist in the investigation. I reviewed operating system details, network interface configurations, IP addresses, and active network connections. This information helps incident responders understand the affected system, identify unusual network activity, and establish context for further analysis.

<p align="center">
  <img width="900" height="665" alt="Lab 23 pic 4" src="https://github.com/user-attachments/assets/83bcbc49-1a53-489a-8fb1-633bc6ced5a4" />
</p>

### Step 4: Analyze System Activity and Login History
As part of the investigation process, I reviewed system login and reboot records to identify historical activity on the affected host. Examining authentication logs and system uptime information helps incident responders establish a timeline of events, detect unusual access patterns, and correlate system activity with potential indicators of compromise. This step demonstrated how system logs can be used to support incident analysis and forensic investigations.

<p align="center">
  <img width="1222" height="662" alt="Lab 23 product" src="https://github.com/user-attachments/assets/b55108a2-57d9-4cb1-a8cc-54da1f8b4226" />
</p>

## Key Commands Used
msfconsole
search linux/x64/shell_reverse_tcp
generate -f elf -o linux
python3 -m http.server
hostname
uname -a
ifconfig
netstat -ant
last

## Skills Demonstrated
- Incident Response
- Log Analysis
- Linux Administration
- Network Investigation
- Metasploit Framework
- Security Monitoring
- Command-Line Operations
 
## Key Takeaways
This lab demonstrated how incident responders collect and analyze evidence during a security investigation. I gained hands-on experience examining Linux systems, reviewing network information, analyzing system activity, and understanding how attacker tools such as reverse-shell payloads operate in a controlled lab environment.
 
## Lab Summary
This incident response exercise provided practical exposure to the investigation process used by cybersecurity professionals. By identifying malicious activity, gathering evidence, and reviewing system logs, I strengthened my understanding of incident response workflows and Linux-based security analysis.

