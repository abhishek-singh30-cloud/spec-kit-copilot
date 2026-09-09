# Canary Infrastructure Specification

## Goal
Deploy a minimal Azure canary environment using Terraform, Spec Kit, GitHub Actions, and Azure OIDC federation.

## Resources to create
1. Resource Group
   - Name: `rg-abhi01`
   - Region: `eastus`

2. Virtual Network
   - Name: `vnet-abhi01`
   - Region: `eastus`
   - Address space: `10.10.0.0/16`
   - No subnets for this POC

## Delivery requirements
- Terraform-based implementation
- Use Azure Verified Modules where applicable
- No long-lived Azure client secrets
- GitHub Actions validation and deployment
- Approval required before apply

## Notes
- This POC validates the spec-driven workflow, OIDC authentication, approval gating, and AVM consumption pattern.
