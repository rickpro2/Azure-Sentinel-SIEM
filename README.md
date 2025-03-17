# Cybersecurity Lab: Azure Sentinel and Honeypot Setup
<img src="images/Title Logo.png"/>

## Overview

In this cybersecurity lab, I set up a cloud-based Security Information and Event Management (SIEM) system using Microsoft Sentinel and deployed a vulnerable Virtual Machine (VM) as a honeypot to attract cyberattacks. I observed live attacks, including Remote Desktop Protocol (RDP) brute-force attempts, originating from various locations worldwide.

To analyze attack data, I created a Log Analytics workspace to ingest logs from the VM. Using the VM’s Event Viewer, I identified failed login attempts under “failed audits.” I then downloaded a PowerShell script that extracted attacker IP addresses and queried ipgeolocation.io to retrieve geolocation data. The script generated a data file, which I transferred to my main computer and uploaded into the Log Analytics workspace.

With these logs in Sentinel, I crafted a custom Kusto Query Language (KQL) query to visualize the geographic locations of attackers on the Azure Sentinel Map.

This project was inspired by the YouTube video <a href="https://youtu.be/g5JL2RIbThM?si=GUjx0TV-xzc0zU9Q" target="_new">"Cyber Home Lab from ZERO and Catch Attackers! Free, Easy, and REAL (Microsoft Sentinel 2025)"</a> by Josh Madakor. The step-by-step instructions, practical demonstrations, and clear explanations in the video were instrumental in setting up Azure Sentinel and deploying the Virtual Machine Honeypot.

### Learning Objectives:

- Configuration & Deployment of Microsoft Azure virtual machines, Log Analytics Workspaces, and Microsoft Sentinel
- Hands-on experience with a SIEM (Security Information and Event Management)
- Understanding Windows Security Event logs
- Using KQL to query logs
- Display attack data on a dashboard with Workbooks (Failed RDP World Map)

### Languages and Utilities Used

- PowerShell
- Azure Virtual Machine
- Microsoft Sentinel

### Environments Used
 - Windows 10

## Attack Map
<img src="images/Map.png"/>

## Conclusion

The cybersecurity lab successfully demonstrated the practical application of tools such as Azure Sentinel and honeypots. The experience deepened my understanding of cybersecurity and emphasized the importance of proactive defense measures.