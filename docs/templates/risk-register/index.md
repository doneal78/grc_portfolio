---
layout: default
title: Risk Register (Template)
---

# Risk Register (Template)

**Contents**
* TOC
{:toc}

> Use this with your scoring model (e.g., FAIR-lite).  
> **Download the CSV:** [risk-register-template.csv]({{ '/assets/files/templates/risk-register-template.csv' | relative_url }})

## Columns
- **ID** — stable identifier (e.g., R-001).  
- **Risk** — short name (“Excess standing admin access”).  
- **Owner** — team or role who manages the risk.  
- **Likelihood (1–5)** — probability band.  
- **Impact (1–5)** — business impact band.  
- **Score** — simple product `L×I` (1–25).  
- **Treatment** — Mitigate, Transfer, Accept, Avoid.  
- **DueDate** — target completion date.  
- **Status** — Open, In Progress, Accepted, Closed.  
- **Notes** — context, justification, tickets.

## Example rows
| ID   | Risk                               | Owner   | L | I | Score | Treatment                  | DueDate     | Status |
|------|------------------------------------|---------|---:|---:|-----:|----------------------------|-------------|--------|
| R-01 | Excess standing admin access       | IT Ops  | 4 | 4 | 16    | Mitigate (JIT RBAC)        | 2025-10-01  | Open   |
| R-02 | Unpatched internet-facing servers  | Infra   | 3 | 5 | 15    | Mitigate (SLA + automation)| 2025-10-15  | Open   |
