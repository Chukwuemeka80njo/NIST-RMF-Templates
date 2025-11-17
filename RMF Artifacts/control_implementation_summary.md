# Control Implementation Summary (CIS)

**File:** control_implementation_summary.md  
**Category:** RMF Artifacts  
**Mapped Standard:** NIST SP 800-53 Rev 5  
**Impact Level:** Moderate

---

## 1. Purpose
The CIS provides a summary of how each applicable NIST 800-53 security control is implemented for the system.

---

## 2. System Information
- System Name: <Insert>  
- System ID: <Insert>  
- Boundary Classification: Internal / Cloud / Hybrid

---

## 3. Control Implementation Table
| Control ID | Control Name | Implementation Summary | Status |
|------------|--------------|-------------------------|--------|
| AC-2 | Account Management | All accounts follow automated provisioning & quarterly review. | Implemented |
| AC-5 | Separation of Duties | Conflicting roles segregated via RBAC. | Implemented |
| AU-6 | Audit Review | Logs reviewed weekly; alerts automated. | Implemented |
| SC-13 | Cryptographic Protection | TLS 1.2+ enforced; AES-256 for data-at-rest. | Implemented |

(Add full list of controls depending on the system’s baseline.)

---

## 4. Inherited Controls
Document inherited controls from:
- Cloud providers (AWS, Azure, GCP)
- Enterprise shared services

---

## 5. Approval
- Security Control Assessor: ____________  
- System Owner: ____________  
- Date: ____________
