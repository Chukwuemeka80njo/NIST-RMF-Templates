# Contingency / Recovery Plan Template

> Replace all bracketed text with system-specific information.

---

## 1. System Information

- **System Name:** [System Name]  
- **Acronym:** [Acronym]  
- **Unique ID:** [System ID]  
- **Organization:** [Org Name]  
- **System Owner:** [Name, Title]  
- **Authorizing Official (AO):** [Name, Title]  
- **Contingency Plan Manager:** [Name, Title]  
- **Last Updated:** [MM/DD/YYYY]

---

## 2. Purpose & Scope

- **Purpose:**  
  [Describe the objective of this contingency plan.]

- **Scope:**  
  [Identify what systems, components, services, and locations are covered.]

- **Assumptions:**  
  [Key assumptions necessary for the plan, e.g., staff availability.]

---

## 3. Roles & Responsibilities

| Role | Name | Responsibilities |
|------|------|------------------|
| Contingency Plan Manager | [Name] | [Duties] |
| System Owner | [Name] | [Duties] |
| Technical Recovery Lead | [Name] | [Duties] |
| Communications Lead | [Name] | [Duties] |
| Support Staff | [Name(s)] | [Duties] |

---

## 4. System Description

Provide a summary of the system:

- **System Function:** [High-level description]  
- **Architecture Overview:** [Servers, network segments, cloud services]  
- **Key Components:**  
  - [Component 1]  
  - [Component 2]  
  - [Component 3]  

- **Dependencies:**  
  - [External systems or services]  

---

## 5. Business Impact Analysis (BIA)

### 5.1 Criticality and Priority

| Function | Description | Maximum Allowable Downtime (MAD) | Priority |
|----------|-------------|----------------------------------|----------|
| [Function 1] | [Description] | [Time] | [High/Med/Low] |
| [Function 2] | [Description] | [Time] | [High/Med/Low] |

### 5.2 Impact of Disruption

- **Operational Impact:**  
  [Describe effects on operations.]

- **Financial Impact:**  
  [Costs or lost revenue.]

- **Security & Compliance Impact:**  
  [Impact on confidentiality, integrity, availability.]

---

## 6. Preventive Measures

List actions to reduce likelihood of system outage:

- Backups and replication  
- Redundant hardware  
- UPS / power protection  
- Monitoring and alerts  
- Patch management  
- Vulnerability scanning  
- Physical security  

Add system-specific details:

[Add details here]

---

## 7. Contingency Strategies

Include recovery strategies per component:

| Component | Recovery Strategy | Location | RTO | RPO |
|-----------|-------------------|----------|-----|-----|
| [Server/DB/App] | [Process to restore] | [Primary / Alternate] | [Time] | [Time] |
| [Server/DB/App] | [Process to restore] | [Primary / Alternate] | [Time] | [Time] |

**RTO:** Recovery Time Objective  
**RPO:** Recovery Point Objective  

---

## 8. Incident Response Integration

Describe how this plan aligns with the Incident Response Plan:

- Detection & reporting  
- Initial analysis  
- Classification  
- Escalation  
- Activation of contingency procedures  

[Add system-specific connections]

---

## 9. Activation & Notification Procedures

### 9.1 Activation Criteria

The plan is activated when:

- ☐ System outage exceeds [Time]  
- ☐ Security incident requires isolation  
- ☐ Data corruption detected  
- ☐ Disaster affects facility or cloud environment  

### 9.2 Notification List

| Person/Team | Contact Info | Role |
|--------------|----------------|------|
| [Name] | [Email/Phone] | [Role] |
| [Name] | [Email/Phone] | [Role] |

---

## 10. Recovery Procedures

Detailed step-by-step restoration steps:

1. **Initial Assessment**  
   [Check system status, logs, indicators.]

2. **Stabilization**  
   [Stop data loss, isolate affected systems.]

3. **Recovery Implementation**  
   - Restore backups from [location]  
   - Rebuild servers  
   - Reconfigure applications  
   - Validate data integrity  

4. **System Testing**  
   [Verify system is functional and secure.]

5. **Return to Normal Operations**  
   [Restore full service, notify stakeholders.]

---

## 11. Backup & Restoration

- **Backup Types:**  
  - Full  
  - Incremental  
  - Differential  

- **Backup Frequency:** [Daily/Weekly/etc.]  
- **Backup Storage Location:** [Primary/Offsite/Cloud]  
- **Retention Period:** [Timeframe]

### Restoration Testing

- Last test date: [MM/DD/YYYY]  
- Test results: [Pass/Fail/Notes]

---

## 12. Training & Testing Requirements

Describe training:

- Annual contingency plan training  
- Tabletop exercises  
- Full restoration test every [time period]  

Document past tests:

| Test Date | Type | Participants | Result | Notes |
|-----------|------|--------------|--------|-------|
| [Date] | [Tabletop/Full] | [Names] | [Result] | [Notes] |

---

## 13. Plan Maintenance

Explain how the plan will be updated:

- Review every 12 months  
- Update after major system changes  
- Update after real incidents  

Next scheduled update: [MM/DD/YYYY]

---

## 14. Approvals

- **System Owner:**  
  Signature: _______________________  
  Date: _______________________

- **Contingency Plan Manager:**  
  Signature: _______________________  
  Date: _______________________

- **Authorizing Official (AO):**  
  Signature: _______________________  
  Date: _______________________

---

