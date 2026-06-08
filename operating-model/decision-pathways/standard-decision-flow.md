---
title: Standard Decision Flow
version: 1.0.1
status: canonical
last-updated: 2026-06-08
---

# Standard Decision Flow

## 1. Purpose
The Standard Decision Flow defines how decisions move through the SC4LE federated governance system. It ensures decisions are made at the **lowest responsible level**, with escalation only when thresholds are exceeded.

## 2. Scope
Applies to all decisions made by:
- operational teams  
- Local Design Authorities (LDAs)  
- Central Design Authority (CDA)  

## 3. Decision Flow (Mermaid)

```mermaid
flowchart TD
    A[Team identifies decision] --> B[Apply SC4LE principles]

    B --> C{Reversible, low-risk,<br/>local impact?}
    C -->|Yes| D[Team decides]
    C -->|No| E{Contextual,<br/>domain-specific?}

    E -->|Yes| F[LDA decides]
    E -->|No| G[Cross-domain, high-impact,<br/>ethical or regulatory risk]

    G --> H[CDA decides]

    D --> I[Decision logged]
    F --> I
    H --> I

    I --> J[Sensing loop captures impact]
