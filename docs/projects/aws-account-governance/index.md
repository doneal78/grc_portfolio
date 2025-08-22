---
layout: default
title: AWS Account Governance Case Study
permalink: /projects/aws-account-governance/
---

# AWS Account Governance Case Study

**Objective**: Design an AWS account structure aligned to NIST CSF, with least privilege and continuous monitoring.

## Problem
Teams adopting AWS often face:
- Siloed accounts without consistent guardrails  
- Over‑privileged identities  
- Manual compliance checks that don’t scale  

## Approach
1. **Baseline Controls** — mapped NIST CSF categories to AWS native services.  
   - Identity & Access → AWS IAM Identity Center  
   - Configuration Management → AWS Config rules  
   - Continuous Monitoring → Security Hub  
2. **Least Privilege** — role‑based access with scoped permissions.  
3. **Guardrails** — Service Control Policies (SCPs) for region use, MFA, budgets.  
4. **Evidence** — screenshots of configs, CLI output, CloudTrail logs for audit packages.

## Outcome
- Reduced risk of unauthorized changes via SCPs across **100% of accounts**  
- Aligned AWS guardrails to **50+ NIST CSF subcategories**  
- Repeatable onboarding pattern with governance pre‑baked

## Evidence Artifacts
- Config rule compliance snapshots  
- IAM role/permission screenshots  
- Mapping matrix: NIST CSF ↔ AWS services
