# Active Directory Lab

(project in progress)

## Operational Relevance (Identity and Access Management)

This project demonstrates foundational Active Directory (AD) skills modeled after an IT Operations environment. A Windows Server domain controller is deployed, and a custom organizational unit (OU) hierarchy separates users, groups, and endpoints. Identity and Access Management (IAM) principles are applied by implementing role-based access control (RBAC) using security groups. A total of 15 Group Policy Objects (GPOs) are implemented and validated by joining a client workstation to the domain and confirming policy application.

### Environment Structure

- **3 departments:** IT, Sales, Finance  
- **3 employees per department:** Assistant, Staff, Director  

### Domain-Wide GPOs (Security Baseline)

- Enforce password length of **15+ characters**
- Domain time synchronization (**NTP**)
- Automatic workstation lock after **15 minutes** of inactivity

### Department-Based GPOs

**IT**
- Enable PowerShell Script Block Logging
- Allow MMC snap-ins

**Sales**
- Map Sales network drive
- Disable access to advanced system settings

**Finance**
- Prevent local data storage
- Block removable storage (USB mass storage)

### Role-Based GPOs

**Assistant**
- Restrict access to selected Control Panel applets
- Prevent software installations

**Staff**
- Allow task-level resources
- Restrict software installations

**Director**
- Allow software installations
- Enable enhanced logon/logoff auditing


## Job Skills (IT Operations)

- Deploy and configure Windows Server Domain Controllers for centralized identity services
- Organize Active Directory using a custom OU hierarchy to support lifecycle management and policy scoping
- Implement group-based access control using Active Directory security groups (RBAC)
- Join and validate client workstations within domains to confirm authentication and DNS integration

## Future Enhancements

- Apply a baseline Group Policy Object (GPO) to demonstrate centralized configuration management 
- Expand user lifecycle workflows to include bulk provisioning and role changes using scripted automation
- Implement additional security groups to model more complex role separation and access scenarios
- Introduce delegated administrative permissions within OUs to simulate tiered administration
