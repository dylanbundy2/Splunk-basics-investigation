# Splunk-basics-investigation
## Overview This project documents hands-on experience using Splunk Enterprise to analyse security logs and investigate suspicious authentication activity.  The investigation was completed as part of practical SOC training using TryHackMe. 
## Objectives
- Understand Splunk search functionality
- Analyse authentication logs
- Identify suspicious login behaviour
- Use SPL queries to investigate events

---

## Tools Used
- Splunk Enterprise
- SPL (Search Processing Language)
- Windows Authentication Logs

---

## Investigation Process

### 1. Log Exploration
Reviewed available log sources and identified authentication-related events.

### 2. Failed Login Analysis
Used SPL queries to identify repeated failed authentication attempts.

Example SPL query:
```spl
index=main sourcetype=WinEventLog:Security EventCode=4625
