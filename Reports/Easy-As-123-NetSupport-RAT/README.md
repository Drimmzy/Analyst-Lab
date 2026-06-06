# Forensic Analysis: NetSupport RAT Infection Case Study

## Challenge Overview
This project contains a formal Incident Response Report detailing a packet analysis of a Windows host compromise. The investigation was conducted using a network packet capture (PCAP) from the "Easy As 123" challenge provided by Malware-Traffic-Analysis.net.

The objective was to locate an unauthorized presence on the corporate network, profile the compromised endpoint and domain user, and identify the specific family of malware active in the environment.

## Tools Used
* **Analysis Tool:** Wireshark
* **Investigation Tool:** Isolated Ubuntu Virtual Machine 
* **Malware Identified:** NetSupport Manager Remote Access Trojan (RAT)

## Investigation Highlights
Through packet analysis the following actions were completed:
1. Extracted network identifiers including the client's internal IP and hardware MAC address.
2. Used Kerberos to pinpoint the exact Active Directory domain user handle.
3. Used SMB2 directory connections to discover the compromised user's human full name.

## Repository Contents
* **`Incident_Report_EasyAs123_Malware_Analysis.pdf`**: The formal Incident Response document containing the complete timeline, Indicators of Compromise (IoCs), and post-incident remediation.

---
*Note: To comply with safety regulations, no live malware samples, extracted payload binaries, or raw malicious PCAP files are hosted in this repository.*
