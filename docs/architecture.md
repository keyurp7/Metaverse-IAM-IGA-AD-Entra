# Architecture

# Overview

The Metaverse IAM Lab is a hybrid IAM environment built to show how identity systems interact across on-prem directory services, governance platforms, and cloud identity layers.

# Core Components

# Active Directory
- primary source of truth for identity data
- hosted on Windows Server VM
- structured OU hierarchy and test identities
- governance-driving attributes such as department and employeeType

# SailPoint IdentityIQ
- hosted on a dedicated VM
- Java and Apache Tomcat installed locally on the IIQ server
- responsible for aggregation, identity mapping, lifecycle events, provisioning, role governance, and access request workflows

# AD Connect / Microsoft Entra Connect
- hosted on a dedicated VM
- synchronizes on-prem identities and groups into Microsoft Entra ID

# Microsoft Entra ID
- cloud identity layer
- receives synced users and groups
- supports hybrid identity visibility and authentication-aligned flows

# Identity Flow

1. identity originates in Active Directory
2. SailPoint aggregates and maps identity data
3. lifecycle events and workflow logic evaluate access decisions
4. approved requests trigger provisioning actions
5. AD Connect synchronizes relevant identities into Entra ID

# Design Principles

- source-of-truth driven IAM
- governance-led access assignment
- hybrid identity visibility
- production-style runtime design
- repeatable validation and troubleshooting support
