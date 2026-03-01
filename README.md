![1](images/AD.banner2.jpg)

## Operational Relevance 

This project demonstrates foundational Active Directory (AD) skills modeled after an IT Support environment. Proficiency with tier 1 and tier 2 IT support tasks is demonstrated with screenshots (click the > dropdowns to view). Troubleshooting activities are supplemented with ITSM-style tickets which are documented in a companion repository.

(see: [Troubleshooting Journal](https://github.com/robohlstrom24/troubleshooting-journal))

## Tier-1 IT Support Tasks

<details>
 <summary> Password reset </summary>

 ![reset1](images/password.reset.4.png)
 ______________________________________
 ![reset2](images/password.reset.2.png)
 ______________________________________
 ![reset3](images/password.reset.3.png)
 
</details>

<details>
 <summary>Provision new user using role-based template</summary>

 ![1](images/onboarding1.png)
 ____________________________
 ![2](images/onboarding2.png)
 ____________________________
 ![3](images/onboarding3.png)
 
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
 <summary>Grant user access to department resource</summary>

 ![1](images/add.group3.png)
 ____________________________
 ![2](images/add.group2.png)
 
</details>

<details>
 <summary>Disable Account</summary>
 
![disable1](images/disable.account1.png)
_________________________________________
 ![disable2](images/disable.account2.png)
 
</details>

## Tier-2 IT Support Tasks

<details>
 <summary> Automate department drive mapping with Group Policy </summary>

 Implemented a Group Policy preference to automatically map a department network drive for Sales users, eliminating manual configuration and ensuring consistent access. 
 
 ![Map Sales network drive 1](images/sales.drive_1.png)
 ______________________________________________________
 ![Map Sales network drive 1](images/sales.drive_2.png)
 ______________________________________________________
 ![Map Sales network drive 1](images/sales.drive_3.png)
 ______________________________________________________
 ![Map Sales network drive 1](images/sales.drive_4.png)
 
</details>

<details>
 <summary>Troubleshooting GPO Misconfigurations </summary>
 
**Department-specific GPO (Finance users can't save files locally)**

![1](images/create.GPO1.png)
________________________
![2](images/create.GPO2.png)
 ____________________________

 **Troubleshooting scenario: Sales user reports they can't save files locally**

 ![3](images/local.save.denied.png)
 __________________________________
 ![4](images/troubleshooting.png)
 ________________________________
 ![5](images/misconfigured.GPO.png)
 __________________________________
 ![6](images/GPO.removed.png)
 ______________________________

 **Resolution:** 
 - Removed the unintended domain-level link while preserving the GPO for the Finance OU
 - Confirmed policy scope corrected and Sales user functionality restored

See: [Troubleshooting Journal T-0008](https://github.com/robohlstrom24/troubleshooting-journal) for ITSM-style troubleshooting ticket

</details>

<details>
 <summary>Troubleshooting Broken Domain Trust</summary>

 **Scenario: A workstation’s computer account was removed from Active Directory during routine directory cleanup, breaking the secure channel between the device and the domain.**

 ![1](images/trust-failure/hook.png)
 ___________________________________

 ![2](images/trust-failure/confirm-trust-broken.png)
 ________________________________________________

 ![3](images/trust-failure/leave-domain.png)
 ________________________________________________

 ![4](images/trust-failure/rejoin-domain)

</details>

## Future Enhancements

- Expand user lifecycle workflows to include bulk provisioning and role changes using scripted automation
- Introduce delegated administrative permissions within OUs to simulate tiered administration
