# Configuration Management / Change Control Procedure  
**File:** configuration_management_procedure.md  
**Category:** Procedures  
**Related Policies:** Configuration Management Policy, System & Communications Protection Policy, Access Control Policy  
**Mapped NIST Controls:** CM-1, CM-2, CM-3, CM-4, CM-5, CM-6, CM-7, CM-8, CM-9, CM-10, CM-11, AC-3, SI-2  

---

## 1. Purpose  
This procedure establishes the required steps for requesting, reviewing, approving, implementing, documenting, and monitoring configuration changes to organizational information systems. It ensures secure and controlled modifications in alignment with NIST 800-53 change management expectations.

---

## 2. Scope  
This procedure applies to all:  
- Production systems, servers, applications, and cloud platforms  
- Development and staging environments  
- Network devices, endpoints, and virtual infrastructure  
- Configuration baselines and system images  
- Employees, contractors, and administrators who request or implement changes  

---

## 3. Definitions  

**Configuration Item (CI):** Any system component that is subject to change control.  
**Change Request (CR):** A formal request to modify a configuration item.  
**Emergency Change:** A change required to quickly address an immediate threat or outage.  
**Baseline Configuration:** Approved and documented system configuration settings.  
**CAB (Change Advisory Board):** A group that reviews and approves changes.

---

## 4. Procedure  

### 4.1 Change Request Submission  
All changes must begin with a documented **Change Request (CR)** that includes:  
- Description of change  
- Business justification  
- Impact assessment (security, operational, user impact)  
- Rollback plan  
- Testing plan  
- Scheduled implementation window  
- Assigned owner  

CRs must be submitted through the approved ticketing system.

---

### 4.2 Change Classification  
CRs must be categorized as:

**1. Standard Change**  
- Low-risk, pre-approved, recurring  
- Example: routine OS updates, approved patches  

**2. Normal Change**  
- Requires full CAB review and approval  

**3. Emergency Change**  
- Required to fix security incidents, outages, or vulnerabilities  
- Can be implemented prior to CAB approval but must be documented after

---

### 4.3 Review and Approval  
1. All Normal Changes must be reviewed by the CAB.  
2. Security impact must be assessed by the ISO or Security Team.  
3. High-risk changes require ISO approval and possibly executive approval.  
4. No changes may be implemented without documented approval.

---

### 4.4 Testing Requirements  
Before deployment:  
- All changes must be tested in a non-production environment.  
- Testing must confirm no negative impact on functionality, security, or compliance.  
- Test results must be attached to the change request.

---

### 4.5 Implementation  
During implementation:  
- Only authorized personnel may perform changes.  
- Logging and monitoring must be enabled.  
- Implement changes during approved maintenance windows unless emergency.  
- Maintain real-time communication for high-impact changes.

---

### 4.6 Verification & Validation  
After implementation:  
- Validate system functionality.  
- Verify that monitoring and logging are operational.  
- Confirm no unauthorized changes occurred.  
- Document results in the change record.

---

### 4.7 Rollback  
A documented rollback plan is mandatory for all changes except low-risk standard changes.  
Rollback must be executed if:  
- System instability occurs  
- Security impact is identified  
- Change fails validation testing  

Rollback actions must be documented.

---

### 4.8 Configuration Baseline Management  
- Maintain documented baselines for all critical systems.  
- Baselines must be reviewed annually.  
- Unauthorized changes must be investigated immediately.  
- Deviations must be corrected or approved through change control.

---

### 4.9 Configuration Inventory  
Maintain an inventory including:  
- System name  
- CI description  
- Owner  
- Version information  
- Installation date  
- Last change date  

Inventory must be updated after every approved change.

---

## 5. Responsibilities  

### System Administrators  
- Submit and implement CRs  
- Maintain baselines and configuration inventories  
- Perform testing and validation  

### Change Advisory Board (CAB)  
- Review and approve CRs  
- Evaluate risks, impacts, and scheduling  

### Information Security Officer (ISO)  
- Assess security impact  
- Ensure alignment with NIST requirements  

### Users / Requestors  
- Provide accurate change details  
- Participate in testing when required  

---

## 6. Enforcement  
Violations of this procedure may result in disciplinary action and revocation of system access.

---

## 7. Review  
This procedure must be reviewed **annually** or whenever significant system changes occur.

