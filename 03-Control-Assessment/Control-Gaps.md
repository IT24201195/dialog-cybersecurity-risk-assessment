# Control Gap Assessment

## 1. Purpose

This assessment identifies control and evidence gaps associated with the cybersecurity risks identified for Dialog Axiata PLC.

The assessment is based exclusively on publicly available information. An identified gap does not confirm that a control is absent or ineffective within Dialog. Instead, it indicates that sufficient public evidence was not available to independently verify the design, implementation, coverage or operating effectiveness of the relevant control.

## 2. Assessment Approach

Control gaps were identified by comparing:

- Identified cybersecurity risk scenarios
- Publicly documented security controls
- Available evidence regarding those controls
- Recommended security practices
- OWASP Top 10:2025 application-security risk categories

Control effectiveness was not independently tested.

---

## GAP-001 - Identity and Access Governance

### Related Risks
R001 - Customer Data Breach  
R002 - Credential Compromise  
R008 - Insider Threat  
R011 - Broken Access Control  
R017 - Authentication Failures

### Observation
Public information indicates that access restrictions and security safeguards are used to protect personal information. However, sufficient public evidence was not available to verify detailed identity and access governance practices such as privileged-access management, periodic access certification, role-based access reviews, authentication-control coverage and Joiner/Mover/Leaver processes.

### Potential Impact
Weaknesses in identity governance could contribute to unauthorized access, excessive privileges, account compromise or misuse of legitimate access.

### Recommendation
Maintain and periodically assess:

- Least-privilege access
- Role-based access control
- MFA for appropriate high-risk access
- Privileged-access management
- Periodic user-access certification
- Dormant-account reviews
- Joiner/Mover/Leaver controls
- Authentication monitoring

### Evidence Limitation
Detailed IAM architecture and operating-effectiveness evidence were not publicly available.

---

## GAP-002 - Secure Configuration Management

### Related Risks
R005 - Cloud Misconfiguration  
R012 - Security Misconfiguration

### Observation
Public information supports the existence of information-security governance and security assessment activities. However, detailed evidence regarding hardened configuration baselines, automated configuration monitoring and configuration-compliance assessment was not available.

### Potential Impact
Security misconfiguration could expose services, information, administrative interfaces or cloud resources.

### Recommendation
Implement or continuously maintain:

- Secure configuration baselines
- Configuration compliance scanning
- Cloud security posture monitoring
- Removal of unnecessary services
- Environment separation
- Change control
- Periodic configuration reviews

### Evidence Limitation
Internal configuration standards and compliance results could not be independently verified.

---

## GAP-003 - Software Supply Chain Security

### Related Risks
R009 - Third-Party / Supply Chain Compromise  
R013 - Software Supply Chain Failures  
R018 - Software or Data Integrity Failures

### Observation
Public information indicates third-party relationships and organizational security governance. However, detailed evidence regarding software dependency governance, SBOM usage, artifact integrity, dependency scanning and CI/CD supply-chain controls was not publicly available.

### Potential Impact
Compromise of dependencies, software repositories, build systems or vendors could introduce vulnerable or malicious components into trusted systems.

### Recommendation
Establish or maintain:

- Software Composition Analysis
- Software Bill of Materials
- Approved dependency repositories
- Dependency/version governance
- Signed build artifacts
- Protected CI/CD pipelines
- Vendor security assessment
- Software integrity verification

### Evidence Limitation
Internal software-supply-chain controls could not be independently assessed.

---

## GAP-004 - Cryptographic Governance

### Related Risks
R001 - Customer Data Breach  
R003 - Payment Compromise  
R014 - Cryptographic Failures

### Observation
Public privacy information describes security protections for personal information. However, detailed information regarding cryptographic standards, encryption coverage, key management, certificate management and cryptographic lifecycle governance is not publicly available.

### Potential Impact
Weak or incorrectly implemented cryptography could expose sensitive customer, payment or authentication information.

### Recommendation
Maintain:

- Approved cryptographic standards
- Encryption of sensitive data in transit
- Encryption of sensitive data at rest where appropriate
- Centralized key management
- Certificate lifecycle management
- Key rotation
- Periodic cryptographic review

### Evidence Limitation
Algorithms, key-management architecture and implementation effectiveness could not be independently verified.

---

## GAP-005 - Secure Software Development Lifecycle

### Related Risks
R006 - Application Vulnerability  
R011 - Broken Access Control  
R015 - Injection  
R016 - Insecure Design  
R017 - Authentication Failures  
R018 - Software or Data Integrity Failures  
R020 - Mishandling of Exceptional Conditions

### Observation
Public information supports the existence of cybersecurity and security-testing activities. However, sufficient public evidence was not available to determine the maturity and coverage of secure software-development practices.

### Potential Impact
Security weaknesses introduced during design, development or deployment could result in unauthorized access, injection, business-logic abuse, insecure error handling or application compromise.

### Recommendation
Maintain a Secure SDLC incorporating:

- Security requirements
- Threat modelling
- Secure design review
- Secure coding standards
- Peer code review
- SAST
- DAST
- Dependency scanning
- Security testing
- Negative and abuse-case testing
- Remediation tracking

### Evidence Limitation
Secure SDLC procedures and testing coverage could not be independently verified.

---

## GAP-006 - Security Logging, Detection and Alerting

### Related Risks
R001 - Customer Data Breach  
R002 - Credential Compromise  
R004 - Service Disruption  
R007 - Employee Account Compromise  
R019 - Security Logging and Alerting Failures

### Observation
Security monitoring capabilities are publicly indicated. However, detailed evidence regarding log-source coverage, alerting rules, log retention, detection engineering, SIEM coverage and detection effectiveness was not publicly available.

### Potential Impact
Insufficient logging or alerting could allow malicious activity to remain undetected and increase incident duration.

### Recommendation
Maintain:

- Centralized security logging
- Defined security logging standards
- Critical-system audit trails
- SIEM monitoring
- Detection use cases
- High-risk security alerts
- Appropriate log retention
- Protected log integrity
- Periodic detection testing

### Evidence Limitation
Monitoring coverage and detection effectiveness could not be independently tested.

---

## GAP-007 - Third-Party Risk Management

### Related Risks
R009 - Third-Party / Supply Chain Compromise  
R013 - Software Supply Chain Failures

### Observation
Dialog publicly identifies relationships involving service providers and other third parties. However, detailed cybersecurity vendor-risk procedures are not sufficiently visible in the public evidence reviewed.

### Potential Impact
A compromised or inadequately controlled third party could expose information, introduce malicious software or disrupt critical services.

### Recommendation
Maintain a formal third-party risk-management process including:

- Vendor risk classification
- Security due diligence
- Contractual security requirements
- Data-protection requirements
- Periodic reassessment
- Critical-vendor monitoring
- Incident notification requirements
- Vendor offboarding

### Evidence Limitation
Internal vendor assessment and monitoring records were not available.

---

## GAP-008 - Backup and Recovery Assurance

### Related Risks
R004 - Service Disruption  
R010 - Backup / Recovery Failure

### Observation
Public information indicates business-continuity and resilience considerations. However, detailed evidence regarding backup architecture, restoration testing, recovery objectives and ransomware-resilient backups was not available.

### Potential Impact
Backup failure could increase recovery time and operational impact following ransomware, destructive attacks or infrastructure failure.

### Recommendation
Maintain:

- Defined RTOs and RPOs
- Regular backups
- Offline or immutable backup protection where appropriate
- Restoration testing
- Disaster-recovery exercises
- Backup integrity monitoring
- Documented recovery procedures

### Evidence Limitation
Backup configuration and recovery-test results could not be independently verified.

---

## GAP-009 - Application Resilience and Exceptional-Condition Testing

### Related Risks
R004 - Service Disruption  
R020 - Mishandling of Exceptional Conditions

### Observation
Public information does not provide sufficient detail to assess how customer-facing applications are tested for abnormal conditions, resource exhaustion, unexpected states or fail-open behaviour.

### Potential Impact
Unexpected application conditions could cause service degradation, information leakage or security controls to behave incorrectly.

### Recommendation
Include:

- Fail-secure design
- Exception handling standards
- Negative testing
- Resource limits
- Graceful degradation
- Generic external error messages
- Availability testing
- Unexpected-state testing

### Evidence Limitation
Detailed resilience and exceptional-condition testing practices were not publicly available.

---

## GAP-010 - Security Control Effectiveness Measurement

### Related Risks
All assessed risks

### Observation
Public sources provide evidence of several cybersecurity controls but do not provide sufficient information to independently determine their operating effectiveness across the assessed environment.

### Potential Impact
Without measurable control-effectiveness information, management may have limited visibility into whether controls are consistently reducing risk to intended levels.

### Recommendation
Maintain measurable security and GRC indicators including:

- Control compliance rate
- Access-review completion rate
- Critical vulnerability remediation time
- Phishing simulation performance
- Vendor-assessment completion
- Backup restoration success rate
- Mean Time to Detect
- Mean Time to Respond
- Security-testing remediation rate
- Risk-treatment completion rate

### Evidence Limitation
Internal KPI, KRI, audit and control-testing results were not publicly available.

---

# 3. Overall Conclusion

The public-source assessment identified evidence of information-security governance, access protection, security monitoring, security testing, incident response and resilience-related activities.

However, public information does not provide sufficient evidence to independently verify the detailed design or operating effectiveness of many controls.

Accordingly, the gaps identified in this assessment should be interpreted as evidence and assurance gaps rather than confirmed deficiencies within Dialog Axiata PLC.

The assessment should not be interpreted as an internal security audit, vulnerability assessment or assertion that the organization contains the weaknesses described.
