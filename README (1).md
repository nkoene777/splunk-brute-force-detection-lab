<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Detect a Brute Force Attack with Splunk

**Project Link:** [View Project](https://nextwork.ai/projects/56e136bf-5194-4d4b-82e2-c72022e0e7c1)

**Author:** Nikita Koene  
**Email:** nikitakoene52@gmail.com

---

![Image](https://nextwork.ai/serene_vermilion_beautiful_tamarind/uploads/56e136bf-5194-4d4b-82e2-c72022e0e7c1_alwurwwo)

## Building a Real-Time Brute Force Detection System

### Project goals and motivation



## Installing and Launching Splunk Enterprise

### Setting up the SIEM platform

I configured Splunk Enterprise as a SIEM and connected it to Windows Security Event Logs. I used SPL to identify failed login attempts, simulated a brute-force attack, and created a security dashboard to visualize suspicious authentication activity.

Key Objectives
Configured Splunk Enterprise as a SIEM.
Ingested and analyzed Windows Security Event Logs.
Created SPL queries to detect failed logins.
Simulated and detected a brute-force attack.
Built a dashboard showing login trends and targeted accounts.
Configured automated alerting for spikes in failed login activity.

![Image](https://nextwork.ai/serene_vermilion_beautiful_tamarind/uploads/56e136bf-5194-4d4b-82e2-c72022e0e7c1_mzscgcny)

### Confirming Splunk Web is live



## Ingesting Windows Security Logs into Splunk

### Connecting Splunk to real security data

.I configured Splunk to collect Windows Security Event Logs and verified that real security events were successfully flowing into Splunk

![Image](https://nextwork.ai/serene_vermilion_beautiful_tamarind/uploads/56e136bf-5194-4d4b-82e2-c72022e0e7c1_a99tmnwf)

### Understanding the data source and sourcetype

I cofigured Splunk to monitor Windows Security Event Logs, which contain events such as login attempts and other security-related activity.

Splunk assigns these events the sourcetype WinEventLog:Security.

## Exploring Security Data with SPL

### Why raw logs aren't enough

I reviewed the raw Windows security events collected by Splunk and used SPL queries to organize and analyze events by type and frequency. This demonstrated why manually searching through large volumes of logs was not an effective way to detect threats.

![Image](https://nextwork.ai/serene_vermilion_beautiful_tamarind/uploads/56e136bf-5194-4d4b-82e2-c72022e0e7c1_l9ydj08u)

### The core problem every SIEM solves

Thousands of security events made it difficult and time-consuming to identify suspicious activity manually. Important security events could easily become buried among normal system activity, demonstrating the need for SPL queries and automated detection.

## Simulating and Detecting a Brute Force Attack

### Creating and catching a real attack pattern

I simulated a brute-force attack by generating multiple failed login attempts on my Windows machine. I then created targeted SPL queries to detect the failed login activity and built a timeline chart to visualize the attack as a spike in events.

![Image](https://nextwork.ai/serene_vermilion_beautiful_tamarind/uploads/56e136bf-5194-4d4b-82e2-c72022e0e7c1_a9rq8mqz)

## Building the Brute Force Monitor Dashboard

### Turning detections into persistent visibility

I created a Splunk security dashboard that provided an at-a-glance view of brute-force activity. I saved the timeline search as a dashboard panel, added panels showing the most targeted accounts and recent failed login attempts, and used the dashboard to quickly identify suspicious activity.

## Automating Threat Detection with Scheduled Alerts

### Why alerts outperform dashboards for autonomous monitoring

## Project Reflection and Key Takeaways

### Tools and concepts mastered

Through this project, the following was completed:

Splunk Enterprise – Used as a SIEM to collect, search, and analyze security logs.
SPL (Search Processing Language) – Used to search and analyze Windows Security events.
Windows Security Logs – Used to identify login attempts and other security activity.
Brute-Force Attack Detection – Learned how to identify repeated failed login attempts and suspicious authentication activity.
Splunk Dashboards – Learned how to turn SPL searches into visual panels for security monitoring.
Timeline Panels – Used to visualize when suspicious activity occurred.
Log Correlation and Analysis – Learned how raw security events can be analyzed and turned into useful security findings.
SIEM Concepts – Gained practical experience with log ingestion, detection, investigation, and security monitoring.


---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/56e136bf-5194-4d4b-82e2-c72022e0e7c1)*
