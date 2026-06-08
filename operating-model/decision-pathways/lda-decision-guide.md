---
title: LDA Decision Guide
version: 1.0.3
status: canonical
last-updated: 2026-06-08
---

# LDA Decision Guide

## 1. Purpose
Provides LDAs with a structured approach to making contextual, principle-driven decisions that maintain flow and alignment.

## 2. LDA Decision Pattern (Mermaid)

  ```mermaid
    flowchart TD
        A[Decision presented to LDA] --> B[Interpret SC4LE principles in context]
        B --> C[Assess risk, impact,<br/>dependencies, ethics]

        C --> D{Within LDA<br/>thresholds?}
        D -->|Yes| E[LDA decides]
        D -->|No| F[Escalate to CDA]

        E --> G[Record decision]
        F --> G

        G --> H[Feed into sensing loop]
  ```

## 3. LDA Decision Rights
LDAs decide on:
- domain-specific governance
- local prioritisation
- contextual interpretation of principles
- local risk and dependency management
- flow optimisation within the domain

## 4. LDA Decision Tests
- Does this decision maintain or improve flow?
- Does it align with SC4LE principles?
- Does it exceed escalation thresholds?
- Does it introduce systemic risk?

## 5. Behaviours
- contextual judgement
- transparency
- collaboration
- ethical awareness

## 6. Anti‑Patterns
- acting as a mini‑CDA
- over-escalation
- local optimisation at the expense of system flow

## 7. Maturity Indicators
- fewer escalations
- improved flow metrics
- consistent principle interpretation
