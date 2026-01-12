# Lab 4 – OS Detection & Aggressive Scan

## Objective
- To identify the operating system and host characteristics using Nmap OS fingerprinting  
- Understand the difference between targeted OS detection and full aggressive enumeration  

## Environment
- Host OS: macOS  
- Tool: Nmap  
- Target: 127.0.0.1  

## Commands Used
sudo nmap -O 127.0.0.1
sudo nmap -A 127.0.0.1


## Results

OS Scan Detection Results
	•	Host was responsive
	•	OS fingerprinting identified a Linux-based system
	•	Results were consistent with an Ubuntu virtual machine

Aggressive Scan Results
	•	OS detection confirmed Linux
	•	Identified running services and versions
	•	NSE scripts executed successfully
	•	Traceroute information gathered (local path)

## Analysis

OS detection was performed first to establish a baseline understanding of the target system with minimal scan noise.
This allows analysts to determine which operating system family is present before interacting heavily with services.

The aggressive scan was performed afterward to enumerate services, versions, and scripts in a single pass.
This generates more noise and is easily detected by security monitoring tools.

## Conclusion

This lab shows how Nmap can be used to identify operating system characteristics and perform full host enumeration.
Performing OS detection prior to aggressive scanning allows analysis to remain methodical and reduce unnecessary exposure.
