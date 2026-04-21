\# 04. Groups \& Access Control



This section demonstrates the implementation of Google Groups for communication, collaboration, and access control within the organisation.



Groups were configured to support role-based access control (RBAC), enabling scalable permission management and simplified administration.



\---



\## Group Configuration (Access Control)



!\[All Staff Group Settings](screenshots/04-01-group-settings-all-staff.png)



Groups were configured with different access types based on purpose:



\- \*\*Public (internal)\*\* – Open collaboration across the organisation  

\- \*\*Team\*\* – Department-level communication  

\- \*\*Announcement-only\*\* – Controlled messaging from leadership  

\- \*\*Restricted\*\* – Sensitive or privileged groups  



This ensures a balance between usability and security.



\---



\## Membership Management



!\[All Staff Members](screenshots/04-02-group-members-all-staff.png)



Users were assigned to groups based on department and role.



The \*\*All Staff\*\* group includes all users, enabling organisation-wide communication and announcements.



Membership can be managed manually or dynamically expanded to include all current and future users.



\---



\## Groups Overview



!\[Groups Overview](screenshots/04-03-groups-overview.png)



The following groups were created to represent organisational structure and communication needs:



\- All Staff  

\- Announcements  

\- HR Team  

\- IT Admins  

\- IT Helpdesk  

\- Management  

\- Sales Team  



\---



\## Access Design (RBAC Support)



Groups were used as an access control layer to simplify permission management across the environment.



This allows:



\- Assigning permissions to groups instead of individual users  

\- Managing access centrally  

\- Reducing administrative overhead  



\### Examples



\- \*\*HR Team\*\* → Restricted due to sensitive employee data  

\- \*\*IT Admins\*\* → Highly restricted for privileged access  

\- \*\*Announcements\*\* → One-way communication from leadership  

\- \*\*All Staff\*\* → Organisation-wide messaging  



\---



\## Design Approach



This implementation ensures:



\- Scalable access control  

\- Centralised permission management  

\- Separation between communication and security roles  

\- Alignment with organisational structure  



\---



\## Summary



This section demonstrates:



\- Use of Google Groups for communication and collaboration  

\- Implementation of group-based access control (RBAC support)  

\- Assignment of users based on roles and departments  

\- Application of security-focused group configurations  



Groups provide a flexible and scalable mechanism for managing access and communication within the organisation.

