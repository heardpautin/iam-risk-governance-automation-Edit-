# IAM Risk Governance & Automation

## Overview
This project implements an Identity & Access Management (IAM) risk governance solution that evaluates user identity risk and operationalizes it through automated workflows.

Built using Microsoft Power BI and Microsoft Power Automate, this project demonstrates how identity risk scoring can move from analysis to action in a governance-driven security model.

It reflects real-world Identity Governance and Administration (IGA) and GRC principles including:
- Identity lifecycle risk evaluation
- Role-based access control (RBAC)
- Risk-based access governance
- Security automation workflows

---

## Core Concept

Modern identity governance is driven by continuous risk evaluation rather than static access rules.

This project models identity risk using key enterprise signals:

- Privileged access (Admin roles)
- User inactivity (stale accounts)
- Department sensitivity (e.g., Finance)
- Account status (active / temporary / inactive)

These signals are combined into a structured risk scoring model that supports governance decisions.

---

## Risk Scoring Model (Power BI)

The risk engine calculates a weighted score for each identity:

### Inputs:
- Role-based risk (privileged access)
- Inactivity risk (last login duration)
- Department-based sensitivity
- Account type / status

### Outputs:
- **RiskScore (numeric value)**
- **RiskLevel (Low / Medium / High classification)**

---

## Visualization Layer

The Power BI dashboard provides:

- User-level risk table view
- RiskScore comparison across identities
- RiskLevel categorization
- Conditional formatting:
  - High → Red
  - Medium → Orange
  - Low → Green

This enables rapid identification of high-risk identity patterns.

---

## Automation Layer (Power Automate – Implemented & Tested)

This project includes an implemented workflow automation layer using Microsoft Power Automate integrated with Power BI risk outputs.

### Implemented Workflow:

- Power Automate flow triggered by Power BI-derived RiskLevel conditions
- Automated alerts for High-risk identity states
- Event-driven notification logic simulating identity governance response behavior
- Manual testing performed to validate trigger conditions and workflow execution

### Validation:

The workflow was tested using sample identity scenarios to confirm:
- Correct trigger activation based on RiskLevel thresholds
- Successful execution of automated alerts
- End-to-end flow from risk detection to notification response

### Outcome:

This demonstrates a working prototype of event-driven identity governance where risk scoring is operationalized into automated response workflows.

---

## Tools & Technologies

- Microsoft Power BI
- DAX (Data Analysis Expressions)
- Microsoft Power Automate
- Identity Governance & Administration (IGA) concepts
- Role-Based Access Control (RBAC)
- Least Privilege principles
- Security workflow automation patterns

---

## Real-World Alignment

This project aligns with enterprise identity governance systems such as:

- Microsoft Entra ID risk-based access policies
- Conditional access decision frameworks
- Identity lifecycle governance models
- Security monitoring and alerting systems

It demonstrates how identity governance evolves from reporting into automated enforcement and response.

---

## Future Enhancements

- Add MFA strength scoring and authentication risk weighting
- Introduce anomaly detection (impossible travel, unusual login patterns)
- Expand role hierarchy and entitlement modeling
- Add multi-step Power Automate escalation workflows
- Integrate semantic model layer for advanced analytics
- Extend into AI-assisted risk interpretation for governance reporting

---

## Purpose

This project demonstrates practical IAM / IGA / GRC engineering capability by showing:

- Identity governance design and implementation
- Risk-based access evaluation
- Security automation integration
- Workflow-driven governance response
- Modern identity security architecture thinking

It represents a working prototype of how identity risk scoring systems evolve into automated governance and response frameworks in enterprise environments.