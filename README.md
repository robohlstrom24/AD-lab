# Active Directory Lab

(project in progress, screenshots provided in drop-down for completed work)

## Operational Relevance (Identity and Access Management)

This project demonstrates foundational Active Directory (AD) skills modeled after an IT Operations environment. A Windows Server domain controller is deployed, and a custom organizational unit (OU) hierarchy separates users, groups, and endpoints. Identity and Access Management (IAM) principles are applied through role-based access control (RBAC) using security groups. Fifteen Group Policy Objects (GPOs) are implemented and validated by joining a client workstation to the domain and confirming policy application.

## Job Duties Demonstrated 

- Deploy and configure Windows Server Domain Controllers for centralized identity services
- Organize Active Directory using a custom organizational unit (OU) hierarchy to support lifecycle management and policy scoping
- Implement group-based access control using Active Directory security groups (RBAC)
- Configure and enforce Group Policy Objects (GPOs) to apply security baselines and role-based system controls
- Join and validate client workstations within domains to confirm authentication, GPO application, and DNS integration

## Environment Structure

- **Departments:** IT, Sales, Finance  
- **Roles per department:** Assistant, Staff, Director  

### Domain-Wide GPOs (Security Baseline)

- Password length **15+ characters**
- domain time synchronization (**NTP**)
- automatic workstation lock after **15 minutes** of inactivity

### Department-Based GPOs

**IT:**
- Enable PowerShell Script Block Logging
- allow MMC snap-ins
  
**Sales:**

<details>
 <summary> Map Sales network drive </summary>
 
 ![Map Sales network drive 1](images/sales.drive_1.png)
 ![Map Sales network drive 1](images/sales.drive_2.png)
 ![Map Sales network drive 1](images/sales.drive_3.png)
 ![Map Sales network drive 1](images/sales.drive_4.png)
 
</details>
- disable access to advanced system settings

**Finance:**
- Prevent local data storage
- block removable storage (USB)  

### Role-Based GPOs

**Assistant:**
- Restrict selected Control Panel applets
- prevent software installations

**Staff:**
- Allow task-level resources
- restrict software installations
  
**Director:**
- Allow software installations
- enable enhanced logon/logoff auditing  





## Future Enhancements

- Expand user lifecycle workflows to include bulk provisioning and role changes using scripted automation
- Introduce delegated administrative permissions within OUs to simulate tiered administration
