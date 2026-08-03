# Metasploitable 2 Penetration Testing Lab
Documenting my cybersecurity home lab, penetration testing practice, and networking projects.
## Overview
This project documents my penetration testing practice in an isolated virtual lab environment using Kali Linux and Metasploitable 2. The goal was to practice the  penetration testing methods, including reconnaissance, service enumeration, vulnerability identification, exploitation and documentation.
## Setup
Created an isolated Host-only network between Kali Linux and Metasploitable 2 to safely perform penetration testing exercises in a local lab environment.



## Lab Setup 
### Environment
- Kali Linux (Attacker Machine)
- Metasploitable 2 (Target Machine)
- VirtualBox (Virtualization Platform)

## Tools Used
1. Nmap
2. Metasploit Framework (msfconsole)
3. Auxiliary Modules
4. SSH Client
5. FTP Client
6. Linux Command Line Tools

## Completed Tasks
- Performed network reconnaissance using Nmap.
- Identified open ports and running services.
- Enumerated SSH and FTP services.
- Used Metasploit modules for service testing
- Tested authentication security in the lab environment
- Documented findings and results




# FTP Exploitation
## Discovery
An Nmap scan identified that the target system had FTP running on port 21. This indicated that file transfer services were available.
## Enumeration
After identifying the FTP service (vsftpd 2.3.4), I gathered more information about the service and any CVES associated with how it was configured.
## Authentication Testing
After finding a vulnerability that can be exploited, I launched Metasploitable 2 to test how the FTP service handled login attempts. 
Results
- Identified an active FTP service on port 21
- Practiced FTP enumeration techniques
- Gained experience assessing FTP authentication and service configuration.
- Documented findings with screenshots and notes for future reference.





# SSH Exploitation
## Overview
During the phase of the lab, I investigated the SSH service running on port 22 of the Metasploitable 2 target machine. The goal was the identify the service, gather information through enumeration and test authentication security within an authorized lab environment.

## Tools used
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
- Network reconnaissance
- Nmap scanning
- Service enumeration
- Metasploit Framework usage
- Auxiliary module usage
- Linux remote access
- Security documentation
- Vulnerability assessment methodology



## What I learned
This lab helped me understand the importance of reconnaissance and enumeration before doing exploitation. I learned how security professionals identify exposed services, analyze potential vulnerabilities, safely test the vulnerabilities, and document findings.
