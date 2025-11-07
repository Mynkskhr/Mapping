```mermaid

flowchart TD
  A[Customer security query intake<br/>(form, ticket, email)] --> B{Scope triage}
  B -- App/Code available? --> C[Run SAST<br/>(CodeQL/Semgrep)]
  B -- Running instance? --> D[Run DAST<br/>(OWASP ZAP)]
  C --> E[Export SAST report<br/>(SARIF/JSON/HTML)]
  D --> F[Export DAST report<br/>(JSON/HTML)]
  E --> G[Store raw reports in GitHub<br/>/security/reports/]
  F --> G
  G --> H[Collect supporting docs<br/>(NIS2, ISO 27001, InfoSec,<br/>product-wise notes)]
  H --> I[Normalize findings<br/>(CVSS/CWE/asset/owner)]
  I --> R[Analyst validation<br/>(FP/duplicates review)]
  R --> I
  I --> J[Generate common report (PDF)<br/>with ReportLab]
  J --> K[Publish artifacts<br/>(Releases/Pages)]
  K --> L[Notify stakeholders<br/>(email/Slack/Jira)]
  B -- Out of scope --> X[Clarify scope & re-intake]


```
