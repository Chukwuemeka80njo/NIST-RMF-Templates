# Continuous Monitoring Procedure  
**File:** continuous_monitoring_procedure.md  
**Category:** Procedures  
**Related Policies:** Continuous Monitoring Policy, Risk Assessment Policy, Incident Response Policy, Configuration Management Policy  
**Mapped NIST Controls:** CA-7, RA-5, SI-4, PM-5, AU-6, AU-12, CM-3  

---

## 1. Purpose  
This procedure establishes the requirements and steps for continuously monitoring organizational systems to detect security weaknesses, anomalies, policy violations, system changes, and emerging threats in alignment with NIST 800-53 continuous monitoring expectations.

---

## 2. Scope  
This procedure applies to:  
- All information systems, networks, applications, and cloud services  
- All on-premise, remote, and hybrid environments  
- Logs, alerts, vulnerability data, system configurations, and performance  
- Security, IT operations, and system administration personnel  

---

## 3. Definitions  

**Continuous Monitoring (ConMon):** Ongoing observation and analysis of system activity to identify security risks.  
**Security Information and Event Management (SIEM):** A system that aggregates and analyzes logs for security events.  
**Health Monitoring:** Tracking CPU, memory, disk, network, and uptime metrics.  
**Configuration Drift:** Unauthorized or unintended changes to system baselines.  
**Alert:** A notification triggered by abnormal or suspicious activity.

---

## 4. Monitoring Components  

### 4.1 System Logs  
Log categories monitored include:  
- Authentication and access logs  
- Network traffic logs  
- Application logs  
- Security tool logs (AV, EDR, IDS/IPS)  
- Firewall and VPN logs  
- Administrative activity logs  
- Cloud audit logs (e.g., AWS CloudTrail, Azure Activity Logs)

---

### 4.2 Security Tools  
Continuous monitoring requires:  
- Endpoint Detection & Response (EDR)  
- Vulnerability scanners  
- SIEM platform  
- Intrusion Detection/Prevention Systems (IDS/IPS)  
- Email security and anti-malware  
- Cloud security posture monitoring tools (CSPM)

---

### 4.3 Configuration Monitoring  
Systems must be monitored for:  
- Unauthorized software installation  
- Configuration changes  
- Missing patches  
- Privilege escalation events  
- Deviation from baselines  

---

## 5. Procedure  

### 5.1 Log Collection & Aggregation  
1. All logs must be forwarded to the SIEM or centralized log repository.  
2. Logs must include timestamps, event type, user ID, and system identifiers.  
3. Logs must be retained according to policy (minimum **1 year**).  
4. Logging failures must be detected and escalated.

---

### 5.2 Daily Monitoring Tasks  
Security Analysts must:  
- Review SIEM dashboards  
- Investigate high and critical alerts  
- Validate endpoint protection alerts  
- Confirm system uptime and health metrics  
- Check for unauthorized changes  

All findings must be documented.

---

### 5.3 Weekly Monitoring Tasks  
1. Review vulnerability scan summaries.  
2. Review patch compliance reports.  
3. Evaluate IDS/IPS alerts.  
4. Validate that all logs are flowing correctly.  
5. Identify anomalies in user behavior or privilege use.

---

### 5.4 Monthly Monitoring Tasks  
1. Conduct configuration drift analysis.  
2. Review privileged account activity logs.  
3. Perform threat hunting activities.  
4. Review third-party vendor access logs.  
5. Report monitoring metrics to leadership.

---

### 5.5 Event Investigation  
When a suspicious event is detected:  
1. Collect relevant logs and evidence.  
2. Assess severity and potential impact.  
3. Escalate to the Incident Response Team if required.  
4. Document investigation details.  
5. Track the event to closure.

---

### 5.6 Alerts & Escalation  
Alerts must be classified as:  
- **Critical:** Immediate response and escalation  
- **High:** Response within 4 hours  
- **Medium:** Response within 24 hours  
- **Low:** Response within 72 hours  

Critical and High alerts must be escalated to IT Management and ISO.

---

### 5.7 Reporting & Metrics  
Monthly reporting must include:  
- Number of alerts by severity  
- Number of incidents escalated  
- Patch and vulnerability posture  
- Configuration drift findings  
- System uptime and performance metrics  
- Compliance with monitoring SLAs  

---

## 6. Responsibilities  

### Security Team / SOC  
- Perform daily, weekly, and monthly monitoring  
- Maintain SIEM rules and alerting thresholds  
- Investigate suspicious activity  
- Prepare monthly security reports  

### System Administrators  
- Maintain logging configurations  
- Provide system access for investigations  
- Support configuration baseline enforcement  

### ISO  
- Oversee continuous monitoring strategy  
- Approve exceptions  
- Review reports and escalate trends  

---

## 7. Exception Management  
Exceptions must be:  
- Documented with justification  
- Include compensating controls  
- Approved by the ISO  
- Reviewed annually  

---

## 8. Enforcement  
Non-compliance with this procedure may result in disciplinary action and system access restrictions.

---

## 9. Review  
This procedure must be reviewed **annually** or following major changes to security monitoring tools or environments.
