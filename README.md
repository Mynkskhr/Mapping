# Mapping

# 🧩 Compliance Maturity Chain  
### From NIS2 → EU AI Act → Cyber Resilience Act → ISO 27001 → Customer Trust

---

## **1️⃣ NIS2 Directive – Security Foundations**
- Establishes **organizational and technical measures** for essential and important entities.  
- Focus areas: Asset management, incident response, supplier risk, and business continuity.  
- **Outcome:** A secure operational baseline for digital infrastructure and critical services.  

> 🧠 **Dependency:** The AI Act and CRA assume NIS2 maturity for core security capabilities.

---

## **2️⃣ EU AI Act – Accountable and Explainable AI**
- Introduces risk-based governance for AI systems (high-risk use cases such as critical infrastructure monitoring and leak detection).  
- Requires **human-in-the-loop (HITL)** oversight, bias controls, and AI lifecycle documentation.  
- Builds on the NIS2 security baseline for **data integrity and traceability.**

> 🧠 **Dependency:** Without a secure NIS2 foundation, AI compliance cannot be sustained.

---

## **3️⃣ Cyber Resilience Act (CRA) – Product and Software Security**
- Focuses on **secure-by-design development**, vulnerability handling, and post-market monitoring.  
- Ensures connected products (including AI-based utilities platforms) maintain cyber resilience throughout their lifecycle.  
- Extends the organizational controls of NIS2 and technical controls of AI Act into product engineering.

> 🧠 **Dependency:** NIS2 = governance layer; CRA = technical implementation layer.

---

## **4️⃣ ISO/IEC 27001 – Integrated Management System**
- Provides the formal Information Security Management System (ISMS) that unites NIS2, AI Act, and CRA controls.  
- Maps organizational processes, risk management, and continuous improvement to audit-ready frameworks.  
- Acts as a “control hub” ensuring consistency and evidence across all EU requirements.

> 🧠 **Dependency:** ISO 27001 turns regulatory compliance into sustainable operations.

---

## **5️⃣ Customer Trust & EU Market Readiness**
- When NIS2, AI Act, and CRA controls are implemented within an ISO 27001 ISMS:  
  - Customers see **transparency and accountability.**  
  - Regulatory audits become simpler and faster.  
  - Market confidence and partnership opportunities increase.

---

## ⚡ **Critical Insight: Unified Governance Builds Trust**
> Achieving compliance with NIS2, EU AI Act, and CRA is not a checkbox exercise — it is a chain of interdependent maturity levels.  
>  
> When implemented through a unified framework (such as Thinkwerke’s CIR³ Framework):  
> - Each directive reinforces the others.  
> - Governance becomes proactive rather than reactive.  
> - The organization gains **resilience, audit readiness, and lasting customer trust.**

---

# ENISA-Linked Compliance Overview  
### NIS2 · EU AI Act · Cyber Resilience Act · ISO 27001 · Cross-Regulation Governance  
*Prepared for Diehl Metering / Preventio – by Thinkwerke (CIR³ Framework)*  

| **Regulation**                                | **Key ENISA Focus / Articles**                                                                                                                                                | **What ENISA Expects**                                                                                                                                                     | **Utility-Specific Compliance Actions**                                                                                                                                     | **Deliverables / Evidence**                                                                                     |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| **NIS2 Directive (Directive (EU) 2022/2555)** | - Art. 21: Security & Risk Mgmt  <br> - Art. 23: Incident Notification  <br> - Art. 25: Supervision  <br> - ENISA Baseline Measures (2023)                                    | - Board-level cybersecurity accountability  <br> - Risk management & policy framework  <br> - Supply chain & incident control  <br> - 24h/72h/1-month incident reporting   | - Map OT/IT network & secure data flows (Azure + IoT)  <br> - CIRATS integration for rapid incident alerts  <br> - Adopt ENISA Baseline 49 Controls                         | - Risk Register (aligned to ISO 27001)  <br> - Incident Response Plan & Reports  <br> - NIS2 Compliance Matrix  |
| **EU AI Act (Reg. (EU) 2024/1689)**           | - Art. 9: Risk Mgmt System  <br> - Art. 14: Human Oversight (HITL)  <br> - Art. 15: Accuracy & Robustness  <br> - Annex III (High-Risk AI)  <br> - Annex IV (Conformity File) | - Secure & transparent AI systems  <br> - HITL oversight and accountability  <br> - Documentation of data sources & model lineage  <br> - Bias, drift & robustness testing | - Identify AI systems as “high-risk” (leak detection, anomaly detection)  <br> - Define HITL process (Databricks workflow)  <br> - Implement AI risk register + model cards | - AI Risk Assessment  <br> - HITL Roles & Log Evidence  <br> - Model Cards & Technical File (Annex IV)          |
| **EU Cyber Resilience Act (CRA)**             | - Annex I: Security by Design  <br> - Annex II: CE Marking  <br> - Art. 10–11: Vulnerability Disclosure  <br> - ENISA IoT Security Guidelines                                 | - Secure product lifecycle (SDLC)  <br> - Continuous vulnerability management  <br> - Transparent update & patch policy  <br> - Disclosure process within 24h              | - Apply ENISA CRA IoT guidelines to smart meters/gateways  <br> - SBOM (Software Bill of Materials) for all firmware  <br> - Integrate CRA conformity checks in CI/CD       | - CE Technical Documentation  <br> - SBOM + Patch Logs  <br> - CRA Declaration of Conformity                    |
| **ISO 27001 Alignment (2022 Update)**         | - ENISA ISMS Maturity Model  <br> - Annex A cross-mapping                                                                                                                     | - Continuous improvement loop for ISMS  <br> - Risk & control verification  <br> - Audit trail integrity                                                                   | - Map ENISA baseline → ISO controls  <br> - Embed NIS2/AI/CRA controls into ISMS                                                                                            | - ISO 27001 Readiness Audit Pack  <br> - Control Evidence Summary                                               |
| **Cross-Regulation Governance**               | - ENISA Cybersecurity Maturity Model  <br> - Threat Landscape 2024  <br> - Incident Notification Templates                                                                    | - Unified governance model across regulations  <br> - Clear accountability and risk visibility  <br> - Automated evidence and dashboards                                   | - Deploy CIR³ framework (Continuous Intelligence, Integration, Resilience)  <br> - Sentinel & Grafana dashboards  <br> - Compliance dashboard for board oversight           | - Unified Compliance Dashboard  <br> - ENISA-formatted Quarterly Report  <br> - Cross-Regulation Control Matrix |



# NIS2 Directive – Core Control Requirements Checklist  
*Aligned with ENISA, NIS2 Directive Articles 21 & 23, and ISO/IEC 27001 Control Mapping*

| **Requirement**                                    | **Control Objective**                                                                                            | **Linked Article / Reference** | **Status / Implementation Evidence**      |
| -------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ------------------------------ | ----------------------------------------- |
| **Asset Inventory in CMDB**                        | Ensure all critical assets and systems are identified, tracked, and linked to configuration management database. | **Art. 21(2)(a)**              | ☐ Entry exists in CMDB (ID recorded)      |
| **Vulnerability Management Process**               | Establish continuous vulnerability identification, assessment, and remediation with defined schedule.            | **Art. 21(2)(d)**              | ☐ Linked process and schedule defined     |
| **Incident Reporting & Contact Runbook**           | Implement reporting procedures, including defined roles and escalation contacts, integrated into repository.     | **Art. 23**                    | ☐ Incident response runbook documented    |
| **Backup & Recovery Procedures**                   | Maintain tested and documented backup and recovery plans to ensure business continuity.                          | **Art. 21(2)(e)**              | ☐ Backup and recovery tested and verified |
| **Supplier Risk Assessment**                       | Evaluate suppliers, dependencies, and containers for security posture and contractual risk.                      | **Art. 21(2)(d,f)**            | ☐ Supplier risk analysis completed        |
| **Data Transfer & Legal Basis (Conditional – EU)** | Validate GDPR and cross-border data transfer compliance for EU-based processing.                                 | **GDPR / NIS2 interplay**      | ☐ Data transfer and legal basis reviewed  |



# NIS2 Directive – Databricks on Azure Implementation Checklist
*Aligned with ENISA Baseline Measures · ISO/IEC 27001 Annex A · Preventio Leak Detection Platform*  

| **NIS2 Control** | **Databricks / Azure Configuration** | **Data Processing Practice (Bronze → Silver → Gold)** | **Audit Evidence / Notes** |
|------------------|--------------------------------------|-------------------------------------------------------|-----------------------------|
| **Asset Inventory (Art.21(2)(a))** | Use Unity Catalog for asset registration and Azure Resource Graph to sync resources to ServiceNow CMDB. | Register every dataset, Delta table, and ML model with owner, classification, and retention policy. | CMDB record IDs, Unity Catalog ownership reports, configuration snapshots. |
| **Vulnerability Management (Art.21(2)(d))** | Apply Databricks cluster policies, enforce runtime pinning, enable Defender for Cloud, and scan base images for vulnerabilities. | Integrate vulnerability scanning in CI/CD pipeline; perform monthly runtime upgrade validation cycles. | Defender vulnerability reports, CI/CD pipeline logs, runtime upgrade tickets. |
| **Incident Reporting (Art.23)** | Stream Databricks audit logs to Microsoft Sentinel and trigger Logic Apps for automated 24-hour incident notifications. | Tag each incident with related Unity Catalog dataset and responsible owner for traceability. | Sentinel alerts, Logic App execution reports, incident documentation (24h/72h). |
| **Backup & Recovery (Art.21(2)(e))** | Enable ADLS versioning and soft delete, Delta Lake time travel, and MLflow model versioning with GRS replication. | Conduct quarterly restore tests for Delta tables and ML models to validate RPO/RTO performance. | Restore logs, test reports, validation screenshots. |
| **Supplier Risk (Art.21(2)(d,f))** | Enforce Private Link for Databricks, ADLS, and Event Hub; apply EU-only region policies; PIM/MFA and SCIM sync for identity management. | Approve Azure Container Registry images through security review; maintain SBOM for all dependencies. | Supplier SLA, ACR scan reports, Azure Policy compliance exports. |
| **Data Transfer & Legal (GDPR/NIS2)** | Use Microsoft Purview for lineage and sensitivity labeling; enforce column-level masking via Unity Catalog. | Hash or remove PII at Silver layer; ensure Gold layer aggregates are anonymized and EU-based. | Purview lineage exports, Unity Catalog masking DDLs, GDPR DPA/DTIA documentation. |
| **Risk & Monitoring (Art.21(2)(a,b))** | Leverage Delta Expectations, Job ACLs, and Sentinel analytics for anomaly detection and proactive monitoring. | Use MLflow metrics for model drift tracking and trigger alerts on threshold breaches. | MLflow drift reports, Sentinel incidents, and alert logs. |
| **Access Control (Art.21(2)(c))** | Apply Unity Catalog RBAC, SCIM group sync, and service principal-based authentication to enforce least privilege. | Use separate service accounts for pipelines; conduct periodic access reviews every 6–12 months. | UC GRANT exports, SCIM sync logs, access review approvals. |
| **Change Control (Art.21(2)(g))** | Use Azure DevOps or GitHub Actions for CI/CD; enforce four-eyes approval for production promotion and PR validation. | Ensure all notebook, job, and cluster policy changes are version-controlled with review gates. | Pull request approvals, release notes, and version control audit trails. |

---

### **Pipeline Reference**
**IoT Hub → Event Hub → ADLS (Private Endpoints) → Databricks Bronze → Silver → Gold Zones → MLflow Registry → Power BI/APIs → Sentinel Monitoring & Purview Lineage**

---

**Prepared by:** Thinkwerke – Strategy Meets Security  
**Date:** October 2025
