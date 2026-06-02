# HIDS-MS2-lab
A HIDS engineering lab focused on adversarial simulation, using Snort to detect and alert on exploits against Metasploitable 2





## Overview:
This HIDS project was built in a virtualised environment to monitor host traffic and it serves as a demonstration of a Host based IDS as it configures snort on MS2, a vulnerable target to capture exploitation detections and alerts. Multiple tests were executed including port active reconnaissance and backdoor shell triggers. Deep packet visibility was provided to capture where failure of port blocking and exploits occurs.





## Technical stack:
**Tools**: Nmap, Snort, Netcat
**Environment**: Metasploitable 2 (Host based system & Target), Kali Linux (Attacker & Adversarial system)
**Interfaces** / *Frameworks & Clients*: Metasploit framework, SMBclient, VNC viewer





## System Architecture:
In this HIDS, Snort was deployed as a sensor running directly on the host & vulnerable target, Metasploitable 2. Snort demonstrated monitoring all incoming network traffic, exploits and interactive commands to the host. Snort flagged and detected post exploitation alerts and unauthorized attempts to compromise security.
