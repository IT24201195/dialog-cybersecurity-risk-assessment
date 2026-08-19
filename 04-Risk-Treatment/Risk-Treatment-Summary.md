# Risk Treatment Summary

## 1. Purpose

This document summarizes the proposed treatment strategy for the cybersecurity risks identified in the Dialog Axiata PLC public-source cybersecurity risk assessment.

The treatment plan is based on the current residual-risk estimates, identified control and evidence gaps, and recommended security practices. Proposed actions, owners, priorities, and timeframes are analytical recommendations and do not represent confirmed Dialog internal plans or assignments.

## 2. Treatment Approach

The assessment uses four standard risk-treatment options:

- Mitigate - reduce the likelihood or impact of a risk through additional or strengthened controls.
- Transfer - allocate defined portions of financial or operational exposure through contracts, insurance, outsourcing, or other arrangements.
- Avoid - discontinue or materially change the activity creating unacceptable risk.
- Accept - formally retain residual risk when it is within approved risk appetite or further treatment is not proportionate.

Most assessed risks are recommended for mitigation because they affect customer information, authentication, payment services, telecommunications availability, cloud infrastructure, software security, or operational resilience.

Third-party and software-supply-chain risks use a combined Mitigate / Transfer approach because technical and governance controls can reduce exposure while contractual requirements can allocate specific responsibilities to suppliers.

## 3. Prioritization

Treatment priorities were assigned according to the current residual risk, control gaps, affected assets, and potential business impact.

- Critical - immediate security improvement focus, proposed within 0-3 months.
- High - significant improvement priority, proposed within 3-6 months.
- Medium - planned improvement, proposed within 6-12 months.
- Low - monitor or address through normal improvement cycles.

Critical treatment priority is concentrated around application-security risks that depend on a mature Secure Software Development Lifecycle, including application vulnerabilities and several OWASP Top 10:2025 categories.

## 4. Key Treatment Themes

### Identity and Access Management

Risks involving customer accounts, broken access control, authentication failure, insider activity, and data breach require stronger identity governance.

Proposed measures include:

- Least privilege
- Role-based access control
- Appropriate strong authentication
- Privileged-access management
- Periodic access certification
- Secure account recovery
- Joiner/Mover/Leaver controls
- Authentication monitoring

### Secure Software Development

Application-security risks require a formal Secure SDLC.

Proposed measures include:

- Security requirements
- Threat modelling
- Secure design review
- Secure coding standards
- Peer code review
- SAST
- DAST
- Dependency scanning
- Penetration testing
- Negative and abuse-case testing
- Remediation tracking

This treatment area addresses the original application-vulnerability risk and OWASP Top 10:2025 risks including Broken Access Control, Security Misconfiguration, Injection, Insecure Design, Authentication Failures, Software or Data Integrity Failures, and Mishandling of Exceptional Conditions.

### Software Supply Chain and Third-Party Risk

Third-party and software-supply-chain risks require controls across both supplier governance and software delivery.

Proposed measures include:

- Vendor risk classification
- Security due diligence
- Contractual security requirements
- Periodic reassessment
- Critical-vendor monitoring
- Software Composition Analysis
- Software Bill of Materials governance
- Trusted dependency repositories
- Signed software artifacts
- Protected CI/CD pipelines
- Incident-notification requirements

### Monitoring and Incident Detection

Security monitoring should provide sufficient visibility to identify attacks and support investigation.

Proposed measures include:

- Centralized security logging
- Critical-system audit trails
- SIEM monitoring
- Detection use cases
- High-risk alerts
- Protected log integrity
- Defined retention requirements
- Periodic detection testing
- Mean Time to Detect and Mean Time to Respond measurement

### Cryptographic Protection

Sensitive customer and payment information requires consistent cryptographic governance.

Proposed measures include:

- Approved cryptographic standards
- Secure transport encryption
- Encryption of sensitive information at rest where appropriate
- Centralized key management
- Certificate lifecycle management
- Key rotation
- Periodic cryptographic review

### Resilience and Recovery

Service disruption and backup failure require preventive and recovery-oriented controls.

Proposed measures include:

- DDoS protection
- Traffic filtering
- Network redundancy
- Capacity monitoring
- Defined RTO and RPO targets
- Immutable or offline backup protection
- Restoration testing
- Disaster-recovery exercises
- Secure exception handling
- Graceful degradation
- Fail-secure behaviour

## 5. Expected Risk Reduction

The Risk Treatment Plan estimates the expected risk after successful implementation of the proposed controls.

These values are planning estimates rather than verified organizational risk ratings.

The expected likelihood generally decreases because the proposed treatments strengthen preventive, detective, and corrective controls. Impact is usually retained at its original severity because a successful compromise of a critical asset could still have major consequences even when the probability of occurrence is reduced.

This approach avoids assuming that additional controls eliminate the underlying business impact.

## 6. Success Measurement

Risk treatment should be measured rather than considered complete simply because a control has been introduced.

Example measures include:

- Access-review completion rate
- Critical vulnerability remediation time
- Secure-development gate completion
- Authentication attack detection
- Vendor-assessment completion
- Critical dependency remediation time
- Backup restoration success rate
- Recovery exercise performance
- Logging coverage
- Detection-test success rate
- Mean Time to Detect
- Mean Time to Respond
- Risk-treatment completion rate

## 7. Management Considerations

The highest-value improvement areas identified by this assessment are:

1. Establishing a mature Secure SDLC for customer-facing applications.
2. Strengthening identity and access governance.
3. Improving software-supply-chain and third-party assurance.
4. Maintaining measurable logging, detection, and response capabilities.
5. Strengthening cryptographic governance.
6. Demonstrating backup, recovery, and operational resilience through testing.
7. Measuring control effectiveness through defined KPIs and KRIs.

Treatment decisions should ultimately be reviewed against organizational risk appetite, implementation cost, regulatory requirements, business priorities, and internal control-testing results.

## 8. Limitations

This treatment plan is based exclusively on publicly available information and analytical risk scenarios.

The assessment does not have access to Dialog Axiata PLC internal policies, system configurations, audit evidence, risk appetite, security-testing results, control-performance data, or management decisions.

Therefore:

- Proposed owners are functional recommendations and are not confirmed internal assignments.
- Target timeframes are suggested planning priorities and are not Dialog commitments.
- Expected residual-risk values are analytical estimates.
- Identified control gaps should not be interpreted as confirmation that a control is absent.
- Recommended treatments should not be interpreted as evidence of an existing vulnerability.

The plan is intended to demonstrate a structured cybersecurity GRC risk-treatment methodology using public information.
