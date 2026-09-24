# Controls and Compliance Checklist
## Botium Toys – Internal Security Audit

**Course:** Google Cybersecurity Certificate – Course 2: Play It Safe: Manage Security Risks  
**Activity:** Portfolio Activity – Conduct a Security Audit  
**Date:** May 2026  

---

## Instructions

This checklist is based on a review of the [Botium Toys: Scope, Goals, and Risk Assessment Report](https://github.com/Ghost25-tech/Botium-toys-security-audit/blob/main/Botium%20Toys_%20Scope%2C%20goals%2C%20and%20risk%20assessment%20report.pdf). For each item, I determined whether the control or compliance best practice is currently in place at Botium Toys, based on the details provided in the risk assessment.

---

## Part 1: Controls Assessment Checklist

> **Question:** Does Botium Toys currently have this control in place?

| Yes | No | Control | Control Type | Notes |
|-----|-----|---------|-------------|-------|
| | ✔ | Least Privilege | Administrative | All employees currently have access to internally stored data, including cardholder data and PII/SPII. Least privilege has not been implemented. |
| | ✔ | Disaster Recovery Plans | Administrative | No disaster recovery plans are currently in place. |
| | ✔ | Password Policies | Administrative | A password policy exists, but requirements are nominal and do not meet current minimum complexity standards (e.g., 8+ characters, letters + numbers + special characters). |
| | ✔ | Separation of Duties | Administrative | Access controls pertaining to least privilege and separation of duties have not been implemented. |
| ✔ | | Firewall | Technical | The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules. |
| | ✔ | Intrusion Detection System (IDS) | Technical | The IT department has not installed an intrusion detection system (IDS). |
| | ✔ | Backups | Technical | There are no disaster recovery plans and the company does not have backups of critical data. |
| ✔ | | Antivirus Software | Technical | Antivirus software is installed and monitored regularly by the IT department. |
| | ✔ | Manual Monitoring, Maintenance, and Intervention for Legacy Systems | Technical | While legacy systems are monitored and maintained, there is no regular schedule in place and intervention methods are unclear. |
| | ✔ | Encryption | Technical | Encryption is not currently used to ensure the confidentiality of customers' credit card information stored in the internal database. |
| | ✔ | Password Management System | Technical | There is no centralized password management system that enforces the password policy's minimum requirements. |
| ✔ | | Locks (Offices, Storefront, Warehouse) | Physical | The store's physical location has sufficient locks. |
| ✔ | | Closed-Circuit Television (CCTV) Surveillance | Physical | Up-to-date CCTV surveillance is in place at the store's physical location. |
| ✔ | | Fire Detection/Prevention (Fire Alarm, Sprinkler System, etc.) | Physical | Functioning fire detection and prevention systems are in place. |

---

## Part 2: Compliance Checklist

### Payment Card Industry Data Security Standard (PCI DSS)

> **Question:** Does Botium Toys currently adhere to this compliance best practice?

| Yes | No | Best Practice | Notes |
|-----|-----|--------------|-------|
| | ✔ | Only authorized users have access to customers' credit card information. | All employees currently have access to internally stored data, including cardholder data. |
| | ✔ | Credit card information is stored, accepted, processed, and transmitted in a secure environment. | Encryption is not used; credit card data is stored in the internal database without proper security. |
| | ✔ | Implement data encryption procedures to better secure credit card transaction touchpoints and data. | Encryption is not currently in place. |
| | ✔ | Adopt secure password management policies. | Password policy requirements are nominal and a centralized password management system is not in place. |

---

### General Data Protection Regulation (GDPR)

| Yes | No | Best Practice | Notes |
|-----|-----|--------------|-------|
| | ✔ | E.U. customers' data is kept private/secured. | Encryption is not used; access controls for PII/SPII are not enforced. |
| ✔ | | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. | The IT department has established a breach notification plan for E.U. customers. |
| | ✔ | Ensure data is properly classified and inventoried. | Asset management is inadequate; the IT department does not fully know which assets are at risk. |
| ✔ | | Enforce privacy policies, procedures, and processes to properly document and maintain data. | Privacy policies, procedures, and processes have been developed and are enforced among IT department members and other employees. |

---

### System and Organizations Controls (SOC Type 1, SOC Type 2)

| Yes | No | Best Practice | Notes |
|-----|-----|--------------|-------|
| | ✔ | User access policies are established. | Least privilege and separation of duties have not been implemented; all employees have broad data access. |
| | ✔ | Sensitive data (PII/SPII) is confidential/private. | All employees can access PII/SPII; encryption is not used. |
| ✔ | | Data integrity ensures the data is consistent, complete, accurate, and has been validated. | The IT department has integrated controls to ensure data integrity. |
| | ✔ | Data is available to individuals authorized to access it. | Access controls have not been implemented — data is available to all employees, not just authorized ones. |

---

## Recommendations

Based on the risk assessment and the controls/compliance gaps identified above, the following actions are recommended for Botium Toys' IT manager to communicate to stakeholders:

### High Priority
1. **Implement Least Privilege and Separation of Duties** — Restrict employee access to only the data and systems necessary for their role. This directly reduces the risk of insider threats and data breaches.
2. **Enable Encryption for Credit Card and PII Data** — Encrypt all sensitive customer data (credit card info, PII/SPII) stored in the internal database to comply with PCI DSS and GDPR.
3. **Install an Intrusion Detection System (IDS)** — Detect and respond to potential network threats or unauthorized access attempts in real time.
4. **Establish Disaster Recovery and Data Backup Plans** — Create and test a disaster recovery plan; regularly back up critical data to ensure business continuity.

### Medium Priority
5. **Strengthen Password Policy and Deploy a Password Management System** — Update password requirements to current complexity standards and implement a centralized password manager.
6. **Create a Regular Schedule for Legacy System Monitoring** — Document and schedule maintenance intervals and define clear intervention procedures for end-of-life systems.

### Lower Priority
7. **Classify and Inventory All Assets** — Conduct a full asset inventory to understand what data and systems exist, which are most critical, and what their risk level is. This aligns with the NIST CSF Identify function.
