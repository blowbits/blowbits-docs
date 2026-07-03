---
title: PATCH & SECURITY UPDATE PROCEDURE
company: Blowbits Solutions LLP
classification: Internal
---

# 1. Purpose

This Standard Operating Procedure (SOP) defines the process for identifying, evaluating, testing, approving and deploying security patches and software updates for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective is to ensure that security vulnerabilities are addressed in a timely manner while maintaining the stability, availability and security of production services.

# 2. Scope

This procedure applies to all production systems supporting the GSP platform, including:

- Cloud infrastructure
- Linux operating systems
- Network and firewall appliances
- Application servers
- Databases
- Containers
- Runtime frameworks
- Third-party software components

# 3. Patch Identification

Security updates may be identified through:

- Software vendor security advisories.
- Cloud service provider notifications.
- Operating system security updates.
- CERT-In advisories.
- GSTN communications.
- Vulnerability Assessment and Penetration Testing (VAPT).
- Internal security reviews.
- Operational monitoring.

# 4. Patch Assessment

Each identified update shall be evaluated to determine:

- Systems affected.
- Security impact.
- Business impact.
- Compatibility with existing applications.
- Potential operational risks.
- Recommended deployment priority.

# 5. Patch Testing

Where practical, security updates shall be verified in a non-production environment before deployment.

Testing may include:

- Application functionality.
- API validation.
- Database connectivity.
- Service availability.
- Performance verification.

Critical security updates may be deployed directly to production where immediate remediation is necessary.

# 6. Patch Deployment

Following successful evaluation, authorised personnel shall deploy approved updates using established operational procedures.

Deployment activities may include:

- Scheduled maintenance windows.
- Service restart or configuration reload.
- Operational verification.
- Functional validation.
- Post-deployment monitoring.

# 7. Emergency Security Updates

Where critical vulnerabilities present a significant security risk, emergency patching may be performed on an expedited basis.

Emergency updates shall be reviewed after deployment to ensure service stability and appropriate corrective actions, where necessary.

# 8. Verification

Following deployment, authorised personnel shall verify:

- Successful installation.
- Service availability.
- Application functionality.
- Security monitoring.
- Overall system health.

Any issues identified shall be investigated and resolved promptly.

# 9. Documentation

Supporting operational records, system logs and other technical evidence may be maintained, as appropriate, in accordance with operational requirements.

# 10. Review

This procedure shall be reviewed annually or whenever significant changes occur to the production environment or patch management process.

## Standard Statement

Blowbits Solutions LLP follows a structured patch and security update process to identify, evaluate, test, deploy and verify security updates for the GST Suvidha Provider (GSP) platform. Security updates are applied in a timely manner based on operational requirements and assessed risk, and supporting technical evidence is maintained through operational records and system logs.
