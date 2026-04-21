\# 05. Admin Roles \& Delegation



This section demonstrates the implementation of administrative role delegation within Google Workspace.



The objective is to distribute administrative responsibilities securely while maintaining control through the \*\*principle of least privilege\*\*.



\---



\## Purpose of Admin Roles



Administrative roles were used to:



\- Delegate responsibilities without granting full access  

\- Reduce security risk by limiting high-level permissions  

\- Support scalable management as the organisation grows  



This follows a \*\*Role-Based Access Control (RBAC)\*\* model.



\---



\## Admin Roles Overview



!\[Admin roles overview](screenshots/05-01-admin-roles-overview.png)



Google Workspace provides predefined system roles such as:



\- Super Admin  

\- Help Desk Admin  

\- Groups Admin  

\- Reports Admin  



These roles allow granular delegation of administrative tasks.



\---



\## Role Assignment



!\[Helpdesk Admin Assigned](screenshots/05-02-helpdesk-admin.png)



Administrative roles were assigned to users based on their responsibilities.



This ensures:



\- Only authorised users can perform administrative actions  

\- Responsibilities are clearly defined  

\- Full administrative access is restricted  



\---



\## Helpdesk Role (Least Privilege Example)



!\[Helpdesk Privileges](screenshots/05-03-role-helpdesk-permissions.png)



The \*\*Help Desk Admin\*\* role was used to support users while limiting access.



Permissions include:



\- View organisational units  

\- View users  

\- Reset passwords  



This allows support staff to assist users \*\*without exposing sensitive configuration settings\*\*.



\---



\## Super Admin Control



!\[Super Admins](screenshots/05-04-super-admins.png)



The \*\*Super Admin role\*\* provides full control over the environment.



Best practices applied:



\- Assigned to a minimal number of trusted users  

\- Used only for high-level configuration and oversight  

\- Not used for daily operational tasks  



This reduces risk of:



\- Accidental misconfiguration  

\- Privilege abuse  

\- Security compromise  



\---



\## Custom Role (Advanced Delegation)



!\[Custom Role Privileges](screenshots/05-05-custom-role-privileges.png)



A custom role was created:



\*\*User Provisioning Admin\*\*



Purpose:



\- Manage user creation and updates  

\- Handle onboarding tasks  

\- \*\*Exclude password reset permissions\*\*  



This separates:



\- Account provisioning  

\- User support (handled by Helpdesk)



\---



\## Custom Role Assignment



!\[Custom Role Assigned](screenshots/05-06-custom-role-assigned-admin.png)



The custom role was assigned to a designated user.



This ensures:



\- Clear separation of duties  

\- Reduced risk of privilege overlap  

\- Better auditability of actions  



\---



\## Delegation Model



Administrative access was structured as follows:



\- \*\*Super Admins\*\*

&#x20; - Full control

&#x20; - Limited to trusted users only  



\- \*\*Helpdesk Admins\*\*

&#x20; - User support (password resets, viewing users)

&#x20; - No access to sensitive settings  



\- \*\*User Provisioning Admin\*\*

&#x20; - Create/manage accounts

&#x20; - No password reset capability  



\---



\## Security Design



This implementation enforces:



\- Principle of least privilege  

\- Separation of duties  

\- Reduced attack surface  

\- Controlled access to sensitive functions  



\---



\## Integration with Groups (From Section 04)



Admin roles can also be assigned to \*\*groups\*\*, enabling:



\- Centralised role management  

\- Easier scaling as users join/leave  

\- Consistent permission assignment  



This aligns with the RBAC model implemented using Google Groups.



\---



\## Summary



This section demonstrates:



\- Delegation of administrative responsibilities  

\- Use of predefined and custom admin roles  

\- Implementation of least privilege principles  

\- Separation of high-risk and operational tasks  



The result is a \*\*secure, scalable, and enterprise-ready administrative model\*\*.

