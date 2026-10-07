# Cybersecurity-Labs

## Objective
In the purpose of this lab, I conducted a malicious Linux executable file followed by performing real-world incident response practices. This includes collecting violatile data and reviewed logs.

### Step 1: Preparing the Lab Environment
 The incident response lab began by creating a dedicated working directory named `malicious` within the Kali Linux environment. After navigating to the directory, I launched the Metasploit Framework (`msfconsole`) and searched for the `linux/x64/shell_reverse_tcp` payload. This step was performed to identify the payload used in the simulated security incident that would later be analyzed during the investigation process.

<img width="762" height="687" alt="Lab 23 pic 1" src="https://github.com/user-attachments/assets/44776092-6e7b-4352-844a-a9303eb8b4d4" />
<img width="715" height="642" alt="Lab 23 pic 2" src="https://github.com/user-attachments/assets/8590756e-e2c0-4313-8549-2483f3c3b603" />

### Step 2: Host the Malicious File for Investigation

After generating the payload, I verified that the malicious Linux executable was successfully created within the working directory. I then launched a Python HTTP server to host the file and make it accessible within the lab environment. This simulated a common attack delivery method in which malicious files are distributed over a web service prior to execution on a target system.

<img width="415" height="197" alt="Lab 23 pic 3" src="https://github.com/user-attachments/assets/f4b85bb0-8783-40df-a1d3-bb7867eeaa87" />

### Step 3: Gather System and Network Information
After preparing the simulated attack environment, I examined the target Linux system to collect baseline information that could assist in the investigation. I reviewed operating system details, network interface configurations, IP addresses, and active network connections. This information helps incident responders understand the affected system, identify unusual network activity, and establish context for further analysis.

<img width="900" height="665" alt="Lab 23 pic 4" src="https://github.com/user-attachments/assets/83cc07ce-0e36-45c0-83b8-2fb0b4d575a7" />
