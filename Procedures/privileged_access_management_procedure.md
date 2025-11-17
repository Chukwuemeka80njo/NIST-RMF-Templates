# Privileged Access Management Procedure  
**File:** privileged_access_management_procedure.md  
**Category:** Procedures  
**Related Policies:** Access Control Policy, Identification & Authentication Policy, Security Assessment & Authorization Policy  
**Mapped NIST Controls:** AC-2(2), AC-5, AC-6, AC-6(1/2/5), AC-17, AC-18, IA-2, IA-5, AU-2, AU-12, CM-5, CM-6  

---

## 1. Purpose
This procedure establishes the steps for granting, modifying, reviewing, and revoking privileged access within the organization’s information systems. It ensures privileged access is controlled, monitored, limited, and compliant with NIST SP 800-53 Rev 5 requirements.

---

## 2. Scope
This procedure applies to:
- System administrators  
- Network administrators  
- Database administrators  
- Cloud platform administrators  
- Security analysts with elevated access  
- Any user with root, sudo, admin, or equivalent roles  

---

## 3. Definitions
**Privileged Access:** Any account or role that can modify system configurations, security settings, user accounts, or sensitive data.

**Privileged User:** An employee or contractor assigned elevated system permissions.

**PAM:** Privileged Access Management – processes and tools for controlling privileged accounts.

---

## 4. Responsibilities
- **System Owner:** Approves privileged access requests.  
- **IT Security:** Reviews justification, enforces MFA, monitors logs.  
- **System Administrators:** Implement access changes and maintain audit trails.  
- **HR / Managers:** Validate job-role requirements for privileged access.  

---

## 5. Procedure Steps

### 5.1 Privileged Access Request
1. User submits a Privileged Access Request Form.  
2. Request must include:
   - Business justification  
   - Required systems and permission levels  
   - Duration of access (Temporary or Standard)  
3. Manager verifies role need.  
4. System Owner provides final approval.

No privileged access is granted without documented approval.

---

### 5.2 Identity Verification & MFA
Before enabling privileged access:

- Identity must be verified by HR or security.
- Multifactor authentication (MFA) must be enforced.
- Default passwords MUST be changed before first login.

---

### 5.3 Provisioning Privileged Access
System Administrators must:

1. Create a **unique privileged account** (no shared accounts).  
2. Assign the **minimum permissions required** (least privilege).  
3. Document:
   - Username  
   - Role assigned  
   - Access purpose  
   - Expiration date  
4. Enable privileged session monitoring if available.  
5. Store logs centrally.

---

### 5.4 Privileged Activity Monitoring
For all privileged accounts:

- Enable command/keystroke logging where supported.  
- Log all admin actions (AU-2, AU-12).  
- Forward logs to SIEM.  
- Review privileged activity at least **weekly**.  
- Investigate anomalies immediately.

---

### 5.5 Temporary Privileged Access
- Duration must be clearly specified.  
- Access automatically expires on the defined date.  
- Extension requires a new approved request.

---

### 5.6 Privileged Access Review
Performed **quarterly** by IT Security.

Review includes:
- User list with privileged roles  
- Access justification  
- Terminated users  
- Orphaned accounts  
- Accounts with unused privileges  

Findings are documented and remediated within 10 business days.

---

### 5.7 Privileged Access Revocation
Revocation must occur:
- Immediately upon role change  
- Immediately upon termination  
- Immediately if suspicious activity is detected  
- Automatically after temporary access expires  

System Administrators must:
1. Disable account or remove elevated role.  
2. Document revocation in the access tracking log.  
3. Notify security upon completion.

---

## 6. Emergency Privileged Access (Break Glass)
1. Emergency account is sealed and monitored.  
2. Security authorizes activation.  
3. All actions are logged and reviewed within 24 hours.  
4. Password is reset immediately after use.

---

## 7. Recordkeeping
The following must be retained for **at least 1 year**:
- Privileged access request forms  
- Approval logs  
- Provisioning and revocation records  
- Privileged session logs  
- Quarterly review reports  

---

## 8. Enforcement
Violation of this procedure may result in:
- Removal of privileges  
- Disciplinary action  
- Termination of employment  
- Legal action where applicable

---

## 9. Revision History
| Version | Date | Description | Author |
|--------|------|-------------|--------|
| 1.0 | YYYY-MM-DD | Initial creation | Security Team |

