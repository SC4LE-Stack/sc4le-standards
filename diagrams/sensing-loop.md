---
title: SC4LE Sensing Loop Diagram
version: 1.0.0
status: canonical
last-updated: 2026-06-08
---

# SC4LE Sensing Loop Diagram

This diagram shows the continuous sensing cycle:  
Sensing → Insight → Decision → Action → Outcome → Sensing.

```mermaid
flowchart TD

    A[Sensing Signals] --> B[Insight Generation]
    B --> C[Decision Making]
    C --> D[Action / Intervention]
    D --> E[Outcome Observed]
    E --> A
