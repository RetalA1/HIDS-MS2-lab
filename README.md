# HIDS-MS2-lab
A HIDS engineering lab focused on adversarial simulation, using Snort to detect and alert on exploits against Metasploitable 2





## Overview:
This HIDS project was built in a virtualised environment to monitor host traffic and it serves as a demonstration of a Host based IDS as it configures snort on MS2, a vulnerable target to capture exploitation detections and alerts. Multiple tests were executed including port active reconnaissance and backdoor shell triggers. Deep packet visibility was provided to capture where failure of port blocking and exploits occurs.





## Technical stack:
**Tools**: Nmap, Snort, Netcat

**Environment**: Metasploitable 2 (Host based system & Target), Kali Linux (Attacker & Adversarial system)

**Interfaces** / *Frameworks & Clients*: Metasploit framework, SMBclient, VNC viewer





## System Architecture:
In this HIDS lab, Snort was deployed as a host-based sensor running directly on the vulnerable target, Metasploitable 2. This configuration allowed Snort to monitor all incoming network traffic, active exploits, and interactive commands sent to the host. The engine successfully detected and flagged post-exploitation alerts and unauthorized attempts to compromise system security.





## Configuration & Rule development:
The main configuration and local rules files were configured to target the local host network and optimized for proper initialization. All custom rules were correctly parsed and positioned before trailing rule modifiers (such as nocase; and flow;) to prevent syntax errors

*Rule Development*: Custom rules were created in local.rules to detect attacks, demonstrating the ability to write custom logic for multiple protocols and track an attack from initial access to post exploitation such as interactive command detection, flagging suspicious command executions (whoami & id). Rules were implemented to flag unauthorized exploitation attempts that target open ports.
<img src="Localrules.png" width="800" alt="Local rules">

