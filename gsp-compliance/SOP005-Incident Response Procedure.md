---
title: INCIDENT RESPONSE PROCEDURE
company: Blowbits Solutions LLP
classification: Internal
revision: "1.1"
last_update_date: 2026-02-10
---

# 1. Purpose

This Standard Operating Procedure (SOP) defines the process for identifying, reporting, assessing, escalating, responding to and closing information security incidents affecting the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of this procedure is to ensure that security incidents are managed in a timely and controlled manner to minimise operational impact, protect GSP services and satisfy applicable regulatory, contractual and organisational requirements.

# 2. Scope

This procedure applies to security incidents affecting applications, APIs, infrastructure, networks, operational processes, taxpayer information and supporting services associated with the Blowbits Solutions LLP GSP platform.

Operational records, communication records and supporting evidence generated during incident management are maintained separately.

# 3. Roles & Responsibilities

Incident response activities shall be performed by authorised internal roles defined in the Roles, Responsibilities & Access Matrix.

| Role | Incident Response Responsibility |
| ---- | -------------------------------- |
| **All Personnel** | Report suspected security incidents promptly through established reporting channels. |
| **Information Security Lead** | Assess, classify, investigate and contain security incidents; preserve relevant security evidence; coordinate security remediation. |
| **Platform Operations Lead** | Support containment, recovery, service restoration, platform validation and operational remediation. |
| **GSP Coordination Lead** | Coordinate GSTN communication and other authorised external communication relating to GSP operations where applicable. |
| **GSP Governance Lead** | Provide oversight for significant incidents; approve major response decisions, exceptions and closure where required. |

Where statutory cyber incident reporting is required, the GSP Coordination Lead shall coordinate the notification with the GSP Governance Lead unless a separate authorised reporting coordinator is assigned in the Contact Directory.

# 4. Incident Categories

Information security incidents may include, but are not limited to:

- Unauthorised access or attempted unauthorised access.
- Suspected credential compromise.
- Malware, ransomware or malicious code.
- Data exposure, data loss or unauthorised disclosure.
- Application, API or infrastructure vulnerability exploitation.
- Service disruption affecting GSP operations.
- Security monitoring alerts requiring investigation.
- Policy, access or configuration violations with security impact.

# 5. Severity Classification

Incidents shall be classified based on operational impact, security impact, data sensitivity, scope and regulatory relevance.

| Severity | Description | Expected Handling |
| -------- | ----------- | ----------------- |
| **Critical** | Confirmed or highly likely compromise affecting taxpayer information, production GSP services, external reporting obligations or major service availability. | Immediate Information Security Lead and Platform Operations Lead action, GSP Governance Lead notification and external notification assessment. |
| **High** | Significant security event affecting production systems, privileged access, sensitive information or service integrity. | Prompt investigation, containment planning and management escalation where required. |
| **Medium** | Security event with limited impact, controlled exposure or localised operational effect. | Documented investigation and remediation through normal operational procedures. |
| **Low** | Minor event, suspicious activity or policy deviation with no confirmed impact. | Record, review and close after appropriate validation. |

# 6. Incident Response Procedure

## Step 1 – Identification

A suspected information security incident shall be identified through monitoring activities, operational observations, user reports, GSTN communication, external notification, vulnerability assessment, cloud provider notification or other trusted sources.

## Step 2 – Reporting

The identified incident shall be reported to the Information Security Lead.

The initial report should include available details such as:

- Date and time of detection.
- Reporting person or source.
- Nature of the incident.
- Systems, services or information affected.
- Current status and observed impact.
- Immediate actions already taken.

## Step 3 – Assessment & Classification

The Information Security Lead shall assess the incident to determine:

- Incident category.
- Systems, services or information affected.
- Operational impact.
- Security impact.
- Potential regulatory or contractual reporting relevance.
- Severity and response priority.

## Step 4 – Escalation and Notification

Incidents shall be escalated according to severity and reporting requirements.

The normal escalation sequence is:

1. Information Security Lead.
2. Platform Operations Lead, where operational containment or recovery is required.
3. GSP Governance Lead, for significant incidents or major response decisions.
4. GSP Coordination Lead, where GSTN or external GSP communication may be required.
5. GSTN Coordination Contact, CERT-In Reporting Channel, customers or other authorised external communication points, where applicable.

External notifications shall be made only through authorised roles and communication channels listed in the Contact Directory.

## Step 5 – Containment

Appropriate containment measures shall be implemented to minimise further impact.

Containment activities may include:

- Restricting access.
- Isolating affected systems.
- Disabling compromised accounts or credentials.
- Blocking malicious activity.
- Preserving relevant logs and evidence.
- Applying temporary compensating controls.

## Step 6 – Investigation and Root Cause Analysis

The Information Security Lead shall investigate the incident to determine root cause where practicable, with support from the Platform Operations Lead where operational systems or recovery activities are involved.

Investigation activities may include:

- Reviewing application, infrastructure, access and security logs.
- Identifying affected systems, accounts, APIs, data or services.
- Determining timeline and scope.
- Assessing whether sensitive information or taxpayer information was affected.
- Identifying corrective and preventive actions.

## Step 7 – Recovery

Recovery activities shall be performed using approved operational procedures.

Activities may include:

- Restoring affected services.
- Rebuilding or reconfiguring affected components.
- Rotating credentials or keys where required.
- Applying patches or configuration changes.
- Validating service availability.
- Confirming operational stability.
- Monitoring post-recovery operations.

## Step 8 – Corrective and Preventive Actions

Corrective and preventive actions shall be identified based on investigation findings.

Actions may include:

- Access removal or modification.
- Configuration changes.
- Patch deployment.
- Monitoring rule updates.
- Procedure updates.
- User or administrator awareness actions.
- Follow-up vulnerability assessment or validation.

## Step 9 – Closure

Following containment, recovery and corrective action planning:

- Incident records shall be updated.
- Required communication records shall be retained.
- Root cause shall be documented where practicable.
- Corrective and preventive actions shall be tracked to closure where applicable.
- Significant incidents shall be closed after GSP Governance Lead review or approval.

# 7. Communication Responsibilities

| Communication Type | Responsible Role |
| ------------------ | ---------------- |
| Internal incident reporting | All Personnel |
| Security investigation updates | Information Security Lead |
| Operational recovery updates | Platform Operations Lead |
| Governance escalation | Information Security Lead |
| GSTN communication | GSP Coordination Lead |
| CERT-In reporting, where applicable | GSP Coordination Lead with GSP Governance Lead oversight, unless separately assigned |
| Customer or stakeholder communication, where applicable | GSP Governance Lead or authorised delegate |

# 8. Contact Directory

Current internal role assignments, phone numbers, email addresses, alternates and external contact channels are maintained in the Contact Directory.

Incident responders shall use the Contact Directory for current contact details and shall not rely on outdated copies of procedures for names, phone numbers or email addresses.

# 9. Incident Records and Evidence

The following records may be maintained, where applicable:

- Incident Report.
- Investigation notes.
- Log extracts or monitoring evidence.
- Root Cause Analysis.
- Corrective and Preventive Action Record.
- External Communication Record.
- Incident Closure Record.
- Management review or approval evidence.

Incident reports should include:

- Date and time of detection.
- Reporting source.
- Nature and category of the incident.
- Severity classification.
- Systems, services or information affected.
- Business, operational and security impact.
- Containment measures implemented.
- Recovery actions completed.
- Corrective and preventive actions.
- External notifications made, where applicable.
- Closure approval, where required.

# 10. Review and Testing

This procedure shall be reviewed annually or whenever significant operational, organisational, regulatory or technical changes occur.

Incident response readiness may be validated through tabletop exercises, incident simulations, post-incident reviews or management review of incident records.

# 11. Compliance

Compliance with this procedure is supported through documented operational records, incident records, communication records, system logs and implementation evidence maintained in accordance with organisational procedures.

Where applicable, regulatory, contractual or GSTN notification requirements shall be followed through authorised communication channels.

# Reference Documents

- POL-012 – Incident Response Policy
- Roles, Responsibilities & Access Matrix
- Contact Directory

# Revision History

| Date | Revision | Change Summary |
| ---- | -------- | -------------- |
| 2025-11-20 | 1.0 | Initial release of the incident response procedure. |
| 2026-02-10 | 1.1 | Added severity classification, escalation sequence, communication responsibilities and incident evidence expectations. |
