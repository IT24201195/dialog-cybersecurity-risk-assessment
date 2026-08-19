# Executive Cybersecurity Risk Report

## Dialog Axiata PLC - Public-Source Cybersecurity Risk Assessment

## 1. Executive Summary

This assessment evaluates cybersecurity risks relevant to Dialog Axiata PLC using publicly available information and recognized cybersecurity risk-management practices.

The assessment covers 20 cybersecurity risk scenarios:

- 10 enterprise cybersecurity risks
- 10 application-security risk scenarios aligned with OWASP Top 10:2025

The assessment identified significant risk exposure associated with customer information, authentication services, payment services, telecommunications availability, cloud infrastructure, customer-facing applications, third-party dependencies and operational resilience.

The initial risk assessment identified:

- 9 Critical inherent risks
- 11 High inherent risks
- 0 Medium or Low inherent risks

After considering publicly evidenced existing controls, the estimated current residual-risk distribution was:

- 0 Critical risks
- 17 High risks
- 3 Medium risks

The average analytical risk score decreased from:

**16.8 Inherent → 9.7 Current Residual**

However, several control and evidence gaps remain.

The most significant improvement areas identified are Secure Software Development Lifecycle maturity, identity and access governance, software-supply-chain security, third-party risk management, security monitoring, cryptographic governance, operational resilience and measurable control effectiveness.

Following implementation of the proposed risk treatments, the analytical model estimates that the overall risk profile could reduce further.

These values represent risk-management planning estimates and should not be interpreted as verified Dialog internal risk ratings.

---

## 2. Assessment Scope

The assessment considers publicly identifiable information assets, systems, services and business dependencies relevant to Dialog Axiata PLC.

The assessment includes risks affecting:

- Customer personal information
- Authentication services
- Digital payment services
- Telecommunications services
- Cloud infrastructure
- Customer web applications
- Customer mobile applications
- Employee accounts
- Security monitoring systems
- Backup and recovery capabilities
- Third-party and technology vendors

The assessment does not include penetration testing, vulnerability scanning or direct technical testing of Dialog infrastructure.

---

## 3. Risk Assessment Overview

Twenty cybersecurity risk scenarios were assessed.

The first ten represent broader enterprise cybersecurity risks:

- R001 - Customer Data Breach
- R002 - Credential Compromise
- R003 - Payment Fraud / Compromise
- R004 - DDoS / Service Disruption
- R005 - Cloud Misconfiguration
- R006 - Application Vulnerability
- R007 - Phishing / Employee Account Compromise
- R008 - Insider Threat
- R009 - Third-Party / Supply-Chain Compromise
- R010 - Backup / Recovery Failure

A further ten application-security scenarios were incorporated using OWASP Top 10:2025:

- R011 - Broken Access Control
- R012 - Security Misconfiguration
- R013 - Software Supply Chain Failure
- R014 - Cryptographic Failure
- R015 - Injection
- R016 - Insecure Design
- R017 - Authentication Failure
- R018 - Software or Data Integrity Failure
- R019 - Security Logging and Alerting Failure
- R020 - Mishandling of Exceptional Conditions

The OWASP scenarios represent potential application-security risk categories.

They do not represent confirmed vulnerabilities within Dialog systems.

---

## 4. Inherent Risk Profile

The inherent-risk assessment estimates risk before considering existing security controls.

The assessment identified:

- 9 Critical inherent risks
- 11 High inherent risks
- 0 Medium inherent risks
- 0 Low inherent risks

The average inherent risk score was approximately **16.8**.

This concentration of High and Critical inherent risk is expected because the assessed scenarios primarily affect high-value assets and critical telecommunications or digital services.

A successful compromise could potentially affect confidentiality, integrity, availability, customer trust, regulatory obligations or business operations.

---

## 5. Existing Security Controls

Public information reviewed during the assessment provides evidence of several security-control areas.

These include:

- Information security management
- Security monitoring
- Security testing
- Security awareness
- Access controls
- Information protection
- Incident response
- Business continuity and resilience

These controls were mapped against the identified risks.

However, public evidence of a control does not demonstrate that the control is operating effectively across all relevant systems.

Control existence, control implementation and control effectiveness were therefore treated as separate concepts throughout the assessment.

---

## 6. Current Residual Risk

After considering publicly evidenced existing controls, the analytical residual-risk profile was estimated as:

- 0 Critical risks
- 17 High risks
- 3 Medium risks
- 0 Low risks

The average residual risk score was approximately **9.7**.

The reduction from inherent risk reflects the expected effect of existing preventive, detective and corrective controls.

Residual-risk values remain analytical estimates because the assessment did not have access to internal control-testing results.

The relatively high remaining residual risk reflects the importance of the assets involved and uncertainty regarding detailed control implementation and effectiveness.

---

## 7. Control Gap Assessment

Ten consolidated control and evidence gaps were identified:

### GAP-001 - Identity and Access Governance

Additional assurance is required around privileged access, access certification, authentication controls and identity lifecycle management.

### GAP-002 - Secure Configuration Management

Detailed evidence regarding secure configuration baselines, automated configuration assessment and cloud configuration monitoring was not publicly available.

### GAP-003 - Software Supply Chain Security

Detailed evidence regarding dependency governance, Software Bills of Materials, artifact integrity and CI/CD supply-chain controls was not publicly available.

### GAP-004 - Cryptographic Governance

Detailed cryptographic standards, key-management practices, certificate governance and encryption coverage could not be independently assessed.

### GAP-005 - Secure Software Development Lifecycle

Public evidence was insufficient to determine the maturity and coverage of secure development practices including threat modelling, secure coding, automated security testing and security requirements.

This was assessed as the highest-priority consolidated control gap.

### GAP-006 - Security Logging, Detection and Alerting

Monitoring capabilities are publicly indicated, but detailed logging coverage, detection engineering, alert quality and monitoring effectiveness could not be independently assessed.

### GAP-007 - Third-Party Risk Management

Detailed vendor security assessment, reassessment and continuous monitoring processes were not publicly available.

### GAP-008 - Backup and Recovery Assurance

Detailed evidence regarding backup architecture, restoration testing, RTOs, RPOs and recovery testing was not publicly available.

### GAP-009 - Application Resilience and Exceptional-Condition Testing

Public evidence did not provide sufficient detail regarding fail-secure behaviour, negative testing, abnormal-state testing and application resilience.

### GAP-010 - Security Control Effectiveness Measurement

Public information provides evidence that security controls exist but does not provide sufficient information to independently determine their operating effectiveness.

---

## 8. Priority Treatment Areas

The risk-treatment assessment identified several areas requiring management attention.

### 8.1 Secure Software Development Lifecycle

Secure software development represents the most concentrated improvement area.

A mature Secure SDLC should incorporate:

- Security requirements
- Threat modelling
- Secure architecture review
- Secure coding standards
- Peer code review
- SAST
- DAST
- Dependency scanning
- Penetration testing
- Negative testing
- Abuse-case testing
- Security remediation tracking

This treatment area addresses multiple application-security risks simultaneously.

---

### 8.2 Identity and Access Governance

Identity controls affect several major risks including customer-data breach, credential compromise, insider activity, broken access control and authentication failure.

Priority measures include:

- Least privilege
- Role-based access control
- Strong authentication for appropriate high-risk access
- Privileged-access management
- Periodic access certification
- Secure account recovery
- Joiner/Mover/Leaver processes
- Authentication monitoring

---

### 8.3 Software Supply Chain and Third-Party Assurance

Modern digital services depend heavily on external software, technology vendors and service providers.

Priority measures include:

- Vendor risk classification
- Security due diligence
- Contractual security requirements
- Periodic vendor reassessment
- Critical-vendor monitoring
- Software Composition Analysis
- Software Bill of Materials governance
- Trusted dependency repositories
- Signed software artifacts
- Protected CI/CD pipelines
- Supplier incident-notification requirements

---

### 8.4 Security Monitoring and Incident Detection

Effective monitoring is required to identify malicious activity before incidents cause significant damage.

Priority measures include:

- Centralized security logging
- Critical-system audit trails
- SIEM monitoring
- Detection engineering
- High-risk alerts
- Protected log integrity
- Appropriate log retention
- Periodic detection testing
- Mean Time to Detect measurement
- Mean Time to Respond measurement

---

### 8.5 Cryptographic Governance

Sensitive customer and payment information requires consistent cryptographic protection.

Priority measures include:

- Approved cryptographic standards
- Secure transport encryption
- Appropriate encryption of sensitive information at rest
- Centralized key management
- Certificate lifecycle management
- Key rotation
- Periodic cryptographic review

---

### 8.6 Backup, Recovery and Operational Resilience

Critical telecommunications and digital services require tested recovery capabilities.

Priority measures include:

- Defined RTO and RPO targets
- Protected backups
- Immutable or offline backup capabilities where appropriate
- Restoration testing
- Disaster-recovery exercises
- Network redundancy
- Capacity monitoring
- DDoS protection
- Secure exception handling
- Graceful degradation

---

### 8.7 Control Effectiveness Measurement

Management should be able to determine whether cybersecurity controls are actually reducing risk.

Potential KPIs and KRIs include:

- Access-review completion rate
- Critical vulnerability remediation time
- Secure-development gate completion
- Vendor-assessment completion
- Critical dependency remediation time
- Backup restoration success rate
- Logging coverage
- Detection-test success rate
- Mean Time to Detect
- Mean Time to Respond
- Risk-treatment completion rate

---

## 9. Risk Treatment Strategy

The primary treatment strategy across the assessed risks is mitigation.

This reflects the high business impact associated with customer information, authentication systems, telecommunications availability, cloud services and customer-facing applications.

Third-party and software-supply-chain risks use a combined:

**Mitigate / Transfer**

strategy.

Security controls can reduce the likelihood and impact of supplier-related incidents, while contractual requirements can allocate specific responsibilities and financial or operational obligations to suppliers.

Risk acceptance should only occur following formal management review and consideration of organizational risk appetite.

---

## 10. Expected Post-Treatment Risk

The Risk Treatment Plan estimates the potential risk profile following successful implementation of the recommended treatments.

The analytical model estimates an average expected risk score of approximately **4.85**.

The model estimates:

- 0 Critical risks
- 0 High risks
- 17 Medium risks
- 3 Low risks

This represents the expected direction of risk reduction rather than a guaranteed security outcome.

The assessment generally reduces likelihood rather than impact.

This is intentional.

For example, stronger access controls may make a customer-data breach less likely, but if a major breach still occurred, its potential impact could remain severe.

Security controls therefore reduce risk without necessarily changing the underlying business consequence.

---

## 11. Framework Alignment

The assessment was mapped against:

- ISO/IEC 27001:2022
- NIST Cybersecurity Framework 2.0
- OWASP Top 10:2025

ISO/IEC 27001:2022 provides the information-security-management and control perspective.

NIST CSF 2.0 provides cybersecurity outcomes across:

- Govern
- Identify
- Protect
- Detect
- Respond
- Recover

OWASP Top 10:2025 provides current application-security risk categories used to strengthen the technical component of the assessment.

The frameworks were used to establish traceability between risk scenarios, control gaps and proposed treatments rather than to claim formal compliance.

---

## 12. Management Priorities

Based on the combined risk, control-gap and treatment assessment, the primary management priorities are:

1. Establish and continuously improve a mature Secure Software Development Lifecycle.
2. Strengthen identity and access governance.
3. Improve software-supply-chain and third-party security assurance.
4. Maintain effective security logging, detection and incident-response capabilities.
5. Strengthen cryptographic governance for sensitive information.
6. Regularly test backup, recovery and operational resilience.
7. Establish measurable control-effectiveness KPIs and KRIs.

These areas provide the greatest opportunity to reduce multiple cybersecurity risks simultaneously.

---

## 13. Limitations and Disclaimer

This assessment is based exclusively on publicly available information.

It is an independent educational cybersecurity risk assessment and is not affiliated with, commissioned by or endorsed by Dialog Axiata PLC.

The assessment did not include:

- Unauthorized access to Dialog systems
- Penetration testing of Dialog infrastructure
- Vulnerability scanning
- Exploitation
- Internal documentation review
- Employee interviews
- Internal audit evidence
- Configuration review
- Control testing

The assessment therefore does not claim that the identified risk scenarios or control gaps represent confirmed vulnerabilities or deficiencies within Dialog Axiata PLC.

Publicly unavailable control evidence was classified as an evidence limitation rather than proof that a control does not exist.

Proposed risk owners, treatment priorities, timeframes and expected risk values are analytical recommendations for the purpose of demonstrating cybersecurity GRC methodology.

---

## 14. Conclusion

The assessment demonstrates a structured cybersecurity risk-management process covering asset identification, risk assessment, control analysis, control-gap identification, risk treatment and framework alignment.

The analysis indicates that the most important cybersecurity themes for the assessed environment are application security, identity governance, third-party security, monitoring, cryptographic protection and operational resilience.

The project also demonstrates how technical security risks can be translated into governance and management decisions.

For example:

**OWASP application-security risk → Enterprise risk scenario → Control gap → Risk treatment → ISO 27001 control → NIST CSF 2.0 outcome → Management KPI**

This traceability allows cybersecurity risk to be communicated in both technical and business terms while maintaining clear limitations around what can be concluded from publicly available information.
