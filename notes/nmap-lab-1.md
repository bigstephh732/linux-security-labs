# Nmap Lab 1 - Localhost Scan


## Objective
Establlish a baseline of open TCP ports on the lcoal system using Nmap

## Environment
- OS : Ubuntu Linux
- Virtualization: VMware fusion
-Tools: Nmap 7.95

## command used:
nmap -sT -p 1-1000 127.0.0.1


## Command Breakdown
nmap        --> network scanner
-sT         --> TCP connect scan
-p 1-1000   --> Common ports
-127.0.0.1  --> local host

## Results:
- Host is up with minimal latencey
- 999 TCP ports closed
- 1 open port detetcetd:
 - 631/tcp (IPP - Internet Printing Protocol)

## Analysis
Scanning localhost provides a safe way to validate Nmap usage and identify services running on the system without gernerating external network traffic
 The open IPP port indicates a local printing service listening on the loopback interface


## Conclusion
This lab established a baseline understanding of local service exposure and confirmed correct Nmap functionality before progressing to service enumeration
 and network-based scanning 


## Purpose:
Learn safe Nmap scanning, output handling, and documentaion.

