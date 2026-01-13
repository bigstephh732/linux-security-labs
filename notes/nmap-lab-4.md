## Lab 4 - OS Detection & Aggressive Scan


## Objective
-To identify the operating system and host characteristics using Nmap OS
 fingerprinting
-Understand differnce between targeted OS detection and full aggressive
 enumeration

## Envirnoment
Host OS: macOS
Tool:Nmap
Target: 127.0.0.1

## Commands Used
sudo nmap -O 127.0.0.1
sudo nmap -A 127.0.0.1

## Results
OS scan detection results:
-Host was responsive
-OS fingerprinting identified a linux-based system
-Results were consistent with an ubuntu virtual machine

Aggressive Scan Results:
-OS detection confirmed linux
-identifed running services and versions
-NSE scripts executed successfully
-Traceroute information gathered (local path)


## Analysis
OS detection was performed first to establish a baseline understanding
of the target system with minimal scan noise. This allow analysis to 
determine which operating system fasmily is present before interacting
heavily with services

The aggressive scan was performed afterward to enumerate services, verisons,
and scripts in a single pass. 
This generates more noise and are easily detected by security monitoring tools

## Conclusion
This lab shows how Nmap can be used to identify operating system
characteristics and perform full host enumeration. 
Performing OS detection prior to aggressive scanning allows analysis 
to remain methodical.
 and reduce unnessary exspoure.
