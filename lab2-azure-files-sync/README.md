# Lab 2 - Azure Files and Azure File Sync

## Objective

Evaluate Azure Files and Azure File Sync as a cloud-backed alternative to a traditional on-premises file server.

## What I Built

- On-premises-style domain environment
- Entra ID admin user for Azure-side administration
- Azure Storage Account
- Azure File Share
- Azure File Sync service
- Sync group and server endpoint
- Mapped file share from a Windows client
- Snapshot-based recovery test

## Architecture Summary

This lab connects cloud file storage with local server-based access:

- Azure Files provides centralized cloud storage
- Azure File Sync links the Azure file share to a Windows server
- Users can access files locally through SMB while data stays aligned with Azure
- Snapshots provide point-in-time recovery capability

## Why This Lab Matters

This lab demonstrates practical hybrid storage concepts:

- cloud-backed SMB file services
- synchronization between Azure and a Windows server
- operational validation of file access
- restore workflow testing
- identity and permissions considerations

## Validation Performed

- Confirmed storage account and file share deployment
- Verified Azure File Sync registration
- Confirmed sync group and server endpoint health
- Mapped the share successfully from a Windows client
- Verified file visibility through the synced path
- Tested snapshot-based recovery workflow

## Issues / Troubleshooting

Examples of troubleshooting areas documented in this lab:

- sync registration issues
- portal/browser authentication friction during agent registration
- delayed sync health state
- share mapping validation
- permission path and share path confusion

## Security / Cost Notes

- Used standard performance and LRS for low-cost lab deployment
- Kept cloud tiering disabled for simpler validation
- Reviewed IAM assignment decisions critically because lab roles may be broader than production roles

## What I Learned

- Azure Files and Azure File Sync are useful when cloud adoption must preserve familiar SMB workflows
- Validation should cover both sync health and user-side access
- Restore testing is necessary to make storage labs credible

## Next Improvements

- Test private endpoint access to the storage account
- Compare LRS, ZRS, and GRS for different use cases
- Add NTFS/share permission documentation
- Add PowerShell validation for sync and mapped-share testing
- Test cloud tiering enabled vs. disabled
