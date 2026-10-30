# IT Pro ladder

Five IT task families, each climbing from an everyday user (L1) to a power user (L2), an IT professional (L3) and an expert (L4).

Each prompt is a self-contained system prompt. Copy one file, fill its `{{PLACEHOLDERS}}`, and paste it as the system prompt. See the [main README](../README.md) for full instructions.

## Matrix

| Family | L1 Everyday User | L2 Power User | L3 IT Professional | L4 Expert |
|---|---|---|---|---|
| Automation and scripting | [Command and Script Explainer](automation-scripting/L1-command-explainer.md) | [Scripting Partner for Power Users](automation-scripting/L2-scripting-partner.md) | [Sysadmin Automation and Change Engineer](automation-scripting/L3-sysadmin-automation-engineer.md) | [Automation and AI Agent Governance Reviewer](automation-scripting/L4-automation-ai-agent-governance.md) |
| Data, backup and recovery | [Personal Backup and Restore Helper](data-backup-recovery/L1-personal-backup-helper.md) | [Home Lab and Small Office Backup Planner](data-backup-recovery/L2-small-office-backup-planner.md) | [Backup and Recovery Operations Engineer](data-backup-recovery/L3-backup-recovery-operations.md) | [Resilience and Business Continuity Architect](data-backup-recovery/L4-resilience-continuity-architect.md) |
| Risk, governance and audit | [App and Online Service Safety Check](risk-governance-audit/L1-app-service-safety-check.md) | [Small Business IT Policy and Vendor Risk Starter](risk-governance-audit/L2-small-business-policy-vendor-starter.md) | [GRC Control Mapping and Evidence Analyst](risk-governance-audit/L3-grc-control-mapping-evidence.md) | [IT Audit Findings and Risk Quantification Lead](risk-governance-audit/L4-it-audit-risk-quantification.md) |
| Security, accounts and access | [Account and Password Security Coach](security-access/L1-account-security-coach.md) | [Home and Small Office Security Hardening Advisor](security-access/L2-home-office-hardening.md) | [SOC Alert Triage and SIEM Query Analyst](security-access/L3-soc-alert-triage.md) | [Incident Response Commander](security-access/L4-incident-response-commander.md) |
| Troubleshooting and support | [Everyday Device Fix Guide](troubleshooting-support/L1-device-fix-guide.md) | [Home Lab and Small Office Troubleshooter](troubleshooting-support/L2-home-office-network-troubleshooter.md) | [Service Desk Triage and Diagnostics Analyst](troubleshooting-support/L3-service-desk-triage.md) | [Major Incident and Problem Management Lead](troubleshooting-support/L4-major-incident-problem-lead.md) |

## Prompts

### Automation and scripting

- **[Command and Script Explainer](automation-scripting/L1-command-explainer.md)** (L1, Everyday User): Explains, part by part, any command or script someone asked an everyday user to run, rates the risk, and says plainly whether to run it.
- **[Scripting Partner for Power Users](automation-scripting/L2-scripting-partner.md)** (L2, Power User): Writes and explains small PowerShell or Bash scripts for personal and home-lab tasks, with a dry-run default, a test on copies, and every line explained.
- **[Sysadmin Automation and Change Engineer](automation-scripting/L3-sysadmin-automation-engineer.md)** (L3, IT Professional): Builds production-grade admin automation for an organization (idempotent, logged, least-privilege, reviewed) and drafts the change request that gets it approved.
- **[Automation and AI Agent Governance Reviewer](automation-scripting/L4-automation-ai-agent-governance.md)** (L4, Expert): Reviews automation and AI agent deployments before go-live (permission scope, human approval points, data exposure, prompt injection and tool misuse, logging, rollback and vendor terms), aligned to NIST AI RMF 1.0 and the OWASP Top 10 for LLM Applications 2025.

### Data, backup and recovery

- **[Personal Backup and Restore Helper](data-backup-recovery/L1-personal-backup-helper.md)** (L1, Everyday User): Gets an everyday user's photos, documents and phone data backed up in at least two places, and proves the backup works by restoring one file.
- **[Home Lab and Small Office Backup Planner](data-backup-recovery/L2-small-office-backup-planner.md)** (L2, Power User): Designs, documents and tests a backup plan for a home lab or small office: what to protect, how often, where copies live, encryption, an offline or immutable copy, and scheduled restore tests.
- **[Backup and Recovery Operations Engineer](data-backup-recovery/L3-backup-recovery-operations.md)** (L3, IT Professional): Runs backup operations for an organization: job-failure triage, authorized restore requests, scheduled restore testing with RPO and RTO evidence, and DR runbooks, aligned to NIST SP 800-34 Rev. 1.
- **[Resilience and Business Continuity Architect](data-backup-recovery/L4-resilience-continuity-architect.md)** (L4, Expert): Sets recovery strategy for the business: business impact analysis, tiered RTO and RPO, ransomware-resilient backup architecture, DR exercise design and leadership reporting, aligned to ISO 22301:2019, NIST SP 800-34 Rev. 1 and CSF 2.0.

### Risk, governance and audit

- **[App and Online Service Safety Check](risk-governance-audit/L1-app-service-safety-check.md)** (L1, Everyday User): Helps an everyday user decide whether an app, browser extension, website or online service is safe to install or sign up for, by reading its permissions, data practices and red flags.
- **[Small Business IT Policy and Vendor Risk Starter](risk-governance-audit/L2-small-business-policy-vendor-starter.md)** (L2, Power User): Gives a small business its first short, usable IT policies and a vendor risk check for its key providers, scaled to CIS Controls v8.1 IG1 and the NIST CSF 2.0 Govern function.
- **[GRC Control Mapping and Evidence Analyst](risk-governance-audit/L3-grc-control-mapping-evidence.md)** (L3, IT Professional): Maps policies and controls to NIST CSF 2.0, NIST SP 800-53 Rev. 5 and CIS Controls v8.1, builds evidence request lists, and tests evidence for exceptions, including third-party and supply chain controls.
- **[IT Audit Findings and Risk Quantification Lead](risk-governance-audit/L4-it-audit-risk-quantification.md)** (L4, Expert): Reviews audit evidence to ISACA ITAF standards, writes findings as criteria, condition, cause, effect and recommendation, and turns top risks into ranged, assumption-labeled loss estimates for leadership.

### Security, accounts and access

- **[Account and Password Security Coach](security-access/L1-account-security-coach.md)** (L1, Everyday User): Helps an everyday user lock down their own accounts: password manager, unique passwords, MFA or passkeys, recovery options, phishing checks, and what to do after a suspected hack.
- **[Home and Small Office Security Hardening Advisor](security-access/L2-home-office-hardening.md)** (L2, Power User): Builds and walks through a prioritized hardening plan for a home lab or small office: inventory, updates, admin rights, router and Wi-Fi, encryption, MFA and logging, measured against CIS Controls v8.1 Implementation Group 1.
- **[SOC Alert Triage and SIEM Query Analyst](security-access/L3-soc-alert-triage.md)** (L3, IT Professional): Triages security alerts to a verdict, maps activity to MITRE ATT&CK, writes read-only SIEM queries to scope it, and escalates true positives with a clean evidence packet.
- **[Incident Response Commander](security-access/L4-incident-response-commander.md)** (L4, Expert): Leads a confirmed security incident from scoping to recovery and lessons learned, aligned to NIST SP 800-61 Rev. 3 and CSF 2.0, with evidence preservation, a decision log, and notification questions routed to counsel.

### Troubleshooting and support

- **[Everyday Device Fix Guide](troubleshooting-support/L1-device-fix-guide.md)** (L1, Everyday User): Walks a non-technical person through fixing a problem on their own phone, computer, printer, home Wi-Fi or app, one safe, explained step at a time.
- **[Home Lab and Small Office Troubleshooter](troubleshooting-support/L2-home-office-network-troubleshooter.md)** (L2, Power User): Diagnoses device, network and service problems in a home lab or small office layer by layer, read-only commands first, explaining each command once.
- **[Service Desk Triage and Diagnostics Analyst](troubleshooting-support/L3-service-desk-triage.md)** (L3, IT Professional): Triages organization tickets: classifies, prioritizes by impact and urgency, runs read-only diagnostics on Windows and Linux, resolves within permissions or escalates cleanly, and writes the ticket notes.
- **[Major Incident and Problem Management Lead](troubleshooting-support/L4-major-incident-problem-lead.md)** (L4, Expert): Coordinates major outages and the root-cause work after: roles, status cadence, a decision log, a blameless post-incident review, and problem records that prevent recurrence.

## How the levels connect

Each prompt has an escalation rule. When the work outgrows its level (for example, the scope, risk or skill needed goes beyond the audience it was written for), it says so in one line and produces a handoff packet with personal data and secrets removed. Paste that packet into the next level's prompt; that prompt reads it at Gate 1 and does not repeat what the packet already answers. The L4 prompts hand off to human decision-makers.
