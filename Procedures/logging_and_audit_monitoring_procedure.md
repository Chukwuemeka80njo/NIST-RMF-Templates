# Logging & Audit Monitoring Procedure  
**File:** logging_and_audit_monitoring_procedure.md  
**Category:** Procedures  
**Related Policies:** Audit & Accountability Policy, Continuous Monitoring Policy, Incident Response Policy, Access Control Policy  
**Mapped NIST Controls:** AU-1, AU-2, AU-3, AU-6, AU-8, AU-9, AU-10, AU-12, SI-4, CA-7  

---

## 1. Purpose  
This procedure defines the standards and steps for generating, collecting, storing, reviewing, and protecting audit logs to ensure accountability and timely detection of security-relevant events as required by NIST 800-53.

---

## 2. Scope  
This procedure applies to:  
- All systems that process, store, or transmit organizational data  
- Servers, databases, applications, endpoints, and network devices  
- Cloud platforms, virtual infrastructure, and third-party hosted systems  
- All personnel involved in system administration, security monitoring, and incident response  

---

## 3. Definitions  

**Audit Log:** A chronological record of system activities.  
**Log Source:** Any system, device, or application that generates log data.  
**Log Retention:** Period logs must be stored to meet legal and compliance requirements.  
**SIEM:** A platform that centralizes, correlates, and analyzes log data.  
**Security Event:** Any action or anomaly indicating potential compromise or misuse.

---

## 4. Logging Requirements  

### 4.1 Required Log Types  
Systems must generate logs for:  
- Authentication (login, logout, failed attempts)  
- Privileged account activity  
- User access to sensitive data  
- Configuration changes  
- Network connections (firewall, VPN)  
- Application errors and warnings  
- Security events (malware, IDS/IPS, EDR)  
- System startup/shutdown  

---

### 4.2 Log Format & Content  
Logs must include:  
- Timestamp (synchronized via NTP)  
- User ID / service ID  
- Event type  
- Source and destination IP addresses  
- Device/host identifier  
- Description of the event  
- Success or failure indication  

---

### 4.3 Log Synchronization (Time Management)  
- All systems must synchronize time using approved NTP servers.  
- Time drift must not exceed **±2 seconds**.  
- Time sync failures must generate alerts.

---

## 5. Logging Process  

### 5.1 Log Collection  
1. All logs must be forwarded to the SIEM or centralized logging platform.  
2. Logs must be encrypted in transit and at rest.  
3. Logging failures must be automatically detected and escalated.  

---

### 5.2 Log Retention  
| Log Type | Retention Duration |  
|----------|--------------------|  
| Security logs | Minimum 1 year |  
| Audit logs | 1–7 years (per compliance) |  
| System logs | 90 days on system + stored long-term in SIEM |  
| Cloud logs | 1 year minimum |  

Retention periods must meet regulatory and contractual requirements.

---

### 5.3 Log Storage Protections  
- Logs must be stored in tamper-resistant storage.  
- Only authorized personnel may access logs.  
- Administrative access to logs must itself be logged.  
- Logs must be backed up regularly.

---

## 6. Audit Monitoring & Review  

### 6.1 Daily Reviews  
Security Analysts must review:  
- High and critical SIEM alerts  
- Authentication anomalies  
- Privileged account usage  
- Malware/EDR alerts  
- VPN and remote access logs  

---

### 6.2 Weekly Reviews  
- Review configuration change logs  
- Validate logging completeness  
- Review IDS/IPS and firewall logs  
- Spot-check system logs for anomalies  

---

### 6.3 Monthly Reviews  
- Review user activity trends  
- Analyze failed login patterns  
- Review third-party vendor activity  
- Conduct audit log integrity checks  
- Report trends to the ISO and leadership  

---

## 7. Audit Log Integrity  

### 7.1 Protection Against Tampering  
- Log files must be write-once or protected by access controls.  
- Hashing mechanisms should validate that logs have not been altered.  
- Alerts must trigger on unauthorized log deletion attempts.  

---

### 7.2 Backup of Logs  
- Logs must be backed up daily or per system schedule.  
- Backups must be encrypted and stored securely.  
- Access to log backups must be restricted.

---

## 8. Event Investigation  

### 8.1 Investigation Steps  
1. Collect relevant logs and timestamps.  
2. Determine user accounts or systems involved.  
3. Correlate events with other data sources.  
4. Identify severity and business impact.  
5. Escalate to Incident Response if needed.  

---

### 8.2 Evidence Handling  
- Logs used as evidence must be preserved in original form.  
- Access must be limited and chain-of-custody documented.

---

## 9. Responsibilities  

### Security Team  
- Perform log reviews  
- Maintain SIEM rules  
- Investigate anomalies  
- Report monthly audit findings  

### System Administrators  
- Ensure logging is enabled and functioning  
- Prevent unauthorized log modification  
- Provide system-specific support during investigations  

### ISO  
- Review audit reporting trends  
- Approve exceptions  
- Ensure compliance with NIST requirements  

---

## 10. Exception Management  
Exceptions must include:  
- Written justification  
- Compensating controls  
- ISO approval  
- Annual review  

---

## 11. Enforcement  
Failure to comply with this procedure may result in disciplinary action, up to and including termination of access.

---

## 12. Review  
This procedure must be reviewed **annually** or following major changes to logging tools, systems, or policies.
