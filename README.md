# AI Prompt Ladders

Tiered system prompts that work on any LLM and chain from novice to expert, with human approval gates at every step.

- **48 prompts** in three collections: an IT Pro ladder (20), a Strategic Ops ladder (20) and a Strategy Consulting pipeline (8).
- **Model-agnostic.** Plain Markdown system prompts. No tools, plugins or special syntax required.
- **Self-contained.** Each prompt carries its own gates, safety rules and style rules inline, so it works when pasted alone.
- **Chained.** Each prompt knows when to hand off to the next level or stage, and produces a handoff packet the next prompt reads first.
- **Human in the loop.** Every prompt stops three times for an explicit APPROVE, REVISE or STOP.

## How to use a prompt

1. **Pick a prompt** from the matrices below. Start at the level that matches the person doing the work, not the size of the problem.
2. **Copy the file.** Everything below the front matter (the block between the `---` lines) is the prompt. The front matter lists the inputs, level and frameworks for reference.
3. **Fill the `{{PLACEHOLDERS}}`.** Replace each one with your input. `{{USER_NAME}}` is the person the assistant works for. Any placeholder you leave unfilled is treated as a missing input, and the assistant asks for it at Gate 1.
4. **Paste it as the system prompt** (or custom instructions, or the first message if your tool has no system prompt field).
5. **Answer each gate.** The assistant stops three times:
   - **Gate 1, Start:** it restates the task, lists inputs and assumptions, and asks up to three questions.
   - **Gate 2, Middle:** it shows a preview (a plan, outline, diff or table) before producing anything final or changing anything.
   - **Gate 3, End:** it presents a draft marked **DRAFT: requires human sign-off**, with a pass/fail self-check and open risks.

   Reply **APPROVE**, **REVISE** (with what to change) or **STOP**. Silence or "looks fine so far" is not approval. Irreversible actions (sending, publishing, deleting, purchasing) always need their own explicit approval.

Optional: load [`shared/human-gates.md`](shared/human-gates.md) and [`shared/style-rules.md`](shared/style-rules.md) alongside a prompt. They are the canonical versions of the inline rules and win where they differ.

## IT Pro ladder

Five IT task families, each climbing from an everyday user (L1) to a power user (L2), an IT professional (L3) and an expert (L4). [Collection README](it-pro/README.md).

| Family | L1 Everyday User | L2 Power User | L3 IT Professional | L4 Expert |
|---|---|---|---|---|
| Automation and scripting | [Command and Script Explainer](it-pro/automation-scripting/L1-command-explainer.md) | [Scripting Partner for Power Users](it-pro/automation-scripting/L2-scripting-partner.md) | [Sysadmin Automation and Change Engineer](it-pro/automation-scripting/L3-sysadmin-automation-engineer.md) | [Automation and AI Agent Governance Reviewer](it-pro/automation-scripting/L4-automation-ai-agent-governance.md) |
| Data, backup and recovery | [Personal Backup and Restore Helper](it-pro/data-backup-recovery/L1-personal-backup-helper.md) | [Home Lab and Small Office Backup Planner](it-pro/data-backup-recovery/L2-small-office-backup-planner.md) | [Backup and Recovery Operations Engineer](it-pro/data-backup-recovery/L3-backup-recovery-operations.md) | [Resilience and Business Continuity Architect](it-pro/data-backup-recovery/L4-resilience-continuity-architect.md) |
| Risk, governance and audit | [App and Online Service Safety Check](it-pro/risk-governance-audit/L1-app-service-safety-check.md) | [Small Business IT Policy and Vendor Risk Starter](it-pro/risk-governance-audit/L2-small-business-policy-vendor-starter.md) | [GRC Control Mapping and Evidence Analyst](it-pro/risk-governance-audit/L3-grc-control-mapping-evidence.md) | [IT Audit Findings and Risk Quantification Lead](it-pro/risk-governance-audit/L4-it-audit-risk-quantification.md) |
| Security, accounts and access | [Account and Password Security Coach](it-pro/security-access/L1-account-security-coach.md) | [Home and Small Office Security Hardening Advisor](it-pro/security-access/L2-home-office-hardening.md) | [SOC Alert Triage and SIEM Query Analyst](it-pro/security-access/L3-soc-alert-triage.md) | [Incident Response Commander](it-pro/security-access/L4-incident-response-commander.md) |
| Troubleshooting and support | [Everyday Device Fix Guide](it-pro/troubleshooting-support/L1-device-fix-guide.md) | [Home Lab and Small Office Troubleshooter](it-pro/troubleshooting-support/L2-home-office-network-troubleshooter.md) | [Service Desk Triage and Diagnostics Analyst](it-pro/troubleshooting-support/L3-service-desk-triage.md) | [Major Incident and Problem Management Lead](it-pro/troubleshooting-support/L4-major-incident-problem-lead.md) |

## Strategic Ops ladder

Five strategy and operations families, each climbing from a new or first-line manager (L1) to an operations manager (L2), a strategic operations director (L3) and a COO or chief strategist (L4). [Collection README](strategic-ops/README.md).

| Family | L1 New or First-Line Manager | L2 Operations Manager | L3 Strategic Operations Director | L4 COO or Chief Strategist |
|---|---|---|---|---|
| Competitive dynamics and game theory | [Rival Move Read and Response Brief](strategic-ops/competitive-dynamics-game-theory/L1-rival-move-read.md) | [Competitive Response Payoff Modeler](strategic-ops/competitive-dynamics-game-theory/L2-competitive-response-payoff-modeler.md) | [Repeated-Game and Signaling Strategist](strategic-ops/competitive-dynamics-game-theory/L3-repeated-game-signaling-strategist.md) | [Strategic Game Architect](strategic-ops/competitive-dynamics-game-theory/L4-strategic-game-architect.md) |
| Decision quality and risk | [Decision Check and Decision Journal Coach](strategic-ops/decision-quality-risk/L1-decision-check.md) | [Decision Tree and Pre-Mortem Analyst](strategic-ops/decision-quality-risk/L2-decision-tree-premortem.md) | [Forecasting and Real Options Analyst](strategic-ops/decision-quality-risk/L3-forecasting-real-options-analyst.md) | [Tail Risk and Decision System Architect](strategic-ops/decision-quality-risk/L4-tail-risk-decision-system-architect.md) |
| Execution and resource allocation | [Team Bottleneck and Weekly Cadence Coach](strategic-ops/execution-resource-allocation/L1-team-bottleneck-cadence-coach.md) | [Throughput and Capacity Planner](strategic-ops/execution-resource-allocation/L2-throughput-capacity-planner.md) | [Initiative Portfolio and OKR Alignment Director](strategic-ops/execution-resource-allocation/L3-initiative-portfolio-okr-director.md) | [Capital Allocation and Incentive System Architect](strategic-ops/execution-resource-allocation/L4-capital-allocation-incentive-architect.md) |
| Negotiation and bargaining | [Negotiation Prep Sheet Builder](strategic-ops/negotiation-bargaining/L1-negotiation-prep-sheet.md) | [Multi-Issue Supplier Deal Designer](strategic-ops/negotiation-bargaining/L2-multi-issue-deal-designer.md) | [Strategic Sourcing and Auction Designer](strategic-ops/negotiation-bargaining/L3-strategic-sourcing-auction-designer.md) | [Multi-Party Negotiation and Coalition Architect](strategic-ops/negotiation-bargaining/L4-multi-party-coalition-architect.md) |
| Strategy formulation and scenarios | [Strategy-to-Team Translator and Local OODA Loop](strategic-ops/strategy-formulation-scenarios/L1-strategy-to-team-translator.md) | [Five Forces and Strategy Kernel Builder](strategic-ops/strategy-formulation-scenarios/L2-five-forces-kernel-builder.md) | [Scenario Planning and Wargame Director](strategic-ops/strategy-formulation-scenarios/L3-scenario-wargame-director.md) | [Playing to Win Cascade and Strategic Choice Architect](strategic-ops/strategy-formulation-scenarios/L4-strategic-choice-cascade-architect.md) |

## Strategy Consulting pipeline

Eight stages of an opportunity assessment for a new small-business venture or product line, run in order, each handing a packet to the next. [Collection README](strategy-consulting/README.md).

| Stage | Prompt | Hands off to |
|---|---|---|
| 1 | [Customer Jobs-to-be-Done Research Designer](strategy-consulting/01-customer-jobs-research.md) | [Competitor and Market Structure Analyst](strategy-consulting/02-competitor-market-structure.md) |
| 2 | [Competitor and Market Structure Analyst](strategy-consulting/02-competitor-market-structure.md) | [Blue Ocean Strategy Designer](strategy-consulting/03-blue-ocean-designer.md) |
| 3 | [Blue Ocean Strategy Designer](strategy-consulting/03-blue-ocean-designer.md) | [Lean Assumption Testing Designer](strategy-consulting/04-lean-assumption-testing.md) |
| 4 | [Lean Assumption Testing Designer](strategy-consulting/04-lean-assumption-testing.md) | [Business Model and Unit Economics Analyst](strategy-consulting/05-business-model-unit-economics.md) |
| 5 | [Business Model and Unit Economics Analyst](strategy-consulting/05-business-model-unit-economics.md) | [Framework Selection and Evidence Challenger](strategy-consulting/06-framework-selection-challenger.md) |
| 6 | [Framework Selection and Evidence Challenger](strategy-consulting/06-framework-selection-challenger.md) | [Opportunity Assessment and Recommendation Writer](strategy-consulting/07-opportunity-recommendation-writer.md) |
| 7 | [Opportunity Assessment and Recommendation Writer](strategy-consulting/07-opportunity-recommendation-writer.md) | [Independent Strategy Engagement Operator](strategy-consulting/08-independent-engagement-operator.md) |
| 8 | [Independent Strategy Engagement Operator](strategy-consulting/08-independent-engagement-operator.md) | The consultant and venture owner (end of pipeline) |

## How the handoffs work

- **Ladders (IT Pro, Strategic Ops).** Each prompt has an escalate-up rule naming the next level and the conditions that trigger it, such as scope, risk or skill beyond the audience it was written for. When a condition is met, the assistant says so in one line and produces a handoff packet with personal data and secrets removed. Paste the packet into the next level's prompt. The receiving prompt reads it at Gate 1 and does not repeat questions or diagnostics the packet already answers. L4 prompts hand off to human decision-makers.
- **Pipeline (Strategy Consulting).** Stages run in order, 1 to 8. Each stage hands off when Gate 3 is approved or its timebox ends, passing what exists with gaps and weak evidence marked. If evidence points to stopping or a major pivot, the prompt says so before the next stage starts, and the people involved decide whether to continue. Several stages point to related Strategic Ops prompts for deeper work on the same method.
- **Gates still apply.** A handoff never skips a gate. The next prompt starts again at Gate 1.

## Repository layout

```
it-pro/<family>/L1-L4 *.md      IT Pro ladder (5 families x 4 levels)
strategic-ops/<family>/L1-L4 *.md   Strategic Ops ladder (5 families x 4 levels)
strategy-consulting/01-08 *.md  Strategy Consulting pipeline (8 stages)
shared/human-gates.md           Canonical human-gate block
shared/style-rules.md           Canonical style rules
```

## Front matter fields

`title`, `version`, `family`, `level` (or `stage`), `tier`, `audience`, `inputs` (the placeholders to fill), `frameworks_referenced`, `escalates_to` or `hands_off_to`, and `purpose`. Strategy Consulting prompts also carry `maps_to_criterion`, the capability each stage exercises.

## Open verification items

The prompts flag uncertain citation details with **[verify]** instead of guessing. These are left in place on purpose. Check them against the original source before you rely on them:

- [Account and Password Security Coach](it-pro/security-access/L1-account-security-coach.md): NIST SP 800-63B, Digital Identity Guidelines: Authentication (general principles only: length over forced complexity, no forced periodic changes without a sign of compromise, screen against known-breached passwords; revision unverified)
- [Decision Check and Decision Journal Coach](strategic-ops/decision-quality-risk/L1-decision-check.md): Jeff Bezos, Amazon shareholder letter (2015): Type 1 and Type 2 decisions [verify year]
- [Tail Risk and Decision System Architect](strategic-ops/decision-quality-risk/L4-tail-risk-decision-system-architect.md): Jeff Bezos, Amazon shareholder letter (2015): Type 1 and Type 2 decisions [verify year]
- [Team Bottleneck and Weekly Cadence Coach](strategic-ops/execution-resource-allocation/L1-team-bottleneck-cadence-coach.md): Commander's intent, from mission command doctrine (US Army ADP 6-0, Mission Command, 2019) [verify edition]
- [Throughput and Capacity Planner](strategic-ops/execution-resource-allocation/L2-throughput-capacity-planner.md): Wallace Hopp and Mark Spearman, Factory Physics (1996; later editions) [verify edition]: variability and utilization effects
- [Initiative Portfolio and OKR Alignment Director](strategic-ops/execution-resource-allocation/L3-initiative-portfolio-okr-director.md): Robert Cooper, Stage-Gate idea-to-launch process (Winning at New Products, 1986 and later editions) [verify edition]
- [Multi-Issue Supplier Deal Designer](strategic-ops/negotiation-bargaining/L2-multi-issue-deal-designer.md): Multiple equivalent simultaneous offers (MESOs), as studied by Geoffrey Leonardelli, Jun Gu and colleagues [verify authorship and year]
- [Multi-Party Negotiation and Coalition Architect](strategic-ops/negotiation-bargaining/L4-multi-party-coalition-architect.md): Bargaining tactics that would breach labor law (for example, a refusal to bargain in good faith where that duty applies) [verify jurisdiction].
- [Strategy-to-Team Translator and Local OODA Loop](strategic-ops/strategy-formulation-scenarios/L1-strategy-to-team-translator.md): John Boyd's OODA loop (observe, orient, decide, act), from his briefings, including 'Patterns of Conflict' and 'The Essence of Winning and Losing' (1995) [verify dates]
- [Scenario Planning and Wargame Director](strategic-ops/strategy-formulation-scenarios/L3-scenario-wargame-director.md): Two-axis scenario matrix, often associated with Global Business Network practice rather than Shell itself [verify attribution]
- [Scenario Planning and Wargame Director](strategic-ops/strategy-formulation-scenarios/L3-scenario-wargame-director.md): UK Ministry of Defence, Red Teaming Handbook, 3rd edition (2021) [verify edition]
- [Scenario Planning and Wargame Director](strategic-ops/strategy-formulation-scenarios/L3-scenario-wargame-director.md): Simon Wardley, Wardley Maps (published openly online, from about 2016) [verify]
- [Playing to Win Cascade and Strategic Choice Architect](strategic-ops/strategy-formulation-scenarios/L4-strategic-choice-cascade-architect.md): Lafley and Martin, Playing to Win (2013), strategy-process chapter: 'what would have to be true' option testing [verify chapter]
- [Playing to Win Cascade and Strategic Choice Architect](strategic-ops/strategy-formulation-scenarios/L4-strategic-choice-cascade-architect.md): Simon Wardley, Wardley Maps: doctrine and gameplay [verify]
- [Customer Jobs-to-be-Done Research Designer](strategy-consulting/01-customer-jobs-research.md): Bob Moesta and Chris Spiek, forces of progress and the switch interview (The Jobs-to-be-Done Handbook, 2014 [verify]); Moesta, Demand-Side Sales 101 (2020)
- [Business Model and Unit Economics Analyst](strategy-consulting/05-business-model-unit-economics.md): Peter van Westendorp, Price Sensitivity Meter (1976) [verify naming of the intersection points]
- [Business Model and Unit Economics Analyst](strategy-consulting/05-business-model-unit-economics.md): Clive Granger and André Gabor, Gabor-Granger pricing method (1960s) [verify]
- [Business Model and Unit Economics Analyst](strategy-consulting/05-business-model-unit-economics.md): Naming of the points varies across sources [verify].
- [Framework Selection and Evidence Challenger](strategy-consulting/06-framework-selection-challenger.md): Barbara Minto, The Pyramid Principle (1987 and later editions) [verify first edition year]: MECE grouping and issue structure
- [Framework Selection and Evidence Challenger](strategy-consulting/06-framework-selection-challenger.md): Lafley and Martin, Playing to Win (2013): 'what would have to be true' [verify chapter]
- [Opportunity Assessment and Recommendation Writer](strategy-consulting/07-opportunity-recommendation-writer.md): Barbara Minto, The Pyramid Principle: SCQA (situation, complication, question, answer) and top-down structure [verify edition]
- [Opportunity Assessment and Recommendation Writer](strategy-consulting/07-opportunity-recommendation-writer.md): GRADE-style evidence grading, adapted from clinical evidence practice [verify]: a qualitative strong, moderate, weak scale
- [Independent Strategy Engagement Operator](strategy-consulting/08-independent-engagement-operator.md): Barbara Minto, The Pyramid Principle [verify edition]

## Disclaimer

These prompts are not legal, financial, tax or security advice, and the output they produce is not either. They are drafting and thinking aids that keep a human in charge of every decision. Verify any framework, standard, citation or figure an assistant cites before you rely on it, and get qualified professional advice where the stakes call for it.

## License

[CC BY 4.0](LICENSE). Copyright (c) 2026 Starboy1968. You may share and adapt these prompts for any purpose, including commercially, with attribution.
