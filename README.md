## Active Directory 101 (in progress)

## Operational Relevance (Identity and Access Management)

This project demonstrates foundational Active Directory skills modeled after an IT Operations environment. A Windows Server Domain Controller is deployed, and a custom organizational unit (OU) hierarchy separates users, groups, and endpoints. The OU structure is designed to support Group Policy application and centralized policy management. The principles of Identity and Access Management (IAM) are applied by implementing role-based access controls (RBAC) across user groups. User lifecycle management is simulated through account deprovisioning, and endpoint integration is demonstrated by joining a client workstation to the domain.

## Job Skills (IT Operations)

- Deploy and configure Windows Server Domain Controllers for centralized identity services
- Organize Active Directory using a custom OU hierarchy to support lifecycle management and policy scoping
- Implement group-based access control using Active Directory security groups (RBAC)
- Join and validate client workstations within domains to confirm authentication and DNS integration

## Future Enhancements

- Apply a baseline Group Policy Object (GPO) to demonstrate centralized configuration management (e.g., password policy or desktop security settings)
- Expand user lifecycle workflows to include bulk provisioning and role changes using scripted automation
- Implement additional security groups to model more complex role separation and access scenarios
- Introduce delegated administrative permissions within OUs to simulate tiered administration
