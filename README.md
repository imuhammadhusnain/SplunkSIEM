# SplunkGuard-Cybersecurity-Vigilance-through-SIEM-Dashboard

# Project Overview

In this project, I focused on designing and implementing a Splunk-based dashboard for cybersecurity monitoring, creating custom Snort NIDS rules, and simulating realistic cyber-attacks to gather data. The aim was to analyze traffic, identify vulnerabilities, and develop responses using various cybersecurity tools and techniques. The project also helped me gain hands-on experience in dealing with network security and data management challenges.

# Implementation Steps for the Project

- Set up Splunk Environment:

Install Splunk Enterprise and configure it to accept log data from other systems.
You can install Splunk Universal Forwarder on relevant machines (e.g., Snort system) to forward logs to the Splunk instance.

- Configure and Install Snort IDS:
Install Snort on a Linux-based machine (e.g., Kali Linux or Ubuntu).
Write custom Snort rules to detect specific attack patterns.
Set up Snort to forward its log data to Splunk for analysis.

- Simulate Cyber Attacks:
Use tools like Nmap, Hydra, and Hping3 to simulate real-world attacks such as port scanning, brute-force attacks, and DoS.
Capture attack traffic and ensure that it’s processed by Snort and indexed in Splunk.

- Develop Splunk Dashboard:
Design a Splunk dashboard that displays real-time attack data.
Create Splunk search queries to analyze attack data and visualize it in an informative and easy-to-understand format.
Optimize Data Processing:

-Optimize Data Processing:

Work within the limitations of Splunk’s free version (e.g., 500MB) by optimizing data volume and ensuring that only relevant data is captured and processed.
Fine-tune Snort’s rule set to avoid unnecessary data and focus on the most significant threats.

