```mermaid

flowchart TB
    A[Automated Scans<br>SAST, SCA/SBOM, DAST, IaC, Container, Secrets]
    B[Detection<br>Vulnerabilities & license issues]
    C[Triage<br>Severity, exploitability, business impact]
    D[Ticket Creation<br>Auto Jira issue per finding]
    E[Remediation<br>Team assigned + SLA tracking]
    F[Verification<br>Re-scan / Code review / Evidence]
    G[Closure<br>Resolved → Ticket closed]
    H[Not Resolved<br>Escalation or remain open]

    A --> B --> C --> D --> E --> F
    F --> G
    F --> H


```

```mermaid

flowchart LR

    A[Automated Scans<br>SAST, SCA/SBOM, DAST, IaC, Container, Secrets]
    B[Detection<br>Vulnerabilities & license issues]
    C[Triage<br>Severity & exploitability]
    D[Remediation<br>Developer fix + SLA tracking]
    E[Verification<br>Re-scan / Code Review]
    F[Closure<br>Resolved → Ticket Closed]
    G[Escalation<br>Critical/High unresolved]

    A --> B --> C --> D --> E --> F
    E --> G


```

```mermaid

flowchart TB

%% ==========================
%% TOP: SSLM CHECKS (HORIZONTAL)
%% ==========================

subgraph SSLM [Secure Software Lifecycle Management (SSLM)]
direction LR

    A1[Code Commit]

    subgraph CHECKS [Automated Checks]
    direction LR
        B1[SAST<br>Static Code Analysis]
        B2[SCA & SBOM<br>Open-Source Components]
        B3[API Security Testing<br>REST / IoT APIs]
        B4[DAST<br>Runtime / Web Testing]
        B5[IaC Scanning<br>Cloud & Infra as Code]
        B6[Container Scanning]
        B7[Secrets Detection]
    end

    A1 --> B1
    A1 --> B2
    A1 --> B3
    A1 --> B4
    A1 --> B5
    A1 --> B6
    A1 --> B7
end

%% ==========================
%% MIDDLE: VULNERABILITY WORKFLOW (HORIZONTAL)
%% ==========================

subgraph WORKFLOW [Operational Vulnerability Workflow]
direction LR
    C1[Detection<br>Findings from SSLM]
    C2[Triage<br>Severity & Business Impact]
    C3[Jira Ticket Automation<br>Owner + SLA]
    C4[Remediation<br>Team Fix]
    C5[Security Champion Review<br>High/C]()


```
