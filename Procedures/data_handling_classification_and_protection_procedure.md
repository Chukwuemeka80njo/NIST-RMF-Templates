# Data Handling, Classification & Protection Procedure  
**File:** data_handling_classification_and_protection_procedure.md  
**Category:** Procedures  
**Related Policies:** Data Classification Policy, Privacy Policy, Access Control Policy, Media Protection Policy, System & Communications Protection Policy  
**Mapped NIST Controls:** MP-2, MP-4, MP-5, MP-6, PL-2, AC-3, AC-4, SC-12, SC-13, SC-28, PT-2  

---

## 1. Purpose  
This procedure establishes standardized processes for classifying, handling, transmitting, storing, and disposing of organizational data to ensure confidentiality, integrity, and availability in compliance with NIST SP 800-53 and federal information security requirements.

---

## 2. Scope  
This procedure applies to:  
- All employees, contractors, vendors, and system users  
- All organizational data, regardless of format (electronic, printed, verbal)  
- All environments including on-premises, cloud, mobile, and remote  
- All systems containing organizational, regulated, or sensitive data  

---

## 3. Definitions  

**Data Classification:** Categorization based on sensitivity, regulatory requirements, and impact.  
**PII:** Personally Identifiable Information.  
**PHI:** Protected Health Information.  
**CUI:** Controlled Unclassified Information.  
**Encryption:** Process of protecting data using cryptographic controls.  
**Secure Disposal:** Sanitization or destruction of data according to NIST 800-88.  

---

## 4. Data Classification Levels  
Data must be classified into one of the following categories:

| Classification Level | Description |
|----------------------|-------------|
| **Public** | Approved for public release |
| **Internal Use** | Organizational use only, low sensitivity |
| **Confidential** | Sensitive business data, restricted to authorized personnel |
| **Regulated** | Includes PII, PHI, CUI, PCI-DSS, FERPA, etc. |

System Owners must approve classifications for **Confidential** or **Regulated** data.

---

## 5. Data Handling Requirements  

### 5.1 Public  
- May be distributed without restriction  
- Must not contain internal metadata or system details  

### 5.2 Internal Use  
- Stored in approved systems  
- Not to be shared externally without approval  
- Must not be stored on personal devices  

### 5.3 Confidential  
- Access limited to authorized personnel  
- Must use encryption in transit and at rest  
- Must not be emailed externally unless approved and encrypted  

### 5.4 Regulated Data (PII / PHI / CUI)  
- Must follow the highest level of protections  
- Encryption required at all times  
- Prohibited from unencrypted removable media  
- Access requires MFA and logging  
- Must be stored only in approved FedRAMP or secure environments  

---

## 6. Data Transmission Requirements  
- All sensitive data must use TLS 1.2+ encryption  
- File transfers must use SFTP, HTTPS, or approved secure channels  
- Emailing regulated data requires encryption tools (e.g., secure portals)  
- Data must never be transmitted through:  
  - Personal email  
  - Public cloud storage without authorization  
  - SMS or unencrypted chat platforms  

---

## 7. Data Storage Requirements  

### 7.1 Electronic Storage  
- Must use approved systems with encryption-at-rest  
- Backups must maintain the same classification protections  
- Access rights must follow least privilege  
- Local device storage must be justified and encrypted  

### 7.2 Physical Storage  
- Confidential/regulated data must be stored in locked areas  
- Printed documents must be secured when not in use  
- Access must be logged where feasible  

---

## 8. Data Access Requirements  
- Access granted based on classification and job role  
- Annual access reviews required for all data repositories  
- Privileged accounts must be reviewed quarterly  
- Data owners must approve high-risk access  

---

## 9. Data Retention Requirements  
- Retention periods must follow regulatory and business requirements  
- Expired records must be securely destroyed  
- Temporary data storage must be minimized  

---

## 10. Data Disposal Procedure  
All data disposal must comply with **NIST SP 800-88**.

### 10.1 Electronic Data  
- Secure overwrite  
- Cryptographic erase  
- Physical destruction of media  

### 10.2 Physical Data  
- Cross-cut shredding  
- Secure destruction vendor with certificate  

### 10.3 Documentation  
- All disposal events must be logged  
- For regulated data, disposal must be verified by a second reviewer  

---

## 11. Data Protection Requirements  
- MFA required for systems containing sensitive data  
- Access logs must be forwarded to the SIEM  
- Data loss prevention (DLP) tools must monitor high-risk activity  
- Encryption keys must follow key management requirements (SC-12/SC-13)  
- Portable devices must enforce full-disk encryption  

---

## 12. Incident Handling for Data Exposure  
If sensitive data is suspected of being exposed:  
1. Immediately notify Security Team  
2. Preserve evidence and logs  
3. Initiate Incident Response Procedure  
4. Determine scope (affected records, users)  
5. Notify leadership, legal, and regulators as required  
6. Document root cause and corrective actions  

---

## 13. User Responsibilities  
All personnel must:  
- Handle data based on proper classification  
- Use only approved storage and transmission tools  
- Report unauthorized access or suspicious behavior  
- Complete annual security and privacy training  

---

## 14. Enforcement  
Violations may result in:  
- Access revocation  
- Disciplinary action  
- Contract termination  
- Legal consequences for intentional violations  

---

## 15. Review  
This procedure must be reviewed **annually** or following changes to classification rules, privacy laws, or data systems.
