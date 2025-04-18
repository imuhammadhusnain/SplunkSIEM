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

- Optimize Data Processing:
Work within the limitations of Splunk’s free version (e.g., 500MB) by optimizing data volume and ensuring that only relevant data is captured and processed.
Fine-tune Snort’s rule set to avoid unnecessary data and focus on the most significant threats.


Guide for Splunk Enterprise Installation:
- Create Account and download Splunk [https://www.splunk.com/en_us/download/splunk-enterprise.html?utm_campaign=google_apac_tier1_anz_en_search_brand_apac_anz_brand_form_fill_tcpa_fy25&utm_source=google&utm_medium=cpc&utm_content=Splunk_Enterprise_Demo_v2&utm_term=splunk%20enterprise%20download&device=c&_bt=733054227318&_bm=p&_bn=g&gad_source=1&gbraid=0AAAAAD8kDz2TyKKh-2PX7NxHit8-Ue3T7&gclid=CjwKCAjw8IfABhBXEiwAxRHlsFs0wyddo6tkh4mP8gZXK1-6xVfgXl17lW7z8wsq9PrABQfdPD-dYBoCPEkQAvD_BwE]
-Once you have created account, now 
- unzip the download file
- Complete installation of the splunk
- Go to Splunk folder:
  Splunk/opt/bin/splunk (start,stop,restart)
- Before starting make sure add 9997 port on web page
- go to ~/../Splunk/etc/system/local
  Create input.conf if not existing and add following script:
          
          [splunktcp://9997]
          disabled = 0
   Save the changes. restart everytime splunk when making any changes. 
        
          sudo netstat -tulnp | grep 9997
  you should see:
    tcp   0.0.0.0:9997 listen ....
- Now restart splunk and try to check splunk list forward=server 



