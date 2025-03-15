# SIEM-Honeypot



In this blog, I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. We will use a custom PowerShell script to look up the attackers Geolocation information and plot it on the Azure Sentinel Map! LEARN THIS IN DEPTH AND PUT THIS ON YOUR RESUME!




# Cybersecurity Lab: Azure Sentinel and Honeypot Setup

## Overview

Welcome to the GitHub repository for the Cybersecurity Lab on setting up Azure Sentinel, a cloud-based Security Information and Event Management (SIEM), and a Virtual Machine Honeypot. This lab provides hands-on exposure to an SIEM without the need for corporate experience, offering insights into real-world cybersecurity scenarios. During the lab, I recorded the latitude and longitude of attackers and presented the data on a world map within the Azure environment.

![WorldMap at Azure](https://res.cloudinary.com/dkqvrhzs3/image/upload/v1700374777/worldmapsiem_ebjg11.png)

## Initial Setup and Configuration

1. **Azure Subscription Setup:**
   - Created an Azure subscription.
   - Provisioned a virtual machine in Azure, intentionally making it highly vulnerable by turning off external and Windows firewalls.

2. **Log Management:**
   - Established a log repository in Azure using Log Analytics Workspace to ingest logs from the vulnerable virtual machine.

3. **Azure Sentinel Configuration:**
   - Configured Azure Sentinel to create a map visualizing attacker data.

## Extracting and Mapping Log Data

1. **PowerShell Script:**
   - Utilized PowerShell to extract IP addresses from Windows logs on the virtual machine.

2. **Geolocation Mapping:**
   - Sent extracted IP addresses to a third-party API to derive latitude and longitude data.
   - Created a custom log with geographic information to visualize attacks on a world map.

## Continuous Monitoring and Analysis

1. **Lab Monitoring:**
   - Continuously monitored and analyzed attacker data.

2. **Insights Gained:**
   - Observed distribution and frequency of attacks, gaining insights into the nature of cyber threats.

## Conclusion

The cybersecurity lab successfully demonstrated the practical application of tools such as Azure Sentinel and honeypots. The experience deepened my understanding of cybersecurity and emphasized the importance of proactive defense measures.

## Future Updates

Stay tuned for more cybersecurity content and practical demonstrations. Future updates will include additional experiments and labs, providing valuable insights into the evolving field of cybersecurity.

Feel free to explore the repository and use the provided resources for your own learning and experimentation. Contributions and feedback are welcome!

## Inspiration

This cybersecurity lab project was inspired by the invaluable guidance and insights shared in the YouTube video titled "SIEM Tutorial for Beginners | Azure Sentinel Tutorial MAP with LIVE CYBER ATTACKS!
" by Josh Madakor. The step-by-step instructions, practical demonstrations, and clear explanations provided in the video served as a foundation for setting up Azure Sentinel and the Virtual Machine Honeypot.

[Link to the YouTube Video](https://youtu.be/RoZeVbbZ0o0?list=PL85GlCRx5t-Lo3Z5aoSFwozqEkuQtuRmk)

Feel free to explore and support the creator's channel for more insightful content in the cybersecurity domain.

**Special thanks to Josh Madakor for the inspiration and knowledge-sharing!**


**Happy Learning and Stay Secure!**
