# Logging Plan

## Purpose
This document defines the logs collected in the Active Directory lab to enable detection, 
investigation, and incident response.

---

## Log Sources

### Domain Controller (DC001)
- Windows Security Event Logs
- Account login events
- Account management events
- Privilege assignment events

**Why:**  
These logs allow detection of brute-force attempts, password spraying, and privilege abuse.

---

### Windows Clients (Client01, Client02)
- Windows Security Event Logs
- User logon/logoff activity
- Process creation events
- PowerShell execution events

**Why:**  
logs help identify suspicious user behaviour and malware execution.

---

### Linux Server (Linux01)
- Authentication logs (`auth.log`)
- System logs (`syslog`)
- Service logs (as applicable)

**Why:**  
Linux systems often host backend services and tooling. Authentication and system
logs provide visibility into unauthorized access and misuse.

---

### SIEM
- Centralised log ingestion
- Correlation and alerting
- Historical log retention

**Why:**  
SIEM provides a single point of visibility for security monitoring and
investigation across all systems.

---

## Logging Goals
- Establish a baseline of normal behaviour
- Detect abnormal authentication patterns
- Identify unauthorized privilege changes
- Support incident investigation and response
