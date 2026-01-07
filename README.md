# Windows Server 2019 Administration Lab

A comprehensive Windows Server 2019 administration project covering Hyper-V virtualization, Active Directory, DNS, DHCP, Group Policy, and security hardening in an enterprise environment.

##  Project Overview

This lab demonstrates complete Windows Server 2019 administration skills through a simulated enterprise environment for **TechNova Corporation**. The project covers infrastructure setup from virtualization to security hardening.

###  Lab Objectives
1. **Hyper-V Virtualization**: Deploy Windows Server 2019 on Hyper-V
2. **Active Directory**: Create and manage domain infrastructure
3. **Network Services**: Configure DNS and DHCP services
4. **Group Policy**: Implement security policies and drive mapping
5. **Security Hardening**: Apply Windows Defender, Firewall, and best practices
6. **Remote Access**: Configure VPN and RDP access

##  Lab Architecture

### Virtual Environment
- **Hypervisor**: Microsoft Hyper-V
- **Server OS**: Windows Server 2019 (Desktop Experience)
- **Domain**: `technova.local`
- **Server Hostname**: `GIF-SERVER01`
- **Client OS**: Windows 10

### Network Configuration
- **IP Addressing**: DHCP with static reservations
- **DNS**: Forward and Reverse lookup zones
- **Services**: Active Directory, DNS, DHCP, Remote Access

##  Lab Components

### 1. Hyper-V Setup & Windows Server Installation
- Virtual machine creation with proper resource allocation
- Windows Server 2019 installation with Desktop Experience
- System configuration and updates

### 2. Active Directory Domain Services
- Promote server to Domain Controller
- Create Organizational Units (HR, IT, Finance)
- User and group management
- Group Policy Object creation and linking

### 3. Network Services Configuration
- **DNS**: Forward/Reverse lookup zones
- **DHCP**: Scope creation with exclusions and reservations
- **IP Address Management**: Range configuration for client devices

### 4. Group Policy Management
- Password complexity policies
- Network drive mapping for HR department
- Security baseline configurations

### 5. Security & Hardening
- Windows Defender Antivirus configuration
- Windows Firewall rules (Allow RDP, Block ICMP)
- Certificate Services (AD CS)
- VPN configuration and testing
- Security best practices implementation

##  Getting Started

### Prerequisites
- Windows 10/11 Pro/Enterprise with Hyper-V enabled
- 16GB RAM minimum (8GB for Host, 8GB for VM)
- 100GB free disk space
- Windows Server 2019 ISO

### Setup Instructions
1. **Enable Hyper-V**:
```powershell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
