# Backup & Restoration Procedure  
**File:** backup_and_restoration_procedure.md  
**Category:** Procedures  
**Related Policies:** Contingency Planning Policy, System Maintenance Policy, Risk Assessment Policy  
**Mapped NIST Controls:** CP-6, CP-7, CP-9, CP-10, MP-4, SI-12, RA-3  

---

## 1. Purpose  
This procedure defines the requirements and steps for securely performing system and data backups, storing backup media, testing restorations, and ensuring business continuity in alignment with NIST 800-53 contingency planning controls.

---

## 2. Scope  
This procedure applies to:  
- All production systems, applications, and databases  
- Cloud and on-premise infrastructure  
- Fileservers, endpoints, and storage systems containing organizational data  
- Personnel responsible for backup operations, cybersecurity, or system administration  
- Critical business systems defined in the Business Impact Analysis (BIA)

---

## 3. Definitions  

**Backup:** A copy of data or system configuration stored for recovery purposes.  
**Full Backup:** An exact copy of all selected data.  
**Incremental Backup:** Backs up only data changed since the last backup.  
**Differential Backup:** Backs up data changed since the last full backup.  
**RPO (Recovery Point Objective):** Maximum acceptable data loss.  
**RTO (Recovery Time Objective):** Maximum acceptable time to restore systems.  
**Immutable Backup:** A backup that cannot be altered or deleted.

---

## 4. Backup Schedule  

### 4.1 Data Backup Frequency  
| System Type | Frequency | Method |  
|-------------|-----------|--------|  
| **Critical systems** | Daily | Full or incremental |  
| **High-value systems** | Every 48 hours | Incremental |  
| **Standard systems** | Weekly | Full backup |  
| **End-user devices** | Daily | Cloud-synced backup |  
| **Logs & audit data** | Daily | Automated log archival |

---

### 4.2 Backup Types  
- **Full backups**: Performed weekly at minimum.  
- **Incremental backups**: Performed daily.  
- **Configuration backups**: After major system changes.  
- **Database snapshots**: Minimum every 24 hours.  
- **VM snapshots** (if applicable): Prior to system updates or maintenance.  

---

## 5. Backup Storage Requirements  

### 5.1 Storage Locations  
Backups must be stored across:  
- **Primary storage** (local or cloud-based)  
- **Secondary/offsite storage** (encrypted cloud or remote data center)  
- **Offline/immutable storage** for ransomware resilience  

### 5.2 Encryption Requirements  
- Backups must be encrypted **in transit and at rest**  
- Minimum encryption standard: **AES-256**  
- Encryption keys must be centrally managed and rotated annually  

### 5.3 Retention Requirements  
| Data Type | Retention |  
|----------|-----------|  
| System configurations | 1 year |  
| Application data | 1–7 years (per compliance needs) |  
| Personnel & HR data | 7 years |  
| Financial records | 7 years |  
| Logs & auditing data | 1 year (minimum) |

---

## 6. Backup Process  

### 6.1 Daily Operational Steps  
1. Verify backup jobs started successfully.  
2. Confirm no backup failures or incomplete jobs.  
3. Document anomalies and escalate to the system owner.  
4. Confirm backup storage capacity is sufficient.

---

### 6.2 Weekly Backup Tasks  
1. Perform a full backup of all applicable systems.  
2. Validate backup integrity using system-generated hash checks.  
3. Store a copy in offsite or immutable storage.

---

### 6.3 Monthly Backup Review  
- Review job logs and reports  
- Confirm compliance with retention schedules  
- Validate recovery readiness  
- Remove outdated or expired backups  
- Update the asset inventory with new or retired systems  

---

## 7. Restoration Procedure  

### 7.1 Restoration Authorization  
Restorations may only be performed when approved by:  
- System Owner  
- Information Security Officer (ISO)  
- Incident Response Lead (if restoration is due to a security event)

---

### 7.2 Restoration Steps  
1. Identify required backup version.  
2. Validate integrity of the backup before restoration.  
3. Notify stakeholders of service interruptions.  
4. Restore data or system from backup repository.  
5. Validate successful restoration:  
   - System functionality  
   - Data integrity  
   - Security controls still active  
6. Document the restoration event.  

---

### 7.3 Restoration Testing  
- Perform **quarterly restoration tests**  
- Test a mix of system-level and file-level restores  
- Document results and improvement actions  
- Report findings during cybersecurity governance meetings  

---

## 8. Responsibilities  

### Backup Administrators  
- Execute daily/weekly/monthly backup tasks  
- Resolve backup errors and failures  
- Maintain backup documentation  

### System Owners  
- Identify critical systems and RTO/RPO requirements  
- Approve restorations  

### Security Team  
- Validate backup encryption  
- Ensure secure offsite backup handling  
- Evaluate risks related to retention and access  

### Information Security Officer (ISO)  
- Approve exceptions  
- Oversee compliance with NIST and organizational policies  

---

## 9. Exception Management  
Exceptions to this procedure require:  
- Documented business justification  
- Compensating controls  
- ISO approval  
- Annual review  

---

## 10. Enforcement  
Failure to follow this procedure may result in disciplinary action, policy violations, or compliance failures.

---

## 11. Review  
This procedure must be reviewed **annually** or following major changes to the backup environment.
