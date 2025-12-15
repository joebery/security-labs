# Build Notes

## Initial VM Setup
- Hypervisor: VirtualBox
- VM Name: DC001
- OS: Windows Server (Desktop Experience)
- CPU: 2 vCPUs
- RAM: 4 GB
- Disk: 60 GB (VDI, dynamically allocated)
- Network: Internal NAT network

## Active Directory Installation
- Installed Active Directory Domain Services role via Server Manager
- Server promoted to Domain Controller
- New forest created:
  - Domain name: lab.local

## Domain Controller Details
- Hostname: DC001
- Role: Domain Controller
- Directory Services Restore Mode (DSRM) password configured

## Domain Users
- standard-user1
  - Role: Standard domain user
  - Purpose: Simulate normal employee activity

- admin-user
  - Role: Domain Administrator
  - Purpose: Simulate privileged administrative actions


## Notes
- DC001 acts as the central authentication and identity authority
- Authentication and directory events will be key security log sources
