# Lab 4 - Hyper-V to Azure Migration with Azure Migrate

## Objective

Test a migration path for an existing Hyper-V virtual machine into Azure using Azure Migrate and replication-based migration.

## What I Built

- Hyper-V source VM for migration testing
- Azure resource group for migration resources
- Azure Migrate project
- Hyper-V host registration using the migration agent and registration key
- Replication configuration for the selected VM
- Migration to Azure after replication completed
- Post-migration cleanup steps

## Architecture Summary

This lab simulates a common modernization scenario:

- an existing on-premises Hyper-V VM
- Azure Migrate project for discovery and migration coordination
- replication from the Hyper-V environment into Azure
- migration cutover after the VM reaches a protected state

## Migration Workflow

1. Create a Hyper-V VM for testing
2. Create Azure migration resources
3. Download and install the required migration provider / agent
4. Register the Hyper-V host
5. Discover the VM
6. Configure replication settings
7. Monitor replication until protected
8. Perform migration to Azure
9. Review jobs and cleanup resources

## Why This Lab Matters

This lab demonstrates migration planning and execution concepts that matter in real environments:

- validating source readiness
- registering migration infrastructure correctly
- handling replication timelines
- understanding target network/resource design
- verifying post-migration state
- cleaning up temporary migration resources

## Validation Performed

- Confirmed Hyper-V host registration
- Confirmed server discovery in Azure Migrate
- Verified replication started successfully
- Monitored replication health and status
- Confirmed migration completed
- Verified Azure VM appeared after migration
- Reviewed migration job history and project overview

## Issues / Troubleshooting

Examples of troubleshooting areas documented in this lab:

- host registration delays
- discovery delays after registration
- internet/proxy/firewall issues blocking registration
- replication taking time to reach first recovery point
- target resource selection mistakes
- cleanup gaps after migration completion

## Security / Cost Notes

- Used a small source VM for lab purposes
- Chose low-cost target options where appropriate
- Treated migration tooling as temporary infrastructure and documented cleanup
- Kept security assumptions explicit because lab setup is often more permissive than production

## What I Learned

- Migration is not a single action; it is a workflow with discovery, registration, replication, cutover, and cleanup
- Replication timing and validation are critical
- Target design decisions such as network, subnet, region, and disk choices should be documented before migration starts

## Next Improvements

- Add an assessment phase before migration
- Compare test migration vs. final migration workflow
- Document rollback / fallback considerations
- Capture pre-migration and post-migration validation checklists
- Compare agent-based migration choices with alternative modernization paths
