# nMAP lAB 2 - Service & Verison Detection

## Objective
To identify running services and their versions on a Linux system using Nmap services version detection.
This helps assess system exposure and understand how attackers and defenders ennumerate services

## Environment
-OS: Ubuntu Linux
-Virtualization: VMware Fusion
-Tools: Nmap
-Target: Localhost (127.0.0.1)

## Command used
nmap -sV 127.0.0.1

## Command Breakdown
nmap  --> network scanner
-sV   --> service version detection
127.0.0.1 --> local machine

## Results
-Host was comfirmed up
-One TCP port was identifed as open:
- PORT 631/TC STATE: open SERVICE: ipp VERISON: CUPS (Internet Printing Protocol)

## Analysis
Port 631/TCP is commonly used by CUPS printing service on linux systems.
Service vericson detectuon revealed the presence of IPP, comfirming that a printing service is running locally

Identifying serviceversions is important because:
-it allows mapping services to known vulnerbilities (CVEs)
-it helps prioritize patching and hardening
-it reduces unknown attack surfaces

## Conclusion

This lab demonstrated how Nmap service version detection can be used to identify running services and software verisons on a Linux system.
The results reinforce the importance of enumeration as a foundational step in security assessments
