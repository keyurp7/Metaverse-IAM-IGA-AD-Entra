# Security Policy

## About This Project

The Metaverse IAM Lab is a **demonstration and portfolio project**. It is not a production system and does not process real user data. All credentials, identities, and configurations shown in screenshots and documentation are from an isolated lab environment.

---

## 🔐 Security Principles

This project follows IAM security best practices even in a lab context:

| Principle | How It's Applied |
|---|---|
| **Least Privilege** | Business roles grant only the minimum entitlements required for each department |
| **Separation of Duties** | Workgroup ownership separates who requests access from who approves it |
| **Governance-Led Access** | All access is assigned through governed workflows, never direct assignment |
| **Source-of-Truth Integrity** | Identity attributes originate from AD — governance decisions depend on clean source data |
| **Audit Trail** | SailPoint IIQ maintains provisioning history, approval records, and task execution logs |
| **Defence in Depth** | Multiple layers — AD, IIQ governance, Entra ID conditional access — provide overlapping controls |

---

## 🛡 Repository Security Measures

### Secret Scanning
This repository has GitHub secret scanning enabled. Any accidentally committed secrets (API keys, tokens, credentials) will trigger an alert.

### Dependency Management
[Dependabot](https://docs.github.com/en/code-security/dependabot) is configured to monitor for vulnerable dependencies and automatically raise pull requests for updates.

### Code Ownership
A [CODEOWNERS](.github/CODEOWNERS) file ensures that all changes to critical files require review from the project maintainer.

### Branch Protection (Recommended)
For production use, enable branch protection on `main`:
- Require pull request reviews before merging
- Require status checks to pass
- Restrict who can push directly to `main`

---

## 🔒 Lab Environment Security

| Control | Detail |
|---|---|
| **Network Isolation** | Lab VMs run on an isolated virtual network with no public internet exposure |
| **Credential Scope** | All credentials are lab-only and have no access to production systems |
| **Certificate Management** | LDAPS certificates are self-signed and scoped to the lab domain only |
| **Java Truststore** | Truststore entries are limited to lab CA certificates |
| **Screenshot Redaction** | Sensitive values (passwords, connection strings) are not visible in published screenshots |
| **No Production Data** | All identity data is synthetic — no real employee or customer data is used |

---

## ⚠️ Reporting a Vulnerability

If you discover a security concern within this repository — for example, accidentally exposed credentials, sensitive configuration data, or documentation that could mislead someone into an insecure setup — please report it responsibly.

### How to Report

1. **Do not** open a public issue for security concerns
2. **Email** [Keyur_7@outlook.com](mailto:Keyur_7@outlook.com) with a description of the concern
3. Include the file path, line number, or screenshot if applicable
4. I will acknowledge your report within **72 hours** and work to resolve it promptly

### What Happens Next

1. I will acknowledge receipt and confirm the issue
2. I will investigate and determine the impact
3. A fix will be committed, and you will be credited (unless you prefer anonymity)
4. If applicable, a security advisory will be published on the repository

---

## 📋 Scope

| In Scope | Out of Scope |
|---|---|
| Exposed credentials or secrets in repo files | Vulnerabilities in third-party products (SailPoint, Entra ID, etc.) |
| Sensitive data visible in screenshots | General IAM design opinions or preferences |
| Misleading security guidance in docs | Issues in lab VMs (not publicly accessible) |
| `.gitignore` gaps that could leak secrets | Theoretical attacks against the lab network |

---

## ✅ Supported Versions

| Version | Supported |
|---|---|
| v1.x (current) | ✅ Active |
| < v1.0 | ❌ No longer maintained |

---

## 📜 Security-Related Documentation

- [Troubleshooting — LDAP, LDAPS, and Certificate Validation](docs/troubleshooting.md)
- [Architecture — Defence in Depth Layers](docs/architecture.md)
- [Validation — End-to-End Governed Access Proof](docs/validation.md)

---

## 🏷 Disclaimer

This lab environment runs on isolated virtual machines that are not publicly accessible. Any credentials, hostnames, or configuration values visible in documentation or screenshots are specific to this lab and carry no risk to production systems. This project is intended for educational and portfolio purposes only.
