# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] — 2026-03-25

### Added
- Active Directory as the on-prem identity source with structured OU hierarchy and governance attributes
- SailPoint IdentityIQ as the identity governance platform with Java and Apache Tomcat runtime
- AD connector configuration, identity aggregation, and provisioning integration
- Identity attribute mapping for governance-driven automation
- Joiner, Mover, and Leaver lifecycle event design and business process workflows
- Business roles aligned to departments with birthright-style access
- Workgroup ownership and delegated governance structure
- AD Connect / Microsoft Entra Connect for hybrid identity synchronisation
- Synced users and groups visible in Microsoft Entra ID
- LDAP, LDAPS, certificate, and Java truststore troubleshooting documentation
- SailPoint connector and IQService debugging documentation
- Tomcat runtime and HTTP 405 investigation documentation
- End-to-end access request, approval, provisioning, and AD group membership validation
- Comprehensive screenshots and architecture diagrams
- Full documentation suite (architecture, implementation, troubleshooting, validation, lessons learned)

### Infrastructure
- VMware-based multi-VM lab environment
- Dedicated VMs for AD, SailPoint IIQ, and AD Connect
- Microsoft Entra ID tenant for cloud identity layer

[1.0.0]: https://github.com/keyurp7/Metaverse-IAM-IGA-AD-Entra-Project/releases/tag/v1.0.0
