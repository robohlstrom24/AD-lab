# Active Directory Lab

(project in progress)

## Operational Relevance 

This project demonstrates foundational Active Directory (AD) skills modeled after an IT Support environment. A Windows Server domain controller is deployed, and a custom organizational unit (OU) hierarchy separates users, groups, and endpoints. Proficiency with tier 1 IT support tasks is demonstrated with screenshots (click the > dropdowns to view).  

## Tier 1 IT Support Tasks

<details>
 <summary> Password reset </summary>

 ![reset1](images/password.reset.4.png)
 ![reset2](images/password.reset.2.png)
 ![reset3](images/password.reset.3.png)
 
</details>

<details>
 <summary>Provision new user using role-based template</summary>

 ![1](images/onboarding1.png)
 ![2](images/onboarding2.png)
 ![3](images/onboarding3.png)
 
</details>

<details>
 <summary>Disable Account</summary>
 
![disable1](images/disable.account1.png)
 ![disable2](images/disable.account2.png)
 
</details>

<details>
 <summary> Account lockout / unlock </summary>

 **Account lockout: 5 failed attempts**

<p align="left">
 <img src="images/account.locked.jpeg" width="300><br>
  </p>

 **Assigning temporary password**

 ![temp](images/temp.password.png)

 **Unlocking account**

 ![unlock](images/unlock.account.png)

 **Password change prompt**

<p align="left">
 <img src="images/change.password.jpeg" width="300"><br>
  </p>

 **Provisioning account lockout policy**

 ![policy](images/configure.account.lockout.png)
 
</details>

<details>
 <summary> New user creation and domain-join validation</summary>

**Finance users provisioned**

![provision](images/new.user.creation.png)

**Domain authentication validation on client workstation**

![new user](images/user.login.validation.png)
 
</details>

<details>
 <summary>Grant user access to department resource</summary>

 ![1](images/add.group3.png)
 ![2](images/add.group2.png)
 
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
