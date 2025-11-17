# Incident Detection & Response Procedure  
**File:** incident_detection_and_response_procedure.md  
**Category:** Procedures  
**Related Policies:** Incident Response Policy, Audit & Accountability Policy, Continuous Monitoring Policy, Access Control Policy, Contingency Plan  
**Mapped NIST Controls:** IR-1 through IR-9, AU-6, SI-4, CP-2, CP-4  

---

## 1. Purpose  
This procedure defines the required steps for detecting, analyzing, prioritizing, responding to, documenting, and reporting cybersecurity incidents in alignment with NIST SP 800-53 and organizational policies.

---

## 2. Scope  
This procedure applies to:  
- All information systems, networks, cloud environments, and applications  
- All personnel, including employees, contractors, and third-party vendors  
- Security operations staff, system administrators, and incident responders  

---

## 3. Definitions  

**Incident:** A confirmed or suspected event that jeopardizes confidentiality, integrity, or availability.  
**Event:** An observable occurrence within a system or network.  
**IOC (Indicator of Compromise):** Evidence that a system may be compromised.  
**EDR:** Endpoint Detection & Response platform.  
**SIEM:** Security Information & Event Management system.  
**Containment:** Actions taken to limit incident spread or damage.  
**Eradication:** Removal of malicious components.  

---

## 4. Incident Categories  
Incidents are classified as:

| Category | Description |
|---------|-------------|
| **1. Unauthorized Access** | Unauthorized use of accounts or systems |
| **2. Malware Infection** | Virus, ransomware, trojans, worms |
| **3. Denial of Service** | Attempts to disrupt availability |
| **4. Data Breach / Data Exposure** | Unauthorized access, exfiltration, or disclosure |
| **5. Misconfiguration Incident** | Improper configurations leading to security risks |
| **6. Insider Threat** | Malicious or negligent user activity |
| **7. Policy Violation** | User activity against company rules |
| **8. Physical Security Incident** | Attempts to access secure locations |

---

## 5. Incident Detection  

### 5.1 Detection Sources  
Incidents may be detected from:  
- SIEM alerts  
- EDR alerts  
- Firewall, IDS/IPS events  
- Cloud security logs  
- User reports (helpdesk, email, hotline)  
- SOC monitoring  
- Third-party notifications  

### 5.2 Automated Alerting Requirements  
- All critical security systems must send alerts to the SIEM.  
- High-severity alerts must notify the security team immediately.  
- Alert thresholds must be reviewed monthly.

---

## 6. Initial Analysis  

### 6.1 Validation Steps  
1. Verify alert authenticity  
2. Identify affected systems and accounts  
3. Review logs for anomalies  
4. Correlate related events  
5. Determine if the activity is benign or malicious  

### 6.2 Severity Classification  
Severity determines response priority:

| Severity | Response Time | Description |
|---------|----------------|-------------|
| **Critical** | Immediate | Active compromise, data breach, ransomware |
| **High** | ≤1 hour | Privileged misuse, malware infection |
| **Medium** | ≤4 hours | Suspicious activity requiring investigation |
| **Low** | ≤24 hours | Minor anomalies, policy violations |

---

## 7. Incident Response Steps  

### 7.1 Containment  
Depending on the incident type, containment may include:  
- Isolating endpoints from the network  
- Disabling compromised user accounts  
- Blocking malicious IPs or domains  
- Stopping unauthorized processes  
- Revoking API keys or tokens  

### 7.2 Eradication  
Actions include:  
- Removing malware  
- Applying patches and configuration fixes  
- Resetting passwords  
- Cleaning or reimaging systems  
- Removing persistence mechanisms  

### 7.3 Recovery  
- Restore systems from known-good backups  
- Validate system functionality  
- Reinstate user accounts after verification  
- Monitor closely for 72 hours after restoration  

### 7.4 Notification Requirements  
Notify:  
- ISO (immediately for critical incidents)  
- Management  
- Legal, HR (as applicable)  
- Affected users (as required)  
- External regulators or authorities (if required)

---

## 8. Evidence Collection  

### 8.1 Forensic Evidence Must Include  
- System logs  
- Network logs  
- EDR telemetry  
- File hashes  
- Screenshots and user reports  
- Timeline of events  

### 8.2 Chain-of-Custody Requirements  
- Document who accessed evidence  
- Record storage locations  
- Ensure integrity protections (hashing)

---

## 9. Documentation Requirements  
Every incident must include:  
- Summary and incident ID  
- Date/time detected  
- Affected systems and users  
- Root cause  
- Impact assessment  
- Actions taken (containment, eradication, recovery)  
- Lessons learned  
- Preventative recommendations  

---

## 10. Post-Incident Review  
A lessons-learned meeting must occur within **5 business days** of incident closure. It must cover:  
- Improvements to controls  
- Logging gaps  
- Policy updates  
- User training needs  
- System hardening steps  

---

## 11. Responsibilities  

### Security Team  
- Monitor systems and alerts  
- Lead incident investigations  
- Document actions and maintain evidence  
- Report findings and improvements  

### System Administrators  
- Support containment and remediation  
- Provide system-specific logs  
- Implement corrective actions  

### ISO  
- Approve incident classification  
- Ensure compliance with reporting laws  
- Authorize closure of critical incidents  

---

## 12. Enforcement  
Failure to follow this procedure may result in disciplinary action, access suspension, or termination depending on severity.

---

## 13. Review  
This procedure must be reviewed **annually** or following:  
- Major system upgrades  
- Changes to logging or detection tools  
- Introduction of new technologies or services  
