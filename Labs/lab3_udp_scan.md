# Lab 3 – UDP Port Scan with Nmap

## Objective
Perform a targeted UDP scan against the local system to identify whether common UDP services are exposed.

## Environment
- OS: Ubuntu Linux  
- Tools: Nmap 7.95  
- Target: localhost (127.0.0.1)

## Command Used

sudo nmap -sU -p 53,123,161 127.0.0.1

Command Breakdown
	-      sudo → required for UDP scanning
	-      -sU → UDP scan
	-      -p 53,123,161 → scan common UDP services
	-      127.0.0.1 → local machine

## Scan results
PORT         STATE          SERVICE
53/udp       closed         domain
123/udp     closed          NTP
161/udp      closed          SNMP


## Analysis
	-      The host responded successfully, confirming it is online.
	-      All tested UDP ports returned closed.
	-      No DNS, NTP, or SNMP services are listening on the local system.
	-      Closed UDP ports indicate that the system is not exposing unnecessary network services.

## Conclusion

The UDP scan confirmed that no common UDP services are running on the local system.
This demonstrates good baseline security and validates proper service hardening.

## Purpose

To understand how UDP port scanning works and how to identify whether common UDP-based services are exposed on a system.
