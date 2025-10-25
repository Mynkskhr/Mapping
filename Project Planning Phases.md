# Thinkwerke Project Blueprint  
## Unified Compliance Implementation Plan for Diehl Metering / Preventio  
### NIS2 Directive · EU AI Act · Cyber Resilience Act · ISO 27001 Alignment  

---

## 1. Regulatory Timelines & ENISA Guidance Overview  

| **Regulation** | **Effective / Transition Dates** | **Compliance Milestones** | **ENISA Reference** |
|----------------|----------------------------------|-----------------------------|----------------------|
| **NIS2 Directive (EU 2022/2555)** | Effective: Oct 2024  <br> Transposition: Oct 2025 | Q1 2025: Gap Analysis  <br> Q2 2025: Control Mapping  <br> Q3 2025: Implementation  <br> Q1 2026: Audit Readiness | ENISA Baseline Security Measures (2023) |
| **EU AI Act (Reg. 2024/1689)** | Enforcement: Aug 2024  <br> Full Application: Aug 2026 | Q2 2025: Risk Register & Classification  <br> Q3 2025: HITL & Governance  <br> Q4 2025: Technical Conformity Docs | ENISA AI Security Framework (2024) |
| **Cyber Resilience Act (CRA)** | Enforcement: 2025  <br> Full compliance: 2027 | 2025: Secure SDLC controls  <br> 2026: CRA pre-audit  <br> 2027: Declaration of Conformity | ENISA IoT & CRA Implementation Guide |
| **ISO/IEC 27001:2022 Alignment** | Continuous | Align through ISMS lifecycle — overlapping 80% with NIS2 & CRA | ENISA ISMS Maturity Model (2024) |

---

## 2. Thinkwerke CIR³ Framework  
### *Continuous Intelligence · Integration · Resilience*

| **Phase** | **Objective** | **Core Activities** | **Deliverables** |
|------------|----------------|---------------------|------------------|
| **Phase 1 – Continuous Intelligence** | Establish real-time visibility into assets, risk, and data pipelines. | - Map infrastructure (Azure + Databricks) <br> - Integrate Sentinel, Purview, and Defender <br> - Create asset inventory baseline | - ENISA-aligned CMDB <br> - Asset register with risk ownership |
| **Phase 2 – Continuous Integration** | Align NIS2, AI Act, and CRA into one implementation track. | - Define NIS2 technical/organizational controls <br> - Build AI governance (HITL, model risk, explainability) <br> - Embed CRA conformity in CI/CD | - Unified compliance matrix <br> - AI conformity technical file (Annex IV) |
| **Phase 3 – Continuous Resilience** | Establish continuous improvement and response framework. | - Implement post-market monitoring <br> - Conduct restoration drills and model drift audits <br> - Create unified reporting dashboard | - CIR³ dashboard <br> - Audit-ready ENISA/ISO reports |

---

## 3. Technical Implementation Guidance (Databricks on Azure)

| **Control Area** | **Azure / Databricks Implementation** | **ENISA / NIS2 Reference** | **Evidence / Deliverable** |
|------------------|----------------------------------------|-----------------------------|-----------------------------|
| **Asset Management** | Unity Catalog + Azure Resource Graph → ServiceNow CMDB | NIS2 Art. 21(2)(a) | CMDB export, ownership mapping |
| **Vulnerability Management** | Cluster policies, Defender for Cloud, CI/CD security scans | NIS2 Art. 21(2)(d) | Scan logs, policy compliance export |
| **Incident Reporting** | Sentinel + Logic Apps (24h/72h reporting) | NIS2 Art. 23 | Incident logs, ENISA-formatted reports |
| **Backup & Recovery** | ADLS versioning, Delta time travel | NIS2 Art. 21(2)(e) | Restore test documentation |
| **Access Control** | Unity Catalog RBAC, SCIM sync, Entra ID PIM | ISO 27001 A.5.17 | Access review logs |
| **Data Governance** | Purview DLP + Unity Catalog lineage | AI Act Art. 10, GDPR | Data quality report, risk register |
| **Monitoring** | MLflow drift detection + Sentinel alerts | AI Act Art. 15 | Model drift metrics, alert dashboard |
| **Supplier Risk** | SBOM tracking + ACR image validation | CRA Annex II | Supplier SLA, SBOM archive |

---

## 4. Compliance Maturity Chain  
### From NIS2 → AI Act → CRA → ISO 27001 → Customer Trust

| **Stage** | **Focus Area** | **Dependency / Outcome** |
|------------|----------------|---------------------------|
| **NIS2 Directive** | Secure organizational and technical foundation for essential entities. | Builds base security posture for AI and product compliance. |
| **EU AI Act** | Risk-based governance for AI transparency, bias control, and HITL oversight. | Depends on NIS2’s established security maturity. |
| **Cyber Resilience Act** | Product security, vulnerability disclosure, and software assurance. | Builds upon NIS2 (governance) and AI Act (technical controls). |
| **ISO 27001** | ISMS unifying all regulatory controls and continuous improvement. | Converts compliance into operational maturity. |
| **Customer Trust** | Demonstrable transparency, traceability, and EU readiness. | Achieved through unified compliance evidence. |

> ⚡ **Critical Insight:** Each regulation strengthens the previous one. Missing one weakens the entire chain.  
> Unified governance through the **CIR³ Framework** builds resilience, trust, and long-term EU market readiness.

---

## 5. ENISA Compliance Mind Map — Utilities / Critical Infrastructure

| **Domain** | **ENISA Control Category** | **Focus Area / Objective** | **Utility-Specific Implementation (Azure / Databricks)** | **Linked Regulation / Article** |
|-------------|----------------------------|-----------------------------|-----------------------------------------------------------|----------------------------------|
| **Governance & Accountability** | Policy & Risk Management | Define risk ownership and board accountability. | NIS2 risk owner mapping via Azure AD & ServiceNow. | NIS2 Art. 21(1), ISO A.5 |
| **Asset & Configuration** | Asset Identification | Maintain updated CMDB of all assets. | Azure Resource Graph + Unity Catalog. | NIS2 Art. 21(2)(a) |
| **Access Control** | Authentication & Authorization | Enforce least privilege and MFA. | Azure AD PIM, SCIM, RBAC. | NIS2 Art. 21(2)(c) |
| **Vulnerability Mgmt** | Patch & Threat Mgmt | Identify and mitigate system vulnerabilities. | Defender for Cloud + CI/CD checks. | CRA Art. 10 |
| **Data & AI Integrity** | AI Governance | Ensure lawful, unbiased, traceable AI models. | Unity Catalog + MLflow lineage. | AI Act Art. 9–15 |
| **Incident Response** | Detection & Notification | Detect and report within 24h/72h. | Sentinel + Logic Apps. | NIS2 Art. 23 |
| **Supply Chain** | Third-Party Risk | Assess vendors and dependencies. | ACR + SBOM + policy automation. | CRA Annex II |
| **Resilience** | Backup & Recovery | Ensure tested restoration and failover. | ADLS versioning + Delta Time Travel. | NIS2 Art. 21(2)(e) |
| **Continuous Improvement** | Metrics & Audit | Assess maturity and improvement. | Grafana + CIR³ dashboards. | ENISA Maturity Model |

---

## 6. AI Act Compliance Checklist (Databricks on Azure – Water Leak Detection)

| **AI Act Requirement** | **Implementation on Databricks (Azure)** | **Evidence / Deliverables** | **Linked Articles / Annexes** |
|-------------------------|-------------------------------------------|------------------------------|-------------------------------|
| **AI System Classification** | Identify water leak detection as *High-Risk AI*; document under Annex III. | AI System Register. | Art. 6–7, Annex III |
| **Risk Management Framework** | AI Risk Register (Delta table) integrated with Purview. | Risk Register & CI/CD logs. | Art. 9 |
| **Data Governance & Quality** | Unity Catalog lineage, bias detection, and validation notebooks. | Data Quality Report. | Art. 10 |
| **HITL Oversight** | Define human approval in Databricks workflow; Logic Apps validation. | HITL Policy & Logs. | Art. 14 |
| **Explainability & Transparency** | SHAP/LIME explainability in notebooks + Power BI reporting. | Explainability Report. | Art. 13 |
| **Accuracy & Robustness** | MLflow drift detection + Sentinel monitoring. | Model Drift Report. | Art. 15 |
| **Record-Keeping** | Log metadata & inference details to ADLS + MLflow. | Audit Logs. | Art. 12 |
| **Conformity Assessment** | Validate compliance vs ENISA & ISO 42001 baselines. | Conformity File (Annex IV). | Art. 43 |
| **Post-Market Monitoring** | CIR³ dashboards + Sentinel alerts for continuous review. | Monitoring Report. | Art. 61 |
| **Incident Reporting** | Logic Apps auto-notification pipeline for EU authority alerts. | Incident Template. | Art. 62 |

---

## 7. Deliverables Summary

| **Deliverable** | **Purpose / Outcome** |
|-----------------|------------------------|
| NIS2 Compliance Matrix | Map controls, owners, and evidence for regulatory reporting. |
| AI Act Technical File | Document AI lifecycle, HITL oversight, and risk controls. |
| CRA Declaration of Conformity | Ensure product-level resilience certification. |
| ISO 27001 Readiness Pack | Merge controls for unified ISMS structure. |
| CIR³ Dashboard | Unified compliance and risk visualization for executives. |
| ENISA Quarterly Report | Standardized EU-style compliance summary. |

---

## 8. Closing Message
> Through this plan, **Thinkwerke** enables **Diehl Metering / Preventio** to move beyond compliance into sustainable governance.  
>  
> With the **CIR³ Framework**, all EU regulations — **NIS2**, **AI Act**, and **CRA** — align with **ISO 27001**, creating a secure, explainable, and resilient foundation for AI-powered utilities operations.

---

**Prepared by:** Thinkwerke – Strategy Meets Security  
**Lead Consultant:** Mayank Sekhar, CISM · ISO 27001 LI · AWS SA Pro · CompTIA SecurityX Architect · NIS2 Directive and DORA Trained Professional 
**Date:** October 2025  
