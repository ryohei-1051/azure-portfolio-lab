# Lab 1 - Hybrid Networking with Azure VPN Gateway and Private DNS

## Objective

Build a hybrid Azure test environment that simulates connectivity between an on-premises-style network and Azure using site-to-site VPN.

## What I Built

- Azure resource group for lab resources
- Azure Policy to restrict deployment locations
- Azure virtual network for Azure-hosted services
- Simulated on-premises virtual network
- Azure Virtual Network Gateway
- Local Network Gateway
- Windows Server 2022 and Windows 11 VMs
- RRAS configuration for VPN connectivity
- Azure Private DNS for name resolution testing

## Architecture Summary

This lab simulates a hybrid environment with:

- Azure-side virtual network
- On-premises-side virtual network
- VPN gateway connection between the two
- RRAS acting as the VPN endpoint on the simulated on-prem side
- Private DNS for hostname resolution

## Why This Lab Matters

This lab demonstrates core hybrid infrastructure concepts relevant to systems administration and cloud migration:

- extending an on-prem network into Azure
- planning address spaces and subnets
- validating routing across connected environments
- supporting private name resolution
- applying basic governance with Azure Policy

## Validation Performed

- Verified virtual network creation and addressing
- Confirmed VPN connection establishment
- Tested reachability between Azure and on-prem resources
- Validated hostname resolution using Private DNS
- Confirmed expected resource placement within allowed regions

## Issues / Troubleshooting

Examples of troubleshooting areas documented in this lab:

- address space overlap
- VPN gateway deployment delays
- RRAS misconfiguration
- DNS resolution issues
- route validation between networks

## Security / Cost Notes

- Chose lab-sized VM instances where possible
- Kept scope limited to required resources
- Planned cleanup after validation
- Used policy for region restriction to reflect governance requirements

## What I Learned

- Hybrid design depends heavily on correct addressing and routing assumptions
- DNS validation is as important as raw IP connectivity
- Azure networking labs become much more useful when paired with troubleshooting evidence

## Next Improvements

- Add NSGs and document allowed traffic
- Add Azure Bastion instead of direct public management exposure
- Compare VPN Gateway SKUs
- Add Network Watcher validation
- Document production design differences vs. lab shortcuts
