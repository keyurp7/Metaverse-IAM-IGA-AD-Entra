# Implementation

# Environment Build

The lab was built on a VM-based setup to reflect a real enterprise IAM environment.

# Runtime Foundation

- Active Directory hosted on Windows Server VM
- SailPoint IdentityIQ hosted on dedicated VM
- Java and Apache Tomcat installed locally on IIQ server
- AD Connect hosted on separate VM

# SailPoint Build Areas
- Active Directory application onboarding
- connector validation and IQService support
- account aggregation and identity correlation
- identity attribute mapping
- lifecycle event creation for Joiner, Mover, and Leaver
- business process configuration for JML workflows
- business roles and governed access structure
- workgroups and ownership for delegated governance

# Hybrid Identity Build Areas
- AD Connect installation and sync configuration
- synced users and groups visible in Entra ID
- Entra Connect health monitoring and validation

# Result

The implementation produced a working IAM model covering identity governance, automation, hybrid sync, server runtime support, and target-system provisioning validation.
