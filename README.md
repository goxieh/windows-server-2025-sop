# Standard Operating Procedure  
**Company Name**: MITT solutions  
**Company Address**: 130 Henlow Bay , Winnipeg  
**Phone**: (204) 555-0198  
**Version**: 1.0  
**Written by**: Success Ibe 
**Date**: 03/25/2025  

---

## Objectives 
This SOP states the standard procedure for the configuration and preparation of the Windows Server 2025. This would be deployed in a Lab or production environment. This SOP ensures the server is installed with necessary roles, security and networking configurations setup for optimal performance and manageability.

---

## Application  
This document applies to IT administrators, system engineers, and network technicians responsible for setting up Windows Server 2025 in enterprise or test lab environments. It is relevant when a new server is being prepared for domain services, application hosting, or infrastructure support.

---

## Definitions  
- **SOP**: Standard Operating Procedure  
- **DHCP**: Dynamic Host Configuration Protocol  
- **DNS**: Domain Name System  
- **AD DS**: Active Directory Domain Services  
- **GUI**: Graphical User Interface  
- **ISO**: Disk image file used for OS installation  

---

## Accountability Matrix  

| Role              | Responsibility                               |
|-------------------|----------------------------------------------|
| System Admin      | Handles installation and setup               |
| Network Engineer  | Double-checks network configurations         |
| Security Analyst  | Makes sure firewall and policies are solid   |
| Supervisor        | Reviews the setup and signs off              |

---


## Reversion Table  

| Version | Date       | Author        | Changes Made                 |
|---------|------------|----------------|-----------------------------|
| 1.0     | 03/25/2025 | Alex Johnson  | Initial SOP creation         |

---


## Procedure Steps  

### Step 1: Gather What You Need  
Before starting, make sure you have:
- A copy of the Windows Server 2025 ISO or bootable USB  
- A server or computer with at least 4 CPU cores, 16GB RAM, and 100GB SSD  
- Static IP details (IP address, subnet mask, gateway, and DNS)  
- Admin username and password  
   

### Step 2: Install Windows Server 2025  
- Boot from your USB or ISO  
- Choose your language and region  
- Select “Custom Install” and pick your disk partition  
- Let the install run, and when it’s done, set a secure Administrator password  

**Hazards**: Ensure backups are made before partitioning.  

### Step 3: Set Up Networking and Hostname  
- Go to `Settings > Network & Internet > Ethernet > IP Settings`  
- Switch to manual and enter your static IP details  
- Open System Properties (right-click This PC > Properties)  
- Change the computer name to something easy to remember, like `WIN-SRV-01`  
 

**Tip**: Restart the system after changing the hostname.  

### Step 4: Install Server Roles and Features  
- Open Server Manager  
- Navigate to “Manage” > “Add Roles and Features”  
- Install:
  - AD DS  
  - DNS Server  
  - File and Storage Services (if needed)  
  - Web Server (IIS) (optional)  



---

## Resources  

| Resource                            | Link or Description                        |
|-------------------------------------|--------------------------------------------|
| Microsoft Docs - Windows Server     | https://docs.microsoft.com/windows-server  |
| ISO Download for Windows Server 2025| Official Microsoft Volume Licensing Center |
| Windows Admin Center                | Optional GUI-based admin tool              |
| sconfig Tool Guide                  | Built-in server configuration utility      |


## Approval Table  

| Name           | Title                    | Signature     | Date Approved |
|----------------|---------------------------|----------------|----------------|
| Success Ibe    | SOP Writer (Student)      | ____CSI_______ | 03/25/2025     |
| Mr Felix Jiang | IT Supervisor/Instructor  | ______________ | 03/25/2025     |

---

**End of SOP**
