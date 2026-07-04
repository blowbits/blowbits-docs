---
title: PATCH & SECURITY UPDATE PROCEDURE
company: Blowbits Solutions LLP
classification: Internal
revision: "1.2"
last_update_date: 2026-03-10
logo: ../assets/octa-gst-logo.png
---

# 1. Purpose

This Standard Operating Procedure (SOP) defines the process for identifying, evaluating, testing, approving and deploying security patches and software updates for the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective is to ensure that security vulnerabilities are addressed in a timely manner while maintaining the stability, availability and security of production services.

# 2. Scope

This procedure applies to all production systems supporting the GSP platform, including:

- Cloud infrastructure.
- Linux operating systems.
- Network and firewall appliances.
- Application servers.
- Databases.
- Containers.
- Runtime frameworks.
- Third-party software components.

# 3. Roles & Responsibilities

Patch and security update activities shall be performed by authorised internal roles defined in the Roles, Responsibilities & Access Matrix.

| Role | Patch & Security Update Responsibility |
| ---- | -------------------------------------- |
| **Information Security Lead** | Review security advisories, assess security impact, assign priority and track security update closure. |
| **Platform Operations Lead** | Evaluate compatibility, test, deploy and validate approved patches and security updates. |
| **GSP Governance Lead** | Review significant patching risks, approve delayed patching, risk acceptance or emergency update decisions where required. |

# 4. Patch Identification

Security updates may be identified through:

- Software vendor security advisories.
- Cloud service provider notifications.
- Operating system security updates.
- CERT-In advisories.
- GSTN communications.
- Vulnerability Assessment and Penetration Testing (VAPT).
- Internal security reviews.
- Operational monitoring.

The following advisory sources shall be reviewed where relevant to the GSP platform:

- Debian Security Advisories: https://www.debian.org/security/
- AWS Security Bulletins: https://aws.amazon.com/security/security-bulletins/
- CERT-In: https://www.cert-in.org.in
- GST Advisory and Releases: https://services.gst.gov.in/services/advisory/advisoryandreleases

Security advisory sources relevant to the GSP platform shall be reviewed at least monthly. Critical advisories, urgent vendor notifications, cloud provider alerts, CERT-In advisories or GSTN communications shall be reviewed when received or identified.

# 5. Patch Assessment

Each identified update shall be evaluated to determine:

- Systems affected.
- Security impact.
- Business impact.
- Compatibility with existing applications.
- Potential operational risks.
- Recommended deployment priority.

Patch deployment priority shall be aligned with vulnerability severity and remediation targets defined in the Vulnerability Management Policy and Vulnerability Assessment & Remediation Procedure.

| Priority | Expected Handling |
| -------- | ----------------- |
| **Critical** | Immediate review and expedited deployment or compensating control. |
| **High** | Deploy within the applicable high-risk remediation target where feasible. |
| **Medium** | Deploy within planned maintenance or the applicable medium-risk remediation target. |
| **Low** | Deploy through planned maintenance or periodic update activity. |

# 6. Patch Testing

Where practical, security updates shall be verified in a non-production environment before deployment.

Testing may include:

- Application functionality.
- API validation.
- Database connectivity.
- Service availability.
- Performance verification.

Critical security updates may be deployed directly to production where immediate remediation is necessary.

# 7. Approval and Deployment

Following successful evaluation, authorised personnel shall deploy approved updates using established operational procedures.

Security updates affecting production systems shall follow applicable change management requirements. Emergency security updates may follow expedited approval and post-implementation review where immediate remediation is required.

Deployment activities may include:

- Scheduled maintenance windows.
- Service restart or configuration reload.
- Operational verification.
- Functional validation.
- Post-deployment monitoring.

# 8. Delayed or Exception Handling

Where a security update cannot be applied within the applicable target timeframe due to compatibility, stability or operational constraints, the reason shall be documented.

Compensating controls, delayed deployment or risk acceptance shall be reviewed by the Information Security Lead and approved by the GSP Governance Lead where required.

# 9. Emergency Security Updates

Where critical vulnerabilities present a significant security risk, emergency patching may be performed on an expedited basis.

Emergency updates shall be reviewed after deployment to ensure service stability and appropriate corrective actions, where necessary.

# 10. Verification

Following deployment, authorised personnel shall verify:

- Successful installation.
- Service availability.
- Application functionality.
- Security monitoring.
- Overall system health.

Any issues identified shall be investigated and resolved promptly.

# 11. Documentation and Evidence

Supporting operational records, system logs and other technical evidence may be maintained, as appropriate, in accordance with operational requirements.

Evidence may include:

- Security advisory, update notice or vulnerability reference.
- Patch impact assessment.
- Test or compatibility validation evidence.
- Change or deployment record.
- Post-deployment verification evidence.
- Exception, delayed deployment or risk acceptance approval where applicable.
- Emergency update review record where applicable.

# 12. Review

This procedure shall be reviewed annually or whenever significant changes occur to the production environment or patch management process.

# 13. Compliance

Compliance with this procedure is supported through documented patch records, change records, validation evidence, exception approvals and implementation evidence maintained in accordance with organisational procedures.

# Reference Documents

- Vulnerability Management Policy
- Vulnerability Assessment & Remediation Procedure
- Change Management Procedure
- Roles, Responsibilities & Access Matrix

# Revision History

| Date | Revision | Change Summary |
| ---- | -------- | -------------- |
| 2025-11-21 | 1.0 | Initial release of the patch and security update procedure. |
| 2026-02-16 | 1.1 | Aligned patch handling with vulnerability severity, remediation targets and change management. |
| 2026-03-10 | 1.2 | Added security advisory sources and monthly advisory review cadence. |
