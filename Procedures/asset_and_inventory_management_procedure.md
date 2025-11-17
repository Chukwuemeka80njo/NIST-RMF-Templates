# Asset & Inventory Management Procedure  
**File:** asset_and_inventory_management_procedure.md  
**Category:** Procedures  
**Related Policies:** Asset Management Policy, Configuration Management Policy, Access Control Policy, Media Protection Policy  
**Mapped NIST Controls:** CM-8, PM-5, MP-6, MP-7, IA-4, AC-19  

---

## 1. Purpose  
This procedure establishes the processes for identifying, classifying, recording, tracking, and maintaining organizational assets throughout their lifecycle to ensure proper protection and accountability of information systems and data.

---

## 2. Scope  
This procedure applies to:  
- All IT assets including hardware, software, virtual machines, cloud resources, mobile devices, and network equipment  
- All data assets including PII, sensitive information, and configuration data  
- All employees, contractors, and system administrators responsible for maintaining asset inventories  

---

## 3. Definitions  

**Asset:** Any hardware, software, data, or system that supports business operations.  
**Asset Owner:** Individual responsible for managing and approving changes to an asset.  
**Configuration Item (CI):** Component tracked as part of the CMDB.  
**CMDB:** Configuration Management Database containing asset metadata.  
**Lifecycle:** Stages including acquisition, deployment, maintenance, and disposal.  

---

## 4. Responsibilities  

### Asset Owners  
- Maintain accurate asset details  
- Approve asset changes  
- Ensure proper classification and security assignments  

### IT Operations  
- Register hardware and virtual assets in the CMDB  
- Track system configuration changes  
- Perform routine asset reconciliations  

### Security Team  
- Validate inventory accuracy  
- Classify assets based on criticality  
- Monitor for unauthorized or rogue devices  

---

## 5. Asset Identification  

### 5.1 Hardware Assets  
All new hardware must be:  
1. Assigned an asset ID  
2. Labeled with a barcode or tag  
3. Recorded in the CMDB with:  
   - Model, serial number  
   - Assigned user  
   - System owner  
   - IP/MAC address  
   - Location  
   - Support lifecycle information  

### 5.2 Software Assets  
Software must be:  
- Approved through the change management process  
- Assigned an owner  
- Tracked by version, license, and installation location  
- Periodically reviewed for unauthorized software  

### 5.3 Cloud & Virtual Assets  
Cloud resources must include metadata:  
- Instance type, region, resource group  
- Creation date  
- Responsible team  
- Data classification  
- Security controls enabled (logging, encryption, MFA)

---

## 6. Asset Classification  
Assets must be classified based on:  
- **Impact Level:** Low, Moderate, High  
- **Data Sensitivity:** Public, Internal, Confidential, Regulated  
- **Operational Criticality:** Mission-essential, Support, Non-critical  

The ISO must approve classifications for High-impact systems.

---

## 7. Asset Inventory Maintenance  

### 7.1 Scheduled Updates  
- Inventory must be updated within **24 hours** of:  
  - Acquisition  
  - Deployment  
  - Reassignment  
  - Disposal  

### 7.2 Automated Discovery  
- Network scans  
- Endpoint management tools  
- Cloud asset discovery agents  
- Vulnerability management tools  

### 7.3 Monthly Reconciliation  
Asset owners must validate:  
- Current status  
- Accurate user assignment  
- License compliance  
- Configuration baseline  

---

## 8. Unauthorized Asset Handling  

If an unauthorized or rogue device is detected:  
1. Immediately isolate it from the network  
2. Notify the Security Team  
3. Investigate and document root cause  
4. Remove or approve the asset depending on results  
5. Perform an incident analysis if malicious activity is suspected  

---

## 9. Configuration Tracking  
Each tracked asset must include:  
- Baseline configurations  
- Patch levels  
- Installed applications  
- Security agent status  
- Network access permissions  

Changes must follow the Change Management Procedure.

---

## 10. Asset Decommissioning  

### 10.1 Secure Removal Steps  
Before disposal or repurposing:  
- Wipe data using approved sanitization methods  
- Remove encryption keys  
- Update CMDB status to “Retired”  
- Record disposal date and method  

### 10.2 Physical Disposal  
Hardware must be:  
- Destroyed or sanitized by approved vendors  
- Documented with serialized certificates of destruction  

---

## 11. Documentation Requirements  
All asset-related activities must be documented, including:  
- Inventory updates  
- Ownership changes  
- Classification updates  
- Decommissioning records  
- Investigation of unauthorized assets  

---

## 12. Review  
This procedure must be reviewed **annually**, or after major infrastructure or organizational changes.
