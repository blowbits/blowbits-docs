---
title: ANNEXURE C - INFRASTRUCTURE SECURITY & OPERATIONAL CONTROLS
company: Blowbits Solutions LLP
classification: Internal
---

**Prepared for:** GSTN GSP Security Assessment

# 1. Purpose

This annexure describes the infrastructure security framework and operational controls implemented to support the Blowbits Solutions LLP GST Suvidha Provider (GSP) platform.

The objective of these controls is to provide a secure production environment, protect infrastructure from unauthorised access, maintain service availability and support reliable platform operations.

# 2. Infrastructure Overview

The Blowbits GSP platform operates within a controlled production infrastructure designed to support secure service delivery, logical separation of operational components and resilient platform operations.

Infrastructure components are organised into distinct operational layers to support security, availability and administrative control.

## 2.1 Infrastructure Scope

This annexure describes infrastructure security, network protection, host security and operational monitoring.

Logical architecture, identity management, API security, cryptographic controls, data protection, logging, backup, business continuity and governance processes are documented separately within their respective annexures.

## 2.2 Infrastructure Interaction Model

```text
          Authorised Network Access
                     │
                     ▼
        Network Security Controls
                     │
                     ▼
        Application Services Layer
                     │
                     ▼
          Secure Data Services
                     │
                     ▼
      Monitoring & Administration
```

# 3. Network Security

Network security controls regulate communication between authorised users, the GSP platform and supporting infrastructure.

## 3.1 Perimeter Protection

Network access is restricted to authorised service endpoints required for platform operations.

Security controls regulate inbound and outbound communication and protect the production environment from unauthorised network access.

## 3.2 Network Segmentation

Infrastructure components are logically separated according to their operational function.

Communication between infrastructure segments is controlled in accordance with operational and security requirements.

# 4. Host Security

Production systems are maintained using secure baseline configurations designed to reduce operational risk.

## 4.1 Secure System Configuration

Production systems are configured to minimise the operational footprint by restricting active software and services to those required for platform operation.

## 4.2 Administrative Access

Administrative access to production infrastructure is restricted to authorised personnel through controlled administrative processes.

Administrative activities are performed using secure management mechanisms and are subject to administrative oversight.

# 5. Platform Monitoring

Continuous monitoring supports operational visibility, infrastructure health and service reliability.

## 5.1 Infrastructure Monitoring

Platform availability, infrastructure health and operational status are continuously monitored.

Operational alerts support timely identification and investigation of infrastructure events.

## 5.2 Infrastructure Resilience

The infrastructure incorporates redundancy features intended to mitigate service disruption during standard operational activities and component-level events.

Where required, individual infrastructure components may be isolated for investigation without affecting the overall infrastructure security framework.

# 6. Infrastructure Principles

The infrastructure security framework is based on the following principles.

- Infrastructure components are logically separated according to operational function.
- Network communication is restricted to authorised pathways.
- Production systems operate using secure baseline configurations.
- Administrative access is restricted to authorised personnel.
- Infrastructure health is continuously monitored.
- Operational controls support reliable service delivery.

# 7. Infrastructure Control Characteristics

| Control Characteristic      | Description                                                                          |
| --------------------------- | ------------------------------------------------------------------------------------ |
| Network Protection          | Network communication is restricted to authorised pathways.                          |
| Infrastructure Segmentation | Infrastructure components are logically separated according to operational function. |
| Secure System Configuration | Production systems operate using approved baseline configurations.                   |
| Administrative Control      | Administrative access is restricted and controlled.                                  |
| Infrastructure Monitoring   | Infrastructure health and operational status are continuously monitored.             |
| Infrastructure Resilience   | Operational controls support reliable and resilient service delivery.                |

## Document Relationship

This annexure defines the infrastructure security and operational control framework of the Blowbits GSP platform.

Logical architecture, identity management, API security, cryptographic controls, data protection, logging, backup, business continuity and governance processes are documented separately within the relevant annexures and supporting operational documents.
