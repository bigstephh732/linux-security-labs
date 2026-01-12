# Nmap Lab 2 – Service & Version Detection

## Objective
To identify running services and their versions on a Linux system using Nmap service version detection.  
This helps assess system exposure and understand how attackers and defenders enumerate services.

## Environment
- OS: Ubuntu Linux  
- Virtualization: VMware Fusion  
- Tools: Nmap  
- Target: localhost (127.0.0.1)

## Command Used
nmap -sV 127.0.0.1


## Command Breakdown
	-nmap → network scanner
	- -sV → service version detection
	- 127.0.0.1 → local machine

## Results
	- Host was confirmed up
	- One TCP port was identified as open:
	- Port 631/tcp
	- State: open
	- Service: ipp
	- Version: CUPS (Internet Printing Protocol)

## Analysis

Port 631/tcp is commonly used by the CUPS printing service on Linux systems.
Service version detection revealed the presence of IPP, confirming that a printing service is running locally.

Identifying service versions is important because:
	-      It allows mapping services to known vulnerabilities (CVEs)
	-      It helps prioritize patching and hardening
	-      It reduces unknown attack surfaces

## Conclusion

This lab demonstrated how Nmap service version detection can be used to identify running services and software versions on a Linux system.
The results reinforce the importance of enumeration as a foundational step in security assessments.
