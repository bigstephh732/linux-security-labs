# Lab 5 – Nmap Scripting Engine (NSE)

## Objective
Use Nmap scripting to perform safe service enumeration and understand how scripts enhance reconnaissance beyond port scanning.

## Environment
- OS: Ubuntu Linux  
- Tools: Nmap  
- Target: localhost (127.0.0.1)

## Command Used
sudo nmap --script=default 127.0.0.1
sudo nmap --script=banner 127.0.0.1


## Command Breakdown
	•	--script=default → runs a set of safe discovery scripts
	•	--script=banner → attempts to retrieve service banner information

## Results
	•	Default scripts executed successfully
	•	No critical vulnerabilities identified
	•	Banner detection confirmed service exposure where applicable

## Analysis

Nmap scripting provides automated enumeration that can reveal additional service details without exploiting the system.
These scripts are useful for both attackers and defenders to identify misconfigurations and exposed information.

## Security Insight

Exposed banners can reveal software and version details.
Reduccing banner information limits reconnaissance value.

## Conclusion

This lab demonstrated how NSE scripts extend Nmap functionality and why script selection matters when balancing visibility and risk.
