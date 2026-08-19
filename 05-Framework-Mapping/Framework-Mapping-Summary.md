# Framework Mapping Summary

## 1. Purpose

This document summarizes how the cybersecurity risks, control gaps and proposed risk treatments identified in the Dialog Axiata PLC public-source cybersecurity risk assessment align with recognized cybersecurity frameworks.

The assessment considers:

- ISO/IEC 27001:2022 Annex A controls
- NIST Cybersecurity Framework 2.0
- OWASP Top 10:2025

The purpose of the mapping is to demonstrate traceability between identified cybersecurity risks and established security practices.

This is not an ISO 27001 certification assessment, formal Statement of Applicability, NIST CSF Organizational Profile or internal security audit.

## 2. Framework Mapping Approach

The assessment follows the relationship:

Asset → Risk → Existing Control → Control Gap → Risk Treatment → Framework Requirement

For application-security risks, OWASP Top 10:2025 categories are also incorporated:

OWASP Category → Risk → Control Gap → Risk Treatment → ISO 27001 Control → NIST CSF 2.0 Category

This provides traceability from a cybersecurity risk scenario through proposed treatment and recognized security frameworks.

## 3. ISO/IEC 27001:2022 Alignment

Relevant ISO/IEC 27001:2022 Annex A controls were selected based on the risks and treatments identified during the assessment.

The mapping focuses primarily on controls relating to:

- Information security governance
- Asset management
- Identity and access management
- Supplier security
- Cloud security
- Incident management
- Business continuity
- Privacy
- Security awareness
- Vulnerability management
- Configuration management
- Logging and monitoring
- Cryptography
- Secure software development
- Application security
- Secure coding
- Security testing
- Change management

Controls were not marked as implemented unless sufficient public evidence was available.

Instead, the assessment uses evidence states such as:

- Publicly Evidenced
- Partially Evidenced
- Not Publicly Verifiable

This distinction is important because the existence of a relevant ISO control does not demonstrate that the control is implemented or operating effectively within the organization.

## 4. NIST Cybersecurity Framework 2.0 Alignment

The assessment maps the cybersecurity program against the six NIST CSF 2.0 Functions:

### Govern

Govern addresses how cybersecurity risk-management strategy, expectations and policy are established and monitored.

Relevant areas include:

- Organizational context
- Risk-management strategy
- Roles and responsibilities
- Cybersecurity policy
- Oversight
- Cybersecurity supply-chain risk management

The risk assessment, proposed risk owners, control-gap assessment and treatment strategy strongly relate to the Govern function.

### Identify

Identify focuses on understanding organizational cybersecurity risks.

Relevant areas include:

- Asset Management
- Risk Assessment
- Improvement

The Asset Register and Risk Register provide the primary portfolio evidence for this function.

### Protect

Protect focuses on safeguards used to manage cybersecurity risk.

Relevant areas include:

- Identity Management, Authentication and Access Control
- Awareness and Training
- Data Security
- Platform Security
- Technology Infrastructure Resilience

Major treatments involving IAM, cryptography, Secure SDLC, configuration management, vulnerability management and resilience align strongly with this function.

### Detect

Detect addresses the identification and analysis of cybersecurity events.

Relevant areas include:

- Continuous Monitoring
- Adverse Event Analysis

Security logging, SIEM monitoring, detection engineering and alert testing are key treatment areas associated with this function.

### Respond

Respond addresses actions performed when a cybersecurity incident occurs.

Relevant areas include:

- Incident Management
- Incident Analysis
- Incident Response Reporting and Communication
- Incident Mitigation

The existing incident-response control and proposed improvements to detection, investigation, communication and containment align with this function.

### Recover

Recover addresses restoration of assets and operations affected by cybersecurity incidents.

Relevant areas include:

- Incident Recovery Plan Execution
- Incident Recovery Communication

Backup assurance, restoration testing, disaster recovery, resilience and recovery communication are the primary treatment areas associated with this function.

## 5. OWASP Top 10:2025 Alignment

The application-security portion of the assessment incorporates the current OWASP Top 10:2025 categories:

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

These categories were converted into risk scenarios R011-R020 rather than being treated as confirmed vulnerabilities.

This distinction is important because the assessment did not perform penetration testing against Dialog Axiata systems.

The OWASP categories are therefore used to evaluate relevant application-security risk exposure and appropriate control requirements.

## 6. Cross-Framework Traceability

One of the main objectives of this project is to demonstrate that cybersecurity frameworks should not be treated as isolated checklists.

For example:

OWASP A05 - Injection

↓

R015 - Injection Risk

↓

GAP-005 - Secure Software Development Lifecycle

↓

T015 - Injection Risk Treatment

↓

ISO/IEC 27001:2022 controls relating to Secure SDLC, application security requirements, secure coding and security testing

↓

NIST CSF 2.0 - PR.PS Platform Security

This demonstrates how a technical application-security issue can be translated into risk, governance requirements, control improvements and framework alignment.

Another example is third-party risk:

R009 - Third-Party / Supply-Chain Compromise

↓

GAP-003 - Software Supply Chain Security

GAP-007 - Third-Party Risk Management

↓

T009 - Third-Party Risk Treatment

↓

ISO/IEC 27001:2022 supplier and ICT supply-chain controls

↓

NIST CSF 2.0 - GV.SC Cybersecurity Supply Chain Risk Management

This provides a direct connection between enterprise risk management and technical cybersecurity controls.

## 7. Key Framework Findings

The strongest areas of framework relevance identified by the assessment are:

1. Information security risk management
2. Identity and access governance
3. Secure software development
4. Third-party and software-supply-chain security
5. Security monitoring and incident response
6. Cryptographic protection
7. Business continuity and recovery
8. Control-effectiveness measurement

The Secure Software Development Lifecycle represents one of the most significant treatment themes because it addresses multiple OWASP Top 10:2025 risk scenarios.

Identity and access governance is similarly important because it affects customer-data protection, credential compromise, insider risk, broken access control and authentication failure.

## 8. Framework Coverage Limitations

Framework alignment does not demonstrate framework compliance.

This assessment is based exclusively on publicly available information.

The assessment does not have access to internal:

- Policies
- Procedures
- System configurations
- Audit evidence
- Control-testing results
- Management-review records
- Risk-acceptance decisions
- Supplier assessments
- Secure-development documentation
- Incident records
- Business-continuity test results

Therefore, framework mappings indicate where a control or cybersecurity outcome is relevant to the identified risks.

They do not confirm that Dialog Axiata PLC has or has not implemented a particular control.

## 9. Conclusion

The framework mapping demonstrates how the identified cybersecurity risks can be managed using recognized security standards and practices.

ISO/IEC 27001:2022 provides the control and information-security-management perspective.

NIST CSF 2.0 provides an outcome-based cybersecurity risk-management structure across Govern, Identify, Protect, Detect, Respond and Recover.

OWASP Top 10:2025 provides current application-security risk categories that strengthen the technical portion of the assessment.

Together, these frameworks demonstrate how governance, risk management and technical cybersecurity controls can be connected within a single cybersecurity risk-management program.
