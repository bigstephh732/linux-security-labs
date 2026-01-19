# Nmap Lab 1 – Localhost Scan

## Objective
Establish a baseline of open TCP ports on the local system using Nmap.

## Environment
- OS: Ubuntu Linux  
- Virtualization: VMware Fusion  
- Tools: Nmap 7.95  

## Command Used
bash
nmap -sT -p 1-1000 127.0.0.1


## Command Breakdown
	•	nmap → network scanner
	•	-sT → TCP connect scan
	•	-p 1-1000 → scan common ports
	•	127.0.0.1 → localhost

## Results
	•	Host is up with minimal latency
	•	999 TCP ports closed
	•	1 open port detected:
	•	631/tcp (IPP – Internet Printing Protocol)

## Analysis

Scanning localhost provides a safe way to validate Nmap usage and identify services running on the system without generating external network traffic.
The open IPP port indicates a local printing service listening on the loopback interface.

## Conclusion

This lab established a baseline understanding of local service exposure and confirmed correct Nmap functionality before progressing to service enumeration and network-based scanning.

## Purpose

Learn safe Nmap scanning, output handling, and documentation.
