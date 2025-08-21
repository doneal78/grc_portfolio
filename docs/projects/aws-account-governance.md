---
layout: default
title: AWS Account Governance — Case Study
permalink: /projects/aws-account-governance/
---

# AWS Account Governance — Case Study

This case study demonstrates how to establish AWS account governance and security foundations aligned with industry best practices.  
It covers identity management, continuous compliance, centralized security monitoring, and cost controls.

## Objectives
- Enforce strong identity and access controls (MFA, least privilege).
- Enable continuous compliance with AWS Config.
- Centralize findings with AWS Security Hub.
- Provide audit-ready evidence and documentation.

## Architecture
- **IAM Identity Center (SSO)** with MFA required for all users.
- **AWS Config** for continuous compliance against CIS benchmarks.
- **AWS Security Hub** enabled across the account.
- **AWS CloudTrail** centralized logging.
- **AWS Budgets** to alert on spend thresholds.

## Implementation Steps
1. Enable **IAM Identity Center** and enforce MFA.
2. Configure **AWS Config** with managed rules for CIS compliance.
3. Enable **AWS Security Hub** in the account.
4. Deploy a **CloudTrail** trail to capture all API activity.
5. Set up **Budgets** with alerting thresholds.

## Evidence / Artifacts
- IAM policy JSON files (least privilege).
- Config rule compliance reports.
- Security Hub findings screenshots.
- Budget alert notification samples.

## Risk & Control Mapping
- **NIST CSF**: ID.AM, PR.AC, DE.CM, RS.MI
- **CIS Controls**: 5, 6, 8, 16

## Lessons Learned
- Automating compliance checks reduced manual effort.
- Security Hub provided better visibility for incident response.
- Clear alignment with frameworks made audits smoother.

---
