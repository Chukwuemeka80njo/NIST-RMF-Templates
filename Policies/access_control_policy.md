✅ **Perfect — we will start with ALL Security Policies.**
You will receive **14 complete, audit-ready, NIST-aligned policies**, each formatted professionally and suitable for GitHub.

I will generate **Policy #1 now**, then you can say **“Next”** to continue to Policy #2, and so on.

---

# 📄 **1. Access Control Policy (ACP)**

**File Name:**
`Policies/access_control_policy.md`

---

# **ACCESS CONTROL POLICY**

**Version:** 1.0
**Approval Date:** *(insert date)*
**Owner:** Information Security Officer (ISO)
**Classification:** Internal / Restricted

---

# **1. Purpose**

The purpose of this Access Control Policy is to establish requirements for managing user access to organizational information systems, applications, networks, and data in accordance with NIST SP 800-53 Rev5, ensuring confidentiality, integrity, and availability.

---

# **2. Scope**

This policy applies to:

* All employees, contractors, and third parties
* All organizational information systems
* All devices accessing company resources (on-premises and cloud)

---

# **3. Policy Statements**

## **3.1 Account Management**

* All system accounts must be approved by the system owner or designated manager.
* Accounts must be created following the User Access Request Procedure.
* Dormant accounts must be disabled after **30 days** of inactivity.
* Accounts must be reviewed **quarterly** to confirm validity.

## **3.2 Least Privilege**

* Users will be granted only the minimum access necessary to perform job duties.
* Privileged accounts (administrator, root, superuser) require:

  * Manager approval
  * Multi-factor authentication (MFA)
  * Quarterly reauthorization
* Privileged activities must be logged and monitored.

## **3.3 Separation of Duties**

* No single individual may perform actions that allow concealment of unauthorized activity.
* Conflicting roles must be segregated (e.g., developer != production approver).

## **3.4 Access Authorization**

* Access must be granted based on job role (RBAC).
* Users must acknowledge the Acceptable Use Policy before system access is activated.
* Access provisioning and de-provisioning must follow the formal procedure.

## **3.5 Authentication Requirements**

* MFA is required for all remote access and all privileged accounts.
* Passwords must conform to:

  * Minimum 14 characters
  * Complexity enabled (upper/lowercase, number, symbol)
  * Changed every 90 days (or compliant with NIST 800-63B if modernized)

## **3.6 Remote Access**

* Remote access must use encrypted channels (VPN, HTTPS, SSH).
* Remote access must be logged, monitored, and restricted to approved personnel.

## **3.7 Access Review and Recertification**

* Managers must review user access **quarterly**.
* HR must notify IT Security within **24 hours** of employee termination.

## **3.8 Third-Party Access**

* Third-party users must sign an NDA and Security Agreement.
* Access must be time-bound and restricted to required systems only.

---

# **4. Responsibilities**

### **Information Security Officer (ISO)**

* Maintains this policy
* Oversees account management compliance

### **System Owners**

* Approve access to their systems
* Validate quarterly access reviews

### **IT Administrators**

* Create, modify, and remove accounts
* Ensure MFA enforcement
* Monitor privileged accounts

### **Users**

* Use access responsibly
* Maintain password confidentiality
* Report suspicious access immediately

---

# **5. Enforcement**

Violations of this policy may result in disciplinary action, termination of access, or legal consequences.

---

# **6. References**

* NIST SP 800-53 Rev5 AC-1 through AC-20
* NIST SP 800-63B Digital Identity Guidelines
* ISO/IEC 27001: A.9 Access Control

---

# **7. Review Cycle**

This policy must be reviewed annually or when significant system or organizational changes occur.

