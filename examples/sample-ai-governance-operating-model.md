# AI Governance Operating Model

This example is generic and illustrative. It does not describe a real organization.

## 1. Operating Model Summary

| Field | Value |
|---|---|
| Organization / team | Example Enterprise AI Office |
| Scope | Enterprise AI portfolio |
| Effective date | 2026-04-26 |
| Owner | Example AI Governance Lead |
| Review cadence | Quarterly |
| Primary frameworks referenced | NIST AI RMF, ISO 42001, internal AI policy |

## 2. Governance Principles

- **Accountability:** every AI system must have a named business owner and technical owner.
- **Traceability:** release decisions must be linked to intake, risk assessment, validation evidence, and monitoring plans.
- **Risk proportionality:** controls scale by risk tier, with high-risk systems requiring formal sign-off and stronger oversight.
- **Human oversight:** human review is mandatory for high-risk decisions, sensitive-user impacts, and unresolved model uncertainty.
- **Continuous improvement:** incidents, drift findings, and post-release reviews feed back into governance templates and release gates.

## 3. Scope of AI Systems

### In scope

- internal AI assistants used by employees
- customer-facing AI features
- AI-enabled routing, summarization, classification, or recommendation systems
- vendor-provided AI embedded into business workflows

### Out of scope

- ordinary rules-based automation without model behavior
- personal experimentation not connected to business data or production workflows

### System inventory expectations

Every AI system must record:

- named business owner
- named technical owner
- use-case description
- risk tier
- release status
- model or vendor dependency
- monitoring owner
- next review date

## 4. Governance Forums and Decision Rights

| Forum / role | Decision rights | Inputs required | Outputs |
|---|---|---|---|
| AI Intake Forum | accept, reject, request more information | intake form, owner, use-case summary | triage decision |
| Prioritization Forum | rank, defer, escalate | impact score, risk score, effort estimate | prioritized AI portfolio |
| Release Gate Review | approve, conditional, hold, reject | validation evidence, risk assessment, release plan | release decision and conditions |
| Monitoring Review | continue, adjust, rollback, retire | metrics, incident log, drift report | improvement actions |

## 5. Lifecycle Controls

| Stage | Minimum controls | Required artifacts |
|---|---|---|
| Intake | use-case definition, ownership, preliminary risk screen | intake form |
| Prioritization | value, risk, feasibility, dependency scoring | prioritization matrix |
| Delivery governance | milestone reviews, risk tracking, data governance | project RAID, model card draft |
| Release readiness | validation, legal/compliance review, monitoring readiness | release gate review, checklist report |
| Post-release monitoring | performance, drift, incidents, user feedback | dashboard, incident log |
| Improvement / retirement | periodic review, remediation, decommissioning decision | improvement review or retirement note |

## 6. Risk Tiering

| Tier | Definition | Example controls |
|---|---|---|
| Low | limited impact, internal use, reversible | technical review, basic monitoring |
| Medium | customer-facing or operationally significant | governance review, model card, rollback plan |
| High | regulated, safety-adjacent, hard to reverse, or high-impact | legal review, human oversight, red-team testing, formal sign-off |

## 7. Metrics and CTQs

| Metric | Purpose | Owner | Review cadence |
|---|---|---|---|
| AI system inventory completeness | confirms traceability | AI Governance Lead | monthly |
| release gate pass rate | tracks release quality | Release Manager | quarterly |
| incident recurrence rate | tracks control effectiveness | Operations Owner | monthly |
| open high-risk actions | tracks unresolved exposure | Risk Owner | weekly |
| time from intake to decision | tracks governance flow efficiency | Portfolio Lead | monthly |

## 8. Escalation Rules

Escalate when:

- high-risk system lacks named owner
- release evidence is missing at a required gate
- a severity-1 or severity-2 AI incident occurs
- model behavior materially deviates from validated behavior
- privacy, legal, or safety concerns are unresolved

## 9. Continuous Improvement Loop

At each quarterly review, capture:

- which gate criteria were unclear or excessive
- which evidence was repeatedly missing
- which incidents indicate weak controls
- which templates should be standardized or simplified
- which systems should be re-tiered, remediated, or retired

## 10. Open Decisions

| Decision | Owner | Due date | Status |
|---|---|---|---|
| Define escalation threshold for high-risk model drift | Risk Owner | 2026-05-15 | open |
| Select standard model-card format | AI Governance Lead | 2026-05-30 | open |
| Confirm quarterly monitoring review calendar | Portfolio Lead | 2026-05-10 | open |
