# Dialog Axiata PLC - Cybersecurity Risk Assessment

## Overview

This project is an independent, public-source cybersecurity risk assessment of Dialog Axiata PLC developed as a cybersecurity Governance, Risk and Compliance portfolio project.

The objective is to demonstrate an end-to-end cybersecurity risk-management process covering:

- Organizational scoping
- Asset identification
- Cybersecurity risk assessment
- Inherent and residual risk analysis
- Existing control assessment
- Control-gap analysis
- Risk treatment
- ISO/IEC 27001:2022 mapping
- NIST Cybersecurity Framework 2.0 mapping
- OWASP Top 10:2025 application-security risk analysis
- Executive cybersecurity reporting

The project connects technical cybersecurity risks with governance, controls, treatment decisions and management reporting.

> This project is based exclusively on publicly available information. It is not affiliated with, commissioned by or endorsed by Dialog Axiata PLC.

---

## Project Objective

The project was designed to answer five primary questions:

1. What information assets, systems and services are important to the organization?
2. What cybersecurity risks could affect those assets?
3. What security controls can be identified from publicly available evidence?
4. What additional control areas should be considered based on the identified risks?
5. How can those risks and controls be communicated using established cybersecurity frameworks?

The final output provides traceability across:

**Asset → Risk → Existing Control → Control Gap → Risk Treatment → Framework Mapping → Management Reporting**

---

## Assessment Scope

The assessment considers publicly identifiable technology and information assets associated with Dialog Axiata PLC, including areas such as:

- Customer personal information
- Authentication services
- Digital payment services
- Mobile services
- Fixed broadband
- Customer web applications
- Customer mobile applications
- Cloud and data-centre services
- Employee information
- Security logs
- Third-party providers
- Technology vendors
- Backup and recovery capabilities

No direct testing of Dialog systems was performed.

---

## Risk Methodology

Risk was assessed using:

**Risk Score = Likelihood × Impact**

Likelihood and impact were scored from 1 to 5.

Risk ratings were classified as:

| Score | Rating |
|---|---|
| 1-4 | Low |
| 5-9 | Medium |
| 10-16 | High |
| 17-25 | Critical |

The assessment distinguishes between:

### Inherent Risk

Risk before considering existing security controls.

### Current Residual Risk

Estimated risk after considering publicly evidenced existing controls.

### Expected Post-Treatment Risk

Estimated risk following successful implementation of proposed additional treatments.

Expected post-treatment values are planning estimates rather than verified organizational risk ratings.

---

## Risk Landscape

The project assesses 20 cybersecurity risk scenarios.

### Enterprise Cybersecurity Risks

- Customer Data Breach
- Credential Compromise
- Payment Fraud / Compromise
- DDoS / Service Disruption
- Cloud Misconfiguration
- Application Vulnerability
- Phishing / Employee Account Compromise
- Insider Threat
- Third-Party / Supply-Chain Compromise
- Backup / Recovery Failure

### OWASP Top 10:2025 Risk Scenarios

The assessment also incorporates the OWASP Top 10:2025 application-security categories:

- A01 - Broken Access Control
- A02 - Security Misconfiguration
- A03 - Software Supply Chain Failures
- A04 - Cryptographic Failures
- A05 - Injection
- A06 - Insecure Design
- A07 - Authentication Failures
- A08 - Software or Data Integrity Failures
- A09 - Security Logging and Alerting Failures
- A10 - Mishandling of Exceptional Conditions

These categories are treated as risk scenarios.

They do not represent confirmed vulnerabilities within Dialog Axiata PLC systems.

---

## Risk Assessment Results

The initial inherent-risk assessment identified:

- 9 Critical risks
- 11 High risks

After considering publicly evidenced controls, the analytical current residual-risk profile was:

- 0 Critical
- 17 High
- 3 Medium

Average analytical risk score:

**16.8 Inherent → 9.7 Current Residual**

Following the proposed treatments, the model estimates:

**9.7 Current Residual → 4.85 Expected Post-Treatment**

These values demonstrate the risk-treatment methodology and should not be interpreted as verified Dialog internal risk ratings.

---

## Control Assessment

Public information was reviewed to identify evidence of cybersecurity control areas including:

- Information security management
- Security monitoring
- Security testing
- Security awareness
- Access control
- Information protection
- Incident response
- Business continuity and resilience

Controls were evaluated using evidence classifications such as:

- Publicly Evidenced
- Partially Evidenced
- Not Publicly Verifiable

A lack of public evidence is not treated as evidence that a control does not exist.

---

## Key Control Gaps

The assessment identified ten consolidated control and evidence gaps:

1. Identity and Access Governance
2. Secure Configuration Management
3. Software Supply Chain Security
4. Cryptographic Governance
5. Secure Software Development Lifecycle
6. Security Logging, Detection and Alerting
7. Third-Party Risk Management
8. Backup and Recovery Assurance
9. Application Resilience and Exceptional-Condition Testing
10. Security Control Effectiveness Measurement

Secure Software Development Lifecycle was identified as the highest-priority consolidated treatment area because it affects several application-security risk scenarios.

---

## Risk Treatment

Each risk was assigned a proposed treatment strategy.

The primary strategy is:

**Mitigate**

Third-party and software-supply-chain risks use:

**Mitigate / Transfer**

Treatments include:

- Identity and access governance
- Privileged-access management
- Strong authentication
- Secure configuration management
- Secure Software Development Lifecycle
- SAST and DAST
- Dependency scanning
- Software Bill of Materials governance
- Security monitoring
- Incident detection
- Cryptographic governance
- Vendor security assessment
- Backup restoration testing
- Disaster recovery
- Control-effectiveness measurement

Each treatment is mapped to proposed owners, priorities, timeframes and measurable success indicators.

---

## Framework Mapping

### ISO/IEC 27001:2022

Relevant Annex A controls were mapped against identified risks, control gaps and proposed treatments.

The mapping includes areas such as:

- Access control
- Identity management
- Supplier security
- Cloud security
- Incident management
- Business continuity
- Privacy
- Vulnerability management
- Configuration management
- Logging
- Monitoring
- Cryptography
- Secure development
- Secure coding
- Security testing

The mapping does not represent an ISO 27001 certification assessment or Statement of Applicability.

### NIST Cybersecurity Framework 2.0

The assessment maps relevant risks and treatments across the six NIST CSF 2.0 Functions:

**Govern → Identify → Protect → Detect → Respond → Recover**

This demonstrates how enterprise cybersecurity risk can be translated into security outcomes and management activities.

### OWASP Top 10:2025

OWASP Top 10:2025 was used to strengthen the application-security component of the assessment.

The project demonstrates traceability such as:

**OWASP A05 Injection**

↓

**R015 - Injection**

↓

**GAP-005 - Secure Software Development Lifecycle**

↓

**T015 - Injection Risk Treatment**

↓

**ISO/IEC 27001 Secure Development Controls**

↓

**NIST CSF 2.0 PR.PS - Platform Security**

---

## Executive Reporting

An executive cybersecurity dashboard summarizes:

- Total risks
- Inherent risk distribution
- Current residual risk distribution
- Expected post-treatment risk
- Treatment priorities
- Control-gap priorities
- Risk reduction
- Management priority areas

This demonstrates how detailed cybersecurity analysis can be translated into information suitable for management decision-making.

---

## Repository Structure

```text
01-Organization-Scope/
    Organization-Profile.md
    Asset-Register.xlsx

02-Risk-Assessment/
    Risk-Register.xlsx
    Risk-Methodology.md

03-Control-Assessment/
    Control-Register.xlsx
    Control-Gap-Assessment.md
    Control-Gap-Register.xlsx

04-Risk-Treatment/
    Risk-Treatment-Plan.xlsx
    Risk-Treatment-Summary.md

05-Framework-Mapping/
    ISO-27001-Control-Mapping.xlsx
    NIST-CSF-2.0-Mapping.xlsx
    Framework-Mapping-Summary.md

06-Executive-Reporting/
    Executive-Risk-Dashboard.xlsx
    Executive-Risk-Report.md
