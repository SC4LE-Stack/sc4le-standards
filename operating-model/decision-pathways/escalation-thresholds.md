---
title: Escalation Thresholds
version: 1.0.3
status: canonical
last-updated: 2026-06-08
---

# Escalation Thresholds

## 1. Purpose
Defines when decisions must be escalated from teams → LDAs → CDA. Escalation is exception-based, not routine.

## 2. Escalation Principles
Escalate only when:
- risk exceeds local tolerance
- decisions impact multiple domains
- ethical guardrails are at risk
- regulatory exposure increases
- sensing signals indicate systemic issues

## 3. Escalation Flow (Mermaid)

  ```mermaid
    flowchart LR
        T[Team decision] --> A{Within<br/>local thresholds?}
        A -->|Yes| TOK[Team keeps decision]
        A -->|No| L[LDA review]

        L --> B{Within<br/>domain thresholds?}
        B -->|Yes| LOK[LDA decides]
        B -->|No| C[CDA escalation]

        C --> COK[CDA decides<br/>and updates guardrails]
  ```

## 4. Threshold Table

| Threshold Type   | Team           | LDA              | CDA                    |
|------------------|----------------|------------------|------------------------|
| Reversibility    | reversible     | reversible       | irreversible           |
| Risk             | low            | medium           | high/systemic          |
| Impact           | local          | domain           | enterprise             |
| Ethics           | no concern     | minor concern    | material concern       |
| Regulatory       | none           | moderate         | significant            |
| Dependencies     | isolated       | cross-team       | cross-domain           |
| Flow Impact      | minimal        | moderate         | major/systemic         |

## 5. Anti‑Patterns
- escalating for certainty
- escalating due to fear
- escalating due to unclear principles

## 6. Maturity Indicators
- stable escalation patterns
- fewer unnecessary escalations
- improved decision clarity
