# Active Directory + Microsoft Sentinel SIEM Lab (Azure)

## Overview
Deployed a Windows Server 2022 Active Directory Domain Controller in Microsoft Azure and monitored authentication security events using Microsoft Sentinel SIEM.

Built a detection pipeline for repeated failed login attempts (Event ID 4625), simulating brute-force credential attack behavior in an enterprise environment.

---

## Environment
- Platform: Microsoft Azure
- Server: Windows Server 2022 Domain Controller
- Domain: cooperlab.local
- SIEM: Microsoft Sentinel
- Log Source: Windows Security Event Logs (Event ID 4625)

---

## Key Implementation Steps
- Promoted a Windows Server VM to an Active Directory Domain Controller
- Created domain users and configured authentication policies
- Generated failed login attempts to produce Security Event ID 4625
- Ingested Windows Security logs into Sentinel using Azure Monitor Agent + Data Collection Rules
- Built an analytics rule to detect failed login spikes
- Created a SOC-style workbook dashboard for monitoring authentication threats

---

## Detection Rule
**Failed Login Spike (4625)**  
Triggers when failed authentication attempts exceed a threshold within a short time window.

---

## Dashboard Panels
- Failed Logins Over Time  
- Top Targeted Accounts  

---

## Skills Demonstrated
- Active Directory administration  
- Windows event log analysis  
- SIEM ingestion and detection engineering  
- Microsoft Sentinel analytics + dashboards  
- Azure cloud security fundamentals  

---



---

