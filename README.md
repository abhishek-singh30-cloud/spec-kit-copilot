# spec-kit-copilot
Poc to deploy resources based on specification and using spec kit 
# Canary Spec-Driven Azure POC

This repository is a minimal proof of concept for deploying Azure resources using a specification-driven workflow.

## Scope
- Single repo
- Single environment: `canary`
- Resource group and virtual network created from a spec file
- GitHub Actions for validation and deployment
- Azure OIDC authentication
- Approval gate before deployment

## Source of truth
- `infra-spec.md`

## Workflow
1. Write/update the spec
2. Generate Terraform from the spec in the pipeline
3. Validate the generated code
4. Approve the deployment
5. Deploy to Azure using OIDC

## Notes
- No custom Terraform modules
- Use Azure Verified Modules where applicable
- Keep the POC minimal
