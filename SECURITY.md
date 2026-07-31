# Security Policy

Thank you for helping improve the security of Octacity projects.

This document provides the default security-reporting guidelines used across the organization. Individual repositories may define additional or different requirements, so always review the repository's own `SECURITY.md`, README, and contribution guidelines first.

Repository-specific security policies take precedence over this document.

## Supported Versions

Unless a repository states otherwise, security fixes are provided for the default branch.

Maintaining teams may define support for specific releases, versions, branches, or deployment environments in their repository-level security policy.

## Reporting a Vulnerability

Credible vulnerabilities that could expose data, privileges, secrets, system access, availability, or code execution should be reported privately through GitHub Private Vulnerability Reporting.

Use the **Security** tab of the affected repository and select **Report a vulnerability** when that option is available.

Do not open a public issue for a vulnerability that could place users, deployments, maintainers, or infrastructure at risk.

Security-critical and safety-critical repositories are strongly encouraged to enable GitHub Private Vulnerability Reporting.

## What Should Be Reported Privately

Private reporting is appropriate when an issue may allow:

- Unauthorized access to data or accounts
- Authentication or authorization bypass
- Exposure of credentials, tokens, keys, or other secrets
- Remote or unintended code execution
- Privilege escalation
- Injection attacks
- Circumvention of security boundaries
- Unsafe file access or path traversal
- Serious cryptographic misuse
- Denial of service with credible practical impact
- Supply-chain compromise
- Exploitation of deployed systems or users

When uncertain, prefer private reporting.

## What Can Be Reported Publicly

Ordinary security improvements may be discussed through public issues when they do not reveal a credible exploitable vulnerability.

Examples include:

- General dependency updates
- Hardening suggestions
- Safer defaults
- Additional validation
- Documentation improvements
- Defense-in-depth changes
- Static-analysis findings without a credible attack path
- Improvements to testing, logging, or monitoring
- Refactoring that reduces future security risk

If public discussion could reveal how to exploit a current weakness, report it privately instead.

## Information to Include

A useful report should include, when possible:

- The affected repository, component, branch, or version
- A clear description of the issue
- The expected security boundary
- The demonstrated or likely impact
- Steps to reproduce the issue
- A minimal proof of concept
- Relevant logs, screenshots, requests, or code
- Any conditions required for exploitation
- Suggested remediation, if known

Reports should distinguish confirmed behavior from assumptions or unverified possibilities.

Do not include unnecessary private data, credentials, or secrets.

## Safe and Non-Destructive Research

Security testing should be limited to what is necessary to demonstrate the issue.

Do not:

- Access, modify, delete, or retain data that does not belong to you
- Continue exploring private data after unauthorized access has been demonstrated
- Disrupt services or degrade availability
- Perform denial-of-service or high-volume load testing
- Damage, corrupt, or erase systems or data
- Establish persistence
- Deploy malware
- Use social engineering, phishing, or impersonation
- Target third-party infrastructure or services
- Test against systems you do not have permission to assess
- Publicly disclose working exploit details before coordinated disclosure

Use local environments, test instances, accounts you control, and minimal proofs of concept whenever possible.

If you unexpectedly encounter private data, credentials, secrets, or access beyond what is necessary to prove the issue:

1. Stop testing.
2. Do not retain, copy, use, or share the information.
3. Report the situation immediately through GitHub Private Vulnerability Reporting.
4. Explain what was accessed and how.

## Coordinated Disclosure

Reporters should keep credible non-public vulnerabilities confidential while the maintaining team investigates and prepares a response.

Public disclosure should be coordinated with the maintaining team.

Octacity does not require indefinite secrecy, but reporters are expected to provide a reasonable opportunity for investigation, remediation, release preparation, and user communication before publishing technical details.

The maintaining team may ask the reporter to delay disclosure when additional time is reasonably necessary to protect users or deployments.

## Review and Responsibility

The maintaining team of the affected repository is responsible for handling the report.

The team leader may:

- Review the report directly
- Delegate investigation to a team member
- Assign a repository maintainer
- Request assistance from a qualified member of another Octacity team
- Coordinate with relevant upstream projects or service providers

The maintaining team decides whether the report is valid, its severity, the appropriate remediation, and the disclosure process.

Security reports are handled according to the same accountability and review principles described in the Octacity [Contributing Guidelines](CONTRIBUTING.md).

## Response Times

Octacity does not guarantee fixed acknowledgment, investigation, or remediation deadlines.

Response time may depend on:

- Maintainer availability
- Project activity
- Technical complexity
- Severity and exploitability
- Access to affected systems
- Coordination with dependencies or external services

Maintaining teams should respond and communicate progress when reasonably possible.

## AI-Assisted and Automated Reports

AI-assisted analysis, scanners, fuzzers, and automated tools are allowed.

The reporter remains responsible for the submission and must:

- Verify that the issue is credible
- Understand the reported behavior
- Provide a useful reproduction or evidence
- Distinguish confirmed findings from generated speculation
- Respond personally to maintainer questions
- Avoid submitting large volumes of unverified output
- Follow the repository's rules and this security policy

Octacity expects to communicate with the accountable reporter, not with an autonomous agent.

Unverified scanner output, speculative AI-generated reports, and reports without a credible path may be closed without further investigation.

## Rewards and Recognition

Octacity does not operate a bug bounty program and does not offer financial rewards unless explicitly announced for a specific project or program.

Octacity may publicly acknowledge reporters of valid vulnerabilities, typically by GitHub username, unless they request anonymity.

Recognition may appear in:

- Repository release notes
- Security advisories
- Acknowledgment files
- Project documentation
- An organization-level contributor list

The form and location of recognition may vary, and public recognition is not guaranteed.

## Confidentiality

Information submitted through GitHub Private Vulnerability Reporting should remain limited to the people involved in investigating and resolving the issue.

Reporters should not share private report content, maintainer discussions, patches, or exploit details without coordination.

Maintainers should avoid sharing reporter information beyond what is necessary to handle the report.

## Out of Scope

The following are generally not treated as security vulnerabilities unless they demonstrate a credible security impact:

- Missing best practices without an exploitable consequence
- Dependency version reports without a relevant attack path
- Automated scan results without verification
- Self-XSS requiring a user to deliberately execute code against themselves
- Reports that rely entirely on unsupported or intentionally unsafe configurations
- Social engineering
- Physical attacks
- Denial-of-service testing without prior authorization
- Issues in third-party services outside Octacity's control
- Duplicate reports of an already known issue

Maintaining teams may define repository-specific scope.

## Good-Faith Reporting

Octacity values good-faith security research that follows this policy.

Reports made honestly, carefully, and without harmful or destructive behavior will be reviewed respectfully.

This policy does not authorize testing against systems, accounts, infrastructure, or data that you do not own or have permission to assess.

## Questions

When unsure whether an issue should be public or private, use GitHub Private Vulnerability Reporting.

If the affected repository does not have private vulnerability reporting enabled, contact its maintaining team through the safest available project channel without disclosing exploit details publicly.
