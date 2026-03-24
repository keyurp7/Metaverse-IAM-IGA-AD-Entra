<div align="center">

# Metaverse IAM Lab

**Enterprise Identity Governance & Hybrid Identity Environment**

A production-inspired Identity and Access Management environment built to demonstrate enterprise-grade capability across IAM systems architecture, identity governance engineering, access automation, platform support, and operational troubleshooting.

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project)](https://github.com/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project/commits/main)
[![GitHub stars](https://img.shields.io/github/stars/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project?style=social)](https://github.com/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project/stargazers)
[![GitHub repo size](https://img.shields.io/github/repo-size/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project)](https://github.com/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project)

[Documentation](#-documentation) · [Roadmap](ROADMAP.md) · [Contributing](CONTRIBUTING.md) · [Report an Issue](../../issues/new/choose)

</div>

---

## 📋 Table of Contents

- [Stack](#-stack)
- [Overview](#-overview)
- [Architecture](#-architecture)
- [Key Areas](#-key-areas)
- [End-to-End Validation](#-end-to-end-validation)
- [Documentation](#-documentation)
- [Skills Demonstrated](#-skills-demonstrated)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [Security](#-security)
- [Author](#-author)

---

## 🛠 Stack

| Technology | Role |
|---|---|
| **Active Directory** | On-prem source of truth |
| **SailPoint IdentityIQ** | Identity governance platform |
| **Microsoft Entra ID** | Cloud identity layer |
| **AD Connect / Entra Connect** | Hybrid identity sync |
| **Java & Apache Tomcat** | IIQ server runtime |

---

## 📖 Overview

This lab was built to reflect real enterprise IAM processes, not just product setup. It covers:

- Source-of-truth driven identity governance
- Joiner, Mover, and Leaver automation
- Role-based access control and business role design
- Workgroup ownership and access accountability
- Hybrid identity sync from AD to Entra ID
- Server runtime validation and connector support
- Troubleshooting across LDAP, LDAPS, certificates, Tomcat, and platform behaviour
- End-to-end access request and provisioning validation

---

## 🏗 Architecture

### Architecture Diagram

<img width="2392" height="742" alt="Metaverse IAM Architecture diagram" src="https://github.com/user-attachments/assets/b2c830ea-c202-482c-9888-aa04db055b92" />

### On-Prem Identity Source
- Active Directory hosted on Windows Server VMs
- OU structure for users, workstations, helpdesk, and governed identity containers
- Identity attributes such as `department` and `employeeType` used in governance logic

### Identity Governance Layer
- SailPoint IdentityIQ hosted on a dedicated VM
- Java and Apache Tomcat installed locally on the IIQ server
- AD onboarding, aggregation, identity mapping, provisioning, lifecycle events, workgroups, and role design

### Hybrid Identity Layer
- AD Connect / Microsoft Entra Connect hosted on a dedicated VM
- Sync from on-prem AD into Microsoft Entra ID via AD Connect

### Cloud Identity Layer
- Microsoft Entra ID for synced users, groups, and cloud identity visibility

---

## 🔑 Key Areas

### Identity Governance
- AD as source of truth
- Identity mapping in SailPoint IIQ
- AD connector configuration and provisioning integration
- Entitlement and role visibility
- Workgroup ownership and governance accountability

### JML Automation
- Joiner, Mover, and Leaver lifecycle events
- Business process workflow design for JML
- Attribute-driven access logic using `department` and `employeeType`
- Birthright and role-based provisioning

### Access Governance
- Business roles aligned to departments
- Birthright-style access design
- Delegated governance through workgroups and ownership
- Controlled access request and provisioning process

### Hybrid Identity
- On-prem AD sync into Entra ID through AD Connect
- Synced users and groups visible in Microsoft Entra ID
- Entra Connect health validation and sync troubleshooting

### Platform Support & Troubleshooting
- LDAP and LDAPS validation
- Certificate and Java truststore troubleshooting
- SailPoint connector debugging
- Tomcat runtime and application hosting validation
- HTTP 405 platform issue investigation
- Final validation through successful task execution and provisioning results

---

## ✅ End-to-End Validation

A full governed access flow was validated for a test identity:

1. Access request initiated in SailPoint IdentityIQ
2. Business role selection and submission
3. Request approval and provisioning completion
4. Provisioning engine execution
5. AD group membership updated after provisioning

> For detailed validation evidence, see [docs/validation.md](docs/validation.md).

---

## 📚 Documentation

| Document | Description |
|---|---|
| [Architecture](docs/architecture.md) | System layers and identity flow |
| [Implementation](docs/implementation.md) | Environment build and SailPoint configuration |
| [Screenshots](docs/screenshots.md) | Annotated evidence across all layers |
| [Troubleshooting](docs/troubleshooting.md) | LDAP, certs, connectors, Tomcat debugging |
| [Validation](docs/validation.md) | End-to-end access flow validation |
| [Lessons Learned](docs/lessons-learned.md) | Key takeaways from building the lab |

---

## 🧠 Skills Demonstrated

<table>
  <tr>
    <td>Identity and Access Management</td>
    <td>Identity Governance and Administration</td>
    <td>SailPoint IdentityIQ</td>
  </tr>
  <tr>
    <td>Active Directory</td>
    <td>Microsoft Entra ID</td>
    <td>AD Connect / Entra Connect</td>
  </tr>
  <tr>
    <td>JML Automation</td>
    <td>Role-Based Access Control</td>
    <td>Access Provisioning</td>
  </tr>
  <tr>
    <td>Workflow & Lifecycle Events</td>
    <td>Hybrid Identity</td>
    <td>LDAP & LDAPS Troubleshooting</td>
  </tr>
  <tr>
    <td>Certificates & Java Truststore</td>
    <td>Tomcat Application Hosting</td>
    <td>Platform Support & Debugging</td>
  </tr>
</table>

---

## 🗺 Roadmap

This project is actively evolving. Planned enhancements include SoD policies, certification campaigns, Okta integration, SIEM/PAM integration, and Zero Trust alignment.

👉 **[View the full Roadmap](ROADMAP.md)**

---

## 🤝 Contributing

Contributions, suggestions, and feedback are welcome. Whether it's a typo fix, a new lab scenario, or an architectural improvement — all input is valued.

👉 **[Read the Contributing Guide](CONTRIBUTING.md)**

---

## 🔒 Security

This is a lab environment — no production data or real credentials are involved. For security-related concerns about the repository itself, please see the security policy.

👉 **[Read the Security Policy](SECURITY.md)**

---

## 📝 Changelog

Track all changes, additions, and releases in the changelog.

👉 **[View the Changelog](CHANGELOG.md)**

---

## 👤 Author

**Keyur Purohit**
IAM Engineer · Melbourne, Australia

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/keyur-purohit)
[![Portfolio](https://img.shields.io/badge/Portfolio-keyurpurohitIAM-orange?style=flat&logo=google-chrome)](https://keyurp7.github.io/keyurpurohitIAM/)
[![Email](https://img.shields.io/badge/Email-Keyur__7%40outlook.com-red?style=flat&logo=microsoft-outlook)](mailto:Keyur_7@outlook.com)

---

<div align="center">

**If you find this project useful, consider giving it a ⭐**

It helps others discover it and motivates continued development.

</div>
