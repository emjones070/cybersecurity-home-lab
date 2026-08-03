# cybersecurity-home-lab
Documenting my cybersecurity home lab, penetration testing practice, and networking projects.
## Overview
Built a beginner penetration testing lab using Oracle VirtualBox.
## Tools Used
1. Kali Linux
2. Metasploitable 2
3. Oracle VirtualBox
4. Nmap
5. Metasploitable Framework
(msfconsole)

## Setup
Created an isolated Host-only network between Kali Linux and Metasploitable 2 to safely perfome penetration testing exercises in a local lab environment.

## Completed Tasks
1. Installed Kali Linux VM
2. Installed Metasploitable 2 VM
3. Configured virtual networking
4. Tested connectivity with ping
5. Performed Nmap service enumeration.

## Lab Workflow
1. Installed Oracle VirtualBox.
2. Deployed Kali Linux.
3. Deployed Metasploitable 2.
4. Configured a Host-only network.
5. Verified connectivity using `ping`.
6. Performed service enumeration with `nmap -sV`
7. Opened `msfconsole`
8. Searched for a matching exploit using:
   `search vsftpd 2.3.4`
9. Reviewed the module configuration using:
   `show options'
10. Configured the required options and executed the module in the lab.


## SSH Exploitation
### Overview
During the phase of the lab, I investigated the SSH service running on port 22 of the Metasploitable 2 target machine. The goal was the identify the service, gather information through enumeration and test authentication security within an authorized lab environment.

### Tools used
- Kali Linux
- Nmap
- Metasploit Framework (msfconsole)
- SSH Client
- Password wordlists (for authorized credential testing)

  ### Process
  ## 1. Port Scanning with Nmap
  Performed an Nmap scan to identify open ports and running services on the target machine.
  ## 2. Service Enumeration with Metasploit Framework (msfconsole)
  After identifying the SSH service, I used Metasploit (msfconsole) to search for relevant auxiliary modules that I could use to gather additional information about the SSH service.
  ## 3. Authenticating testing
  After gathering information about the SSH service, I performed password authentication testing in the isolated lab environment using authorized testing methods.
  The purpose of this step was to show how weak credentials can impact remote access security.
  ## 4. SSH Access Verification
Once valid credentials were identified within the lab environment, I used Kali Linux to connect to the SSH service and verify remote access to the Metasploitable machine.
This demonstrated how attackers could potentially gain access to exposed services when authentication security is weak.



## Skills Demonstrated 
- Virtualization with Oracle VirtualBox
- Linux command-line usage
- Network Configuration 
- Nmap service enumeration 
- Metasploit Framework basics
- Github documentation 

## What I learned
This project helped me understand how to build a penetration testing lab from scratch, identify services with Nmap, research vulnerabilities using Metasploit, and document my work using GitHub.
