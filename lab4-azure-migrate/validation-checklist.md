# Validation Checklist

## Pre-Migration
- [ ] Hyper-V VM created and running
- [ ] VM settings documented
- [ ] Azure resource group created
- [ ] Azure Migrate project created
- [ ] Target region confirmed
- [ ] Target VNet and subnet prepared

## Registration / Discovery
- [ ] Migration provider / agent downloaded
- [ ] Registration key downloaded
- [ ] Agent installed on Hyper-V host
- [ ] Hyper-V host registration completed
- [ ] Host visible in Azure Migrate
- [ ] Source VM discovered

## Replication
- [ ] Replication settings configured
- [ ] Resource group selected
- [ ] Target network selected
- [ ] OS type confirmed
- [ ] Disk type selected
- [ ] Replication started successfully
- [ ] Replication status monitored
- [ ] VM reached protected state

## Migration
- [ ] Migration initiated
- [ ] Job completed successfully
- [ ] Azure VM visible in portal
- [ ] Basic post-migration validation completed

## Evidence Captured
- [ ] Project overview screenshot
- [ ] Replication status screenshot
- [ ] Job history screenshot
- [ ] Azure VM screenshot
- [ ] Cleanup evidence recorded

## Cleanup
- [ ] Replication stopped
- [ ] Temporary resources removed
- [ ] Cost review completed
