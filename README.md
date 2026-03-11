# Metaverse-IAM-IGA-AD-Entra

The Metaverse IAM Lab is a production-inspired Identity and Access Management environment built to demonstrate enterprise-grade capability across IAM systems architecture, identity governance engineering, access automation, platform support, and operational troubleshooting.

# Stack

- *Active Directory** as the on-prem source of truth
- *SailPoint IdentityIQ** as the identity governance platform
- *Microsoft Entra ID** as the cloud identity layer
- *AD Connect / Microsoft Entra Connect** for hybrid identity sync
- *Java and Apache Tomcat** installed locally on the IIQ server

# Overview

This lab was built to reflect real enterprise IAM processes, not just product setup. It covers:

- source-of-truth driven identity governance
- joiner, mover, and leaver automation
- role-based access control and business role design
- workgroup ownership and access accountability
- hybrid identity sync from AD to Entra ID
- server runtime validation and connector support
- troubleshooting across LDAP, LDAPS, certificates, Tomcat, and platform behavior
- end-to-end access request and provisioning validation

# Architecture

# On-Prem Identity Source

- Active Directory hosted on Windows Server VMs
- OU structure for users, workstations, helpdesk, and governed identity containers
- identity attributes such as department and employeeType used in governance logic

# Identity Governance Layer
- SailPoint IdentityIQ hosted on a dedicated VM
- Java and Apache Tomcat installed locally on the IIQ server
- AD onboarding, aggregation, identity mapping, provisioning, lifecycle events, workgroups, and role design

# Hybrid Identity Layer
- AD Connect / Microsoft Entra Connect hosted on a dedicated VM
- sync from on-prem AD into Microsoft Entra ID via AD Connect

# Cloud Identity Layer
- Microsoft Entra ID for synced users, groups, and cloud identity visibility

# Architecture Diagram

<img width="2392" height="742" alt="Metaverse IAM Architecture diagram" src="https://github.com/user-attachments/assets/b2c830ea-c202-482c-9888-aa04db055b92" />


# Key Areas

# Identity Governance
- AD as source of truth
- identity mapping in SailPoint IIQ
- AD connector configuration and provisioning integration
- entitlement and role visibility
- workgroup ownership and governance accountability

# JML Automation
- Joiner, Mover, and Leaver lifecycle events
- business process workflow design for JML
- attribute-driven access logic using department and employeeType
- birthright and role-based provisioning

# Access Governance
- business roles aligned to departments
- birthright-style access design
- delegated governance through workgroups and ownership
- controlled access request and provisioning process

# Hybrid Identity
- on-prem AD sync into Entra ID through AD Connect
- synced users and groups visible in Microsoft Entra ID
- Entra Connect health validation and sync troubleshooting

# Platform Support and Troubleshooting
- LDAP and LDAPS validation
- certificate and Java truststore troubleshooting
- SailPoint connector debugging
- Tomcat runtime and application hosting validation
- HTTP 405 platform issue investigation
- final validation through successful task execution and provisioning results

# End-to-End Validation

A full governed access flow was validated for a test identity:

1. access request initiated in SailPoint IdentityIQ
2. business role selection and submission
3. request approval and provisioning completion
4. provisioning engine execution
5. AD group membership updated after provisioning


This shows controlled access request, workflow-driven provisioning, and final entitlement assignment in the target system.

# Lifecycle Events
![Figure 8](assets/screenshots/08-lifecycle-events.png)

# JML Workflow Logic
![Figure 9](assets/screenshots/09-jml-workflow-logic.png)

# Business Role Model
![Figure 10](assets/screenshots/10-business-role-model.png)

# Workgroups and Ownership
![Figure 11](assets/screenshots/11-workgroups-and-owners.png)

# Access Request to Provisioning Validation
![Figure 12](assets/screenshots/12-access-request-initiation.png)
![Figure 13](assets/screenshots/13-role-selection-submission.png)
![Figure 14](assets/screenshots/14-request-completion.png)
![Figure 15](assets/screenshots/15-provisioning-engine-result.png)
![Figure 16](assets/screenshots/16-ad-membership-validation.png)

# Entra Visibility
![Figure 17](assets/screenshots/17-entra-users-sync-view.png)
![Figure 18](assets/screenshots/18-entra-groups-sync-view.png)
![Figure 19](assets/screenshots/19-entra-connect-health.png)

# Troubleshooting Evidence
![Figure 20](assets/screenshots/20-troubleshooting-collage.png)
![Figure 21](assets/screenshots/21-ldap-certificate-collage.png)

# Final Operational State
![Figure 22](assets/screenshots/22-final-outcomes-collage.png)

# Documentation

- [Architecture](docs/architecture.md)
- [Implementation](docs/implementation.md)
- [Screenshots](docs/screenshots.md)
- [Troubleshooting](docs/troubleshooting.md)
- [Validation](docs/validation.md)
- [Lessons Learned](docs/lessons-learned.md)

# Skills Demonstrated

- Identity and Access Management
- Identity Governance and Administration
- SailPoint IdentityIQ
- Active Directory
- Microsoft Entra ID
- AD Connect / Entra Connect
- JML Automation
- Role-Based Access Control
- Access Provisioning
- Workflow and Lifecycle Events
- Hybrid Identity
- LDAP and LDAPS Troubleshooting
- Certificates and Java Truststore Validation
- Tomcat Application Hosting
- Platform Support and Debugging


# Author
  KP  
IAM Engineer
