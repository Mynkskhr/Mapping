```mermaid


```

┌────────────────────┐   →   ┌───────────────────┐   →   ┌──────────────┐   →   ┌────────────────────┐   →   ┌───────────────────┐   →   ┌──────────────┐
│ Automated Scans     │       │    Detection      │       │    Triage     │       │   Ticket Creation   │       │    Remediation     │       │ Verification  │
│ (SAST / SCA / DAST /│       │ (Vulns, licenses, │       │ (Severity,    │       │ (Auto Jira issue    │       │ (Team assigned,    │       │ (Re-scan &   │
│ IaC / Container /   │       │ secrets, IaC)     │       │ exploitability)│      │ per finding)        │       │ SLA tracking)      │       │ evidence)    │
│ Secrets)            │       │                   │       │               │       │                     │       │                     │       │              │
└────────────────────┘       └───────────────────┘       └──────────────┘       └────────────────────┘       └───────────────────┘       └──────────────┘
                                                                                                                       ↓
                                                                                                               ┌────────────────┐
                                                                                                               │    Closure     │
                                                                                                               │ (Resolved /     │
                                                                                                               │ Escalate)       │
                                                                                                               └────────────────┘

