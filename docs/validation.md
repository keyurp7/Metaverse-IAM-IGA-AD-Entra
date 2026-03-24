# Validation

## Overview

The Metaverse IAM Lab was validated end to end to confirm that the full governed access lifecycle works as designed — from identity creation through to provisioned access in the target system.

## What Was Validated

| Layer | Validation |
|---|---|
| **Identity Source** | AD identity attributes (department, employeeType) correctly populated and available for governance logic |
| **Aggregation** | SailPoint IIQ successfully aggregated identities and entitlements from Active Directory |
| **Identity Mapping** | Correlation rules correctly mapped AD accounts to IIQ identity cubes |
| **Lifecycle Events** | Joiner, Mover, and Leaver events triggered correctly based on attribute changes |
| **Workflow Execution** | BP_JML_Joiner workflow executed successfully, assigning birthright entitlements |
| **Role Assignment** | Business roles aligned to departments and assigned through governed process |
| **Access Request** | End-to-end access request initiated and submitted in SailPoint IIQ |
| **Approval** | Request approved through the configured approval workflow |
| **Provisioning** | Provisioning engine committed role and group updates to Active Directory |
| **Target System** | AD group membership confirmed after provisioning |
| **Hybrid Sync** | Synced users and groups visible in Microsoft Entra ID via AD Connect |
| **Sync Health** | Entra Connect health monitoring confirmed healthy sync state |

## End-to-End Access Flow

The following flow was validated for a test identity:

1. Access request initiated in SailPoint IdentityIQ
2. Business role selected and submitted for approval
3. Request approved through the governance workflow
4. Provisioning engine executed and committed changes
5. Active Directory group membership updated to reflect the provisioned access

## Evidence

Detailed screenshots demonstrating each validation step are available in the [Screenshots](screenshots.md) documentation:

- **Figure 9C** — Joiner workflow execution with birthright role assignment
- **Figure 10** — Business role and entitlement structure
- **Figure 12–15** — Hybrid identity sync and Entra ID visibility
- **Figure 22–25** — Final access request, approval, provisioning, and AD group membership validation
- **Figure 19** — Provisioning engine result showing committed updates
- **Figure 20** — Active Directory group membership after provisioning

## Key Takeaway

The lab demonstrates a complete governed access lifecycle — not just configuration and setup, but real, verifiable outcomes in the target system. This is the strongest form of IAM lab validation: proof that governed decisions translate into enforced access state.
