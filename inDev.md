```mermaid

flowchart TD
  A[Customer security query intake\n(form, ticket, email)] --> B{Scope triage}
  B -- App/Code available? --> C[Run SAST\n(e.g., CodeQL/semgrep)]
  B -- Running instance? --> D[Run DAST\n(e.g., ZAP/OWASP)]
  C --> E[Export SAST report\n(SARIF/JSON/HTML)]
  D --> F[Export DAST report\n(JSON/HTML)]
  E --> G[Store raw reports in GitHub\nrepo: /security/reports/]
  F --> G
  G --> H[Collect supporting docs\n(NIS2, ISO 27001, InfoSec\ntheory, product-wise notes)]
  H --> I[Normalize findings\n(CVSS, CWE, asset, owner)]
  I --> J[Generate common report (PDF)\nwith ReportLab]
  J --> K[Publish artefacts\n(GitHub Releases/Pages)]
  K --> L[Notify stakeholders\n(email/Slack/Jira)]
  B -- Out of scope --> X[Clarify scope & re-intake]
  I --> |FP review| R[Analyst validation\n(false positives, dupes)]
  R --> I

```
