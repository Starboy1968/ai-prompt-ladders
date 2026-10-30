# Strategy Consulting pipeline

Eight stages of an opportunity assessment for a new small-business venture or product line, run in order, each handing a packet to the next.

Each prompt is a self-contained system prompt. Copy one file, fill its `{{PLACEHOLDERS}}`, and paste it as the system prompt. See the [main README](../README.md) for full instructions.

## Matrix

| Stage | Prompt | Hands off to |
|---|---|---|
| 1 | [Customer Jobs-to-be-Done Research Designer](01-customer-jobs-research.md) | [Competitor and Market Structure Analyst](02-competitor-market-structure.md) |
| 2 | [Competitor and Market Structure Analyst](02-competitor-market-structure.md) | [Blue Ocean Strategy Designer](03-blue-ocean-designer.md) |
| 3 | [Blue Ocean Strategy Designer](03-blue-ocean-designer.md) | [Lean Assumption Testing Designer](04-lean-assumption-testing.md) |
| 4 | [Lean Assumption Testing Designer](04-lean-assumption-testing.md) | [Business Model and Unit Economics Analyst](05-business-model-unit-economics.md) |
| 5 | [Business Model and Unit Economics Analyst](05-business-model-unit-economics.md) | [Framework Selection and Evidence Challenger](06-framework-selection-challenger.md) |
| 6 | [Framework Selection and Evidence Challenger](06-framework-selection-challenger.md) | [Opportunity Assessment and Recommendation Writer](07-opportunity-recommendation-writer.md) |
| 7 | [Opportunity Assessment and Recommendation Writer](07-opportunity-recommendation-writer.md) | [Independent Strategy Engagement Operator](08-independent-engagement-operator.md) |
| 8 | [Independent Strategy Engagement Operator](08-independent-engagement-operator.md) | The consultant and venture owner (end of pipeline) |

## Prompts

- **[Customer Jobs-to-be-Done Research Designer](01-customer-jobs-research.md)** (stage 1): Designs and analyzes customer research for {{VENTURE}} with Jobs-to-be-Done: who is hiring what for which job, the forces that cause switching, need statements in measurable form, and segments defined by job rather than demographics.
- **[Competitor and Market Structure Analyst](02-competitor-market-structure.md)** (stage 2): Analyzes the structure of {{VENTURE}}'s market with Porter's five forces, scans local competitors and substitutes against the customer jobs from stage 1, and finds the gaps where important needs are underserved and the structure allows a new entrant to earn a return.
- **[Blue Ocean Strategy Designer](03-blue-ocean-designer.md)** (stage 3): Uses Blue Ocean Strategy tools to design a value curve for {{VENTURE}} that breaks the tradeoff between differentiation and low cost: the strategy canvas of the local market, the four-actions ERRC grid, the six paths and the three tiers of noncustomers.
- **[Lean Assumption Testing Designer](04-lean-assumption-testing.md)** (stage 4): Turns the venture's riskiest assumptions into testable hypotheses, designs the cheapest experiment or minimum viable product for each, sets pass and fail thresholds before running, and runs build-measure-learn cycles that end in persevere, pivot or stop calls.
- **[Business Model and Unit Economics Analyst](05-business-model-unit-economics.md)** (stage 5): Builds the Business Model Canvas for {{VENTURE}}, computes unit economics and break-even from sourced inputs, tests pricing with willingness-to-pay methods such as Van Westendorp and Gabor-Granger, and produces a feasibility verdict with the conditions it depends on.
- **[Framework Selection and Evidence Challenger](06-framework-selection-challenger.md)** (stage 6): Chooses which frameworks the engagement needs for the question at hand, then challenges the work so far: does each conclusion rest on evidence, which assumptions fail under scrutiny, and which alternative directions were not considered.
- **[Opportunity Assessment and Recommendation Writer](07-opportunity-recommendation-writer.md)** (stage 7): Writes the engagement's main deliverable: a concise opportunity assessment for {{OWNER}} with one recommended direction, the evidence behind it graded by strength, the key assumptions still open, and concrete next steps with owners and dates.
- **[Independent Strategy Engagement Operator](08-independent-engagement-operator.md)** (stage 8): Runs a 6-to-8-week part-time strategy engagement for {{OWNER}}: scope and statement of work, stage plan using the pipeline, weekly cadence with the owner and specialist advisors, decision log, written status updates and the client-ready standard for every deliverable.

## How the stages connect

Run the stages in order. At the end of each stage, after Gate 3 is approved (or the stage timebox ends), the prompt produces a handoff packet. Paste that packet into the next stage at Gate 1; the next prompt reads it first and does not re-ask what it already answers. If the evidence points to stop or a major pivot, the prompt says so before the next stage starts, and the consultant and owner decide whether to continue.

Several stages list related Strategic Ops prompts for deeper work on the same method.
