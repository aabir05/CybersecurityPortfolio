# Internal Security & Compliance Audit: Botium Toys

**Author:** Aabir Benyahia  
**Context:** Google Cybersecurity Professional Certificate (Coursera) — Simulated Security Audit Lab  
**Frameworks & Standards:** NIST Cybersecurity Framework (CSF), PCI DSS, GDPR, SOC Type 1 & Type 2  

---

## 1. Project Overview & Business Context
Completed as a practical internal security audit lab for the Google Cybersecurity Professional Certificate on Coursera, this case study evaluates the security posture of **Botium Toys**—a small U.S.-based toy retailer operating a single physical location (main office, storefront, and warehouse) alongside a rapidly expanding global e-commerce presence.

As international online orders grew, the IT department faced mounting pressure to protect customer payment data and personal information while maintaining compliance with U.S. and European Union regulations. The objective of this audit was to review the IT manager's initial NIST Cybersecurity Framework (CSF) scope, goals, and risk assessment report, evaluate existing administrative, technical, and physical controls, and deliver prioritized remediation recommendations.

---

## 2. Audit Scope, Assets & Risk Baseline
* **Audit Scope & Goals:** Assess Botium Toys' entire security program—covering physical hardware, end-user devices, storefront/warehouse inventory, e-commerce and database systems, internal networks, data retention, and legacy infrastructure—to identify control gaps and compliance risks.
* **Baseline Risk Rating (8 / 10 — High Risk):** While potential impact from individual asset loss was rated medium due to incomplete asset classification (*NIST CSF Identify* function), overall exposure to data breaches and regulatory fines was rated high due to unrestricted internal data access, unencrypted cardholder data, and missing continuity safeguards.

---

## 3. Security Controls Assessment Summary

| Control | Status | Audit Observation |
| :--- | :---: | :--- |
| **Least Privilege** | No (Gap) | All employees can access internally stored data, including PII/SPII and cardholder records. |
| **Separation of Duties** | No (Gap) | No role-based division of critical system and payment administration tasks. |
| **Disaster Recovery Plans** | No (Gap) | No formal recovery plan exists to restore operations following a cyber incident or outage. |
| **Backups** | No (Gap) | Critical business and customer data are not backed up. |
| **Intrusion Detection System (IDS)** | No (Gap) | No active network monitoring/alerting tool deployed to detect suspicious traffic. |
| **Encryption** | No (Gap) | Credit card data is accepted, processed, transmitted, and stored locally without encryption. |
| **Password Policies** | No (Gap) | Nominal policy exists, but requirements are too minimal to prevent unauthorized access. |
| **Legacy System Maintenance** | No (Gap) | End-of-life systems rely on irregular manual monitoring with unclear intervention procedures. |
| **Password Policies** | Yes (Weak) | A nominal policy exists but lacks modern complexity standards (length, numbers, symbols). |
| **Firewall & Antivirus Software** | Yes | Configured firewall rules block unauthorized traffic; antivirus is installed and monitored. |
| **Physical Controls** | Yes | Sufficient locks, up-to-date CCTV surveillance, and functioning fire detection/prevention systems. |

---

## 4. Regulatory Compliance Evaluation
* **Payment Card Industry Data Security Standard (PCI DSS) — Non-Compliant:** Fails core requirements due to unencrypted cardholder data in transit and at rest, unrestricted employee access to payment records, and weak password enforcement.
* **General Data Protection Regulation (GDPR) — Partially Compliant:** Meets breach notification (72-hour E.U. customer notification plan) and internal privacy documentation requirements, but fails data security/privacy and asset classification standards due to lack of encryption and access restrictions.
* **System and Organization Controls (SOC Type 1 & Type 2) — Partially Compliant:** Data integrity controls are in place, but formal user access policies, confidentiality protections (encryption) for PII/SPII, and proper authorization boundaries for data availability are missing.

---

## 5. Strategic Recommendations for IT Leadership
1. **Enforce Access Controls:** Implement role-based access control (RBAC), least privilege, and separation of duties to isolate cardholder data and PII/SPII from general staff (addressing PCI DSS and SOC gaps).
2. **Implement End-to-End Encryption & Password Management:** Deploy strong encryption across payment transaction touchpoints and local databases, and adopt a centralized password manager enforcing modern complexity standards.
3. **Establish Disaster Recovery & Automated Backups:** Develop a documented disaster recovery plan and schedule automated, encrypted backups to guarantee business continuity and data availability.
4. **Upgrade Network & Legacy System Security:** Deploy an Intrusion Detection System (IDS) for real-time threat alerting, and replace ad-hoc manual legacy monitoring with standardized maintenance schedules or system upgrades.
5. **Complete Asset Classification (NIST CSF Identify):** Inventory and classify all IT and data assets by criticality to align security investments with business impact and fulfill GDPR inventory requirements.

---

## 6. Key Competencies Demonstrated
`Internal Security Auditing` • `NIST CSF` • `Risk Assessment & Scoring` • `PCI DSS, GDPR & SOC Compliance` • `Security Controls Evaluation` • `Stakeholder Risk Communication`
