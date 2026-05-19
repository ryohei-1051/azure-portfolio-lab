# Azure Hybrid Infrastructure Labs

This repository documents my hands-on Azure lab work across hybrid networking, file services, serverless compute, and VM migration.

The goal of this repo is not just to show that I completed guided labs, but to document how I deployed, validated, troubleshot, and improved each solution from an infrastructure and operations perspective.

## Lab Scope

| Lab | Focus Area | Core Services / Technologies | What It Demonstrates |
|----|----|----|----|
| Lab 1 | Hybrid networking | Azure Virtual Network, VPN Gateway, Local Network Gateway, RRAS, Private DNS, Windows Server, Windows 11 | Site-to-site connectivity, routing, DNS, hybrid design |
| Lab 2 | Storage solutions | Azure Storage Account, Azure Files, Azure File Sync, Entra ID, Windows Server, Windows 11 | Hybrid file services, sync, share access, snapshot testing |
| Lab 3 | Serverless compute | Azure Functions, Cosmos DB, Storage Account Static Website | Frontend/backend integration, serverless app hosting, NoSQL basics |
| Lab 4 | Migration | Azure Migrate, Hyper-V, replication, migration validation | Discovery, replication, migration workflow, modernization planning |

## Repository Goals

- Document each lab in my own words
- Capture validation steps and screenshots
- Record issues encountered and troubleshooting performed
- Add security, cost, and production-minded improvement notes
- Expand guided labs into stronger personal portfolio projects

## Skills Demonstrated

- Azure hybrid infrastructure design
- Azure storage and synchronization
- Serverless application deployment
- Migration planning and execution
- Validation and troubleshooting
- Operational documentation
- Cost-conscious lab deployment and cleanup

## Repo Structure

- `lab1-hybrid-networking/` - hybrid Azure networking with VPN and DNS
- `lab2-azure-files-sync/` - Azure Files and Azure File Sync
- `lab3-serverless-todo/` - Azure Functions + Cosmos DB TO-DO app
- `lab4-azure-migrate/` - Hyper-V to Azure migration workflow
- `docs/` - shared screenshots, diagrams, cleanup, cost, and security notes

## Notes

- Original course materials are not included in this public repo.
- All documentation here is rewritten in my own words.
- Sensitive values such as keys, connection strings, account names, and public IP details should be sanitized before upload.

## Future Improvements

- Add Bicep or Azure CLI deployment notes
- Add PowerShell validation scripts
- Add network/security hardening notes
- Add production-vs-lab design comparisons
- Expand selected labs into deeper standalone projects
