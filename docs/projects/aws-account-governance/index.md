---
layout: default
title: AWS Account Governance — Case Study
---

# AWS Account Governance — Case Study

**Contents**
* TOC
{:toc}

This case study shows a pragmatic baseline for AWS account governance...

## Objectives
- Enforce MFA and least-privilege using IAM Identity Center.
- Continuously check configuration drift with AWS Config.
- Centralize findings in Security Hub for triage.
- Capture audit evidence; control cost with Budgets.
...

## Architecture
- **IAM Identity Center (SSO)** with MFA
- **AWS Config** managed rules (CIS-aligned)
- **AWS Security Hub** enabled
- **CloudTrail** logging
- **AWS Budgets** alerts

## Implementation Summary

### 1) Identity Center + MFA
- Create users/groups in Identity Center.
- Enforce MFA in settings.
- Map permission sets to roles (Admin, ReadOnly).

### 2) AWS Config
- Turn on Config in the region.
- Add managed rules (CIS baseline subset).

### 3) Security Hub
- Enable Security Hub.
- Turn on CIS/AWS Foundational checks.

### 4) CloudTrail
- One account trail, all management events.

### 5) Budgets
- Create monthly cost budget with email alerts.

## Risk & Control Mapping
- **NIST CSF**: ID.AM, PR.AC, DE.CM, RS.MI  
- **CIS Controls**: 5, 6, 8, 16

## Artifacts (add later if you like)
- IAM policies (JSON)  
- Config rules list (CSV)  
- Screenshots (Security Hub, Config, Budgets)
