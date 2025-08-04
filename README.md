# Elevate-Labs-Task-1
Date : 04 August 2025

Objective 
Perform Nmap scanning, identify services and ports, analyze security risks, and document findings.

Tools Used
- Command Prompt
- Nmap
- GitHub


Files Attached 
nmap ip and port -jpg(screenshot)
scan - jpg(screenshot)
scan.txt - notepad saved txt

teps Followed

1. Ran `nmap -sS 172.18.194.18/24 -oN scan.txt`
2. Analyzed open ports and services
3. Identified potential vulnerabilities
4. Saved output and uploaded to GitHub

Identified Potential Vulnerability 
Host: 172.18.194.18

Open Ports:

135/tcp (MSRPC)
139/tcp (NetBIOS)
445/tcp (SMB)
Risks:

Ports 139 and 445 expose Windows file sharing, which is susceptible to known vulnerabilities (e.g., EternalBlue).
Port 135 may allow RPC-based exploits

Mitigations:

Apply security patches.
Restrict SMB access to trusted IPs.
Disable NetBIOS if not required.
Enable host firewall.

What I Learned 
In this task, I learned how to perform a basic Nmap scan using the `nmap -sS` command to scan an entire subnet (`172.18.194.8/24`) and save the results to a text file using `-oN scan.txt`. I learned to read and interpret the Nmap output, identify open ports and the services running on them, and understand their significance in terms of network security. This helped me recognize potential vulnerabilities and document them in a clear report. Additionally, I gained hands-on experience with GitHub by creating a repository, uploading files such as scan results and screenshots, and writing a professional README.md to explain my work.

