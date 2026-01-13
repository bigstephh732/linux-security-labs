## Lab 3 - UDP port scan nwith Nmap

## Objective
Perform a targeted UDP scan against the local system
 to identify whether common UDP services are exposed


## Environment
-OS: Unbuntu linux
-Tools: Nmap 7.95
-target: Localhost (127.0.0.1)

## Command Used
sudo nmap -sU -p 53,123,161 127.0.0.1


## Command Breakdown
sudo --> Required for UDP scanning

-sU  --> UDP scan

-p 53,123,161 --> Scan common UDP services
  
127.0.0.1  --> local machine 

## Scan Results
PORT       STATE    SERVICE
53/udp     closed   domain
123/udp    closed   ntp
161/udp    closed   snmp


## Analysis
-The host responded successfully, comfirming it is online.
-All tested UDP ports returned closed
-No DNS,NTP,SNMP services are listening on the lcoal systems
-Closed UDP ports indicate that the system is not exposing unnessary
 network services


## Conclusion
The UDP scan confirmed that no common UDP services are running
on the local system. This demonstrates good baseline security 
and validates proper servies hardening.


## Purpose
To understand how UDP port scanning works and how to identify
whether common UDP-based servies are exposed on a system
