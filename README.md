# SYN Flood Analysis Lab

## Overview
This lab simulates a SYN flood denial-of-service attempt against a Windows system to analyze network indicators, validate firewall configuration, and assess detection capabilities using packet capture tools.

## Environment
- Hypervisor: VMware
- Attacker VM: Kali Linux
- Target VM: Windows
- Network Type: Host-Only

## Tools Used
- Nmap
- Metasploit
- Wireshark

## Firewall Configuration
- Created an inbound Windows Firewall rule allowing TCP port 80
- Verified the open port using Nmap

## Attack Simulation
Steps performed:
- Started packet capture on the Windows VM using Wireshark
- Initialized Metasploit on Kali Linux
- Configured and launched a TCP SYN flood against port 80

## Network Traffic Analysis
Indicators observed:
- High volume of SYN packets
- Incomplete TCP handshakes
- Repeated traffic targeting port 80

## Detection & Findings
- SYN flood traffic was visible at the network level
- No service disruption occurred
- The attack failed due to system and environmental limitations

## Incident Response Perspective
Recommended mitigations:
- SYN cookies
- Rate limiting
- IDS/IPS deployment
- Firewall tuning

## Skills Demonstrated
- Network traffic analysis
- DoS detection
- Firewall configuration
- Packet capture interpretation

⚠️ IP addresses have been redacted.  
This lab was conducted in a controlled environment for defensive testing.

