# IAM Governance & Risk-Based Access Control System

## Overview

This project implements an end-to-end Identity and Access Management (IAM) governance system that combines risk-based identity analytics with automated access request and approval workflows.

It demonstrates how identity governance operates in modern enterprises by connecting identity risk scoring, access request intake, automated approval routing, and audit logging into a single system.

Built using Microsoft Power BI, Power Apps, SharePoint, and Power Automate, this project simulates a real-world Identity Governance and Administration (IGA) lifecycle.

---

## Architecture

Identity Data → Risk Scoring Engine → Risk Level Output → Access Request System → Workflow Automation → Audit Logging → Reporting

---

## Business Problem

Organizations struggle with:
- Excessive user access privileges
- Lack of structured approval workflows
- Manual and inconsistent governance decisions
- Limited visibility into identity risk
- Weak audit and compliance traceability

This system addresses these challenges through structured identity governance and automation.

---

## Core Components

### Risk Scoring Engine (Power BI)
Evaluates identity risk using:
- Privileged access roles
- User inactivity (last login)
- Department sensitivity
- Account status

Outputs:
- RiskScore
- RiskLevel (Low / Medium / High)

---

### Access Request System (Power Apps)
Users submit structured access requests including:
- Requested role
- Department
- Business justification
- Identity metadata

---

### Governance Workflow (Power Automate)
Automates approval routing based on risk:

- High Risk → Security/Compliance review
- Medium Risk → Manager approval
- Low Risk → Standard or auto-approval

Includes:
- Conditional routing logic
- Approval/rejection actions
- Automated notifications
- SharePoint write-back updates

---

### Data & Audit Layer (SharePoint)
Stores:
- User identity data
- Access requests
- Approval decisions
- Reviewer comments
- Audit trail history

---

### Reporting Layer (Power BI)
Provides governance visibility:
- Risk distribution across users
- Access approval trends
- High-risk identity patterns
- Department-level analysis

---

## Governance Logic

- High-risk identities trigger enhanced review
- Privileged roles require additional approval layers
- Inactive accounts are flagged for review
- Department sensitivity influences risk scoring
- All decisions are logged for auditability

---

## IAM Lifecycle Modeled

1. Identity evaluation
2. Risk scoring
3. Access request submission
4. Approval workflow execution
5. Decision enforcement
6. Audit logging
7. Governance reporting

---

## Tools Used

- Microsoft Power BI
- Microsoft Power Apps
- Microsoft Power Automate
- Microsoft SharePoint

---

## Real-World Alignment

This system aligns with enterprise identity governance practices including:
- Microsoft Entra ID Identity Protection
- Conditional Access frameworks
- SOC 2 / ISO 27001 access controls
- Identity Governance and Administration (IGA) systems

---

## Outcome

This project demonstrates a complete IAM governance lifecycle system that connects identity risk analysis, access decisions, workflow automation, and audit visibility into a unified governance model.

---
## Roadmap / Future Enhancements

This project is currently a functional proof-of-concept demonstrating end-to-end IAM governance workflows.

Planned enhancements include:
- Improved role-based access catalog
- Expanded risk scoring logic
- Additional workflow branching for complex approval scenarios
- Enhanced reporting and dashboard refinements in Power BI
- Integration with enterprise IAM platforms (e.g., Entra ID / SailPoint concepts)

These enhancements are intended to simulate scaling this POC into an enterprise-grade identity governance system.
---
## Author

Craig Heard  
IAM | GRC | Cloud Security | Identity Governance
