# Active Directory Lab

(project in progress)

## Operational Relevance 

This project demonstrates foundational Active Directory (AD) skills modeled after an IT Support environment. A Windows Server domain controller is deployed, and a custom organizational unit (OU) hierarchy separates users, groups, and endpoints. Identity and Access Management (IAM) principles are applied through role-based access control (RBAC) using security groups. Proficiency with tier 1 / tier 2 IT support tasks is demonstrated with screenshots visible when clicking the > dropdowns.  

## Tier 1/Tier 2 IT Support Tasks

<details>
 <summary> New user creation and domain-join validation</summary>

**Finance users provisioned**

<p align="center">
 <img scr="images/new.user.creation.png" width="600"><br>

**Domain authentication validation on client workstation**

![new user](images/user.login.validation.png)
 
</details>

<details>
 <summary> Account lockout / password reset </summary>

 **Provisioning account lockout policy**

 ![policy](images/configure.account.lockout.png)

 **Account lockout: 5 failed attempts**

 ![locked](images/account.locked.jpeg)

 **Assigning temporary password**

 ![temp](images/temp.password.png)

 **Unlocking account**

 ![unlock](images/unlock.account.png)

 **Password change prompt**

 ![change](images/change.password.jpeg)
 
</details>

## Group Policy Objects
<details>
 <summary> Map Sales network drive </summary>
 
 ![Map Sales network drive 1](images/sales.drive_1.png)
 ![Map Sales network drive 1](images/sales.drive_2.png)
 ![Map Sales network drive 1](images/sales.drive_3.png)
 ![Map Sales network drive 1](images/sales.drive_4.png)
 
</details>

## Job Duties Demonstrated 

- Deploy and configure Windows Server Domain Controllers for centralized identity services
- Organize Active Directory using a custom organizational unit (OU) hierarchy to support lifecycle management and policy scoping
- Implement group-based access control using Active Directory security groups (RBAC)
- Configure and enforce Group Policy Objects (GPOs) to apply security baselines and role-based system controls
- Join and validate client workstations within domains to confirm authentication, GPO application, and DNS integration





## Future Enhancements

- Expand user lifecycle workflows to include bulk provisioning and role changes using scripted automation
- Introduce delegated administrative permissions within OUs to simulate tiered administration
