---
layout: page
title: "Compliance & Data Protection"
nav_exclude: true
---
\# 02. Organisational Units



This section demonstrates the design and implementation of organisational units (OUs) within Google Workspace.



The OU structure was configured to reflect a realistic business environment, enabling structured user management, policy enforcement, and hierarchical control through inheritance.



\---



\## Initial OU State



The environment initially contained only the root organisational unit.



!\[Initial OU Overview](screenshots/02-01-ou-overview.png)



\---



\## OU Creation



Organisational Units (OUs) were configured within the Admin console by defining:



\- Name  

\- Description  

\- Parent OU  



!\[Create OU Example](screenshots/02-02-create-ou-example.png)



This allows administrators to build a hierarchical structure for users and policies.



\---



\## OU Structure



The following OU hierarchy was implemented:



\- Root: Nietz Ltd

&#x20; - IT

&#x20;   - Admins

&#x20;   - Helpdesk

&#x20; - HR

&#x20; - Finance

&#x20; - Sales

&#x20; - Management



!\[Final OU Hierarchy](screenshots/02-03-ou-hierarchy.png)



\---



\## Design Approach



The structure was designed to:



\- Separate users by department (HR, Finance, Sales, etc.)

\- Isolate privileged accounts (IT Admins vs Helpdesk)

\- Support scalable organisational growth

\- Enable policy inheritance across OUs



\### Policy Inheritance



Policies applied at higher-level OUs automatically cascade down to child OUs unless explicitly overridden.



This allows:



\- Centralised control (e.g. security policies at root level)

\- Granular overrides (e.g. stricter controls for Admins)

\- Reduced administrative overhead



\---



\## Summary



This section demonstrates:



\- Implementation of organisational unit hierarchy  

\- Understanding of policy inheritance  

\- Separation of users by role and department  

\- Scalable design aligned to business structure  



These organisational units form the foundation for applying policies across the environment.

