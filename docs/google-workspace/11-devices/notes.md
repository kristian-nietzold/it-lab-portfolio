\# 11 – Devices



\## Overview



This section demonstrates how devices are managed within Google Workspace, focusing on:



\- Enforcing security policies on mobile devices

\- Controlling access based on compliance requirements

\- Monitoring enrolled devices

\- Validating policy enforcement through real-world testing



The configuration uses \*\*Basic Mobile Device Management\*\*, suitable for small to medium environments while still enforcing essential security controls.



\---



\## Device Management Configuration



Mobile device management was configured using Universal Settings.



!\[Mobile management (basic configuration)](screenshots/11-02-mobile-management-basic.png)



\### Configuration



\- Management level: \*\*Basic (agentless)\*\*

\- Scope: \*\*Organisation-wide (Nietz Ltd)\*\*

\- Features enabled:

&#x20; - Account wipe capability

&#x20; - Basic password enforcement

&#x20; - Device approval tracking



\---



\## Configuration Applied



The configuration was saved and applied across the organisation.



!\[Mobile management (applied settings)](screenshots/11-03-mobile-management-saved.png)



\### Result



\- Mobile management is active for all users

\- Devices must comply with security requirements

\- Admin visibility into connected devices is enabled



\---



\## Policy Enforcement (2-Step Verification)



A sign-in attempt was made from a device that did not meet the organisation’s 2-Step Verification requirements.



!\[Device blocked due to 2SV policy](screenshots/11-04-device-blocked-2sv.png)



\### Result



\- Access was \*\*blocked automatically\*\*

\- User was required to meet 2SV requirements before proceeding

\- Demonstrates enforcement of identity-based security policies



\---



\## Device Enrolment



After meeting the required security controls, the device successfully connected and appeared in the Admin console.



!\[Device enrolled](screenshots/11-05-device-enrolled.png)



\### Observations



\- Device is linked to the user account

\- Device status: \*\*Approved\*\*

\- Ownership: \*\*User-owned (BYOD scenario)\*\*

\- Sync activity confirms active usage



\---



\## Device Inspection



Detailed device information was reviewed within the Admin console.



!\[Device details](screenshots/11-06-device-details.png)



\### Available Information



\- Device ID and resource ID

\- Operating system (Android 14)

\- Ownership type (User-owned)

\- First sync and last sync timestamps

\- Management level applied



\### Admin Actions Available



\- Block device access

\- Wipe account from device

\- Delete device from management

\- View audit information



\---



\## Devices Overview



The Devices dashboard provides a high-level view of all device categories.



!\[Devices overview](screenshots/11-01-devices-overview.png)



\### Insights



\- Separation of device types (mobile, endpoints, ChromeOS)

\- Visibility into managed vs unmanaged environments

\- Centralised control for device policies



\---



\## Key Security Decisions



\- Implemented \*\*Basic Mobile Device Management\*\* for simplicity and coverage

\- Enforced \*\*2-Step Verification integration\*\* for access control

\- Allowed \*\*BYOD (user-owned devices)\*\* with policy enforcement

\- Prioritised \*\*visibility and control without heavy device management overhead\*\*



\---



\## Validation



The following behaviours confirm correct configuration:



\- Devices are blocked if they do not meet security requirements

\- Devices successfully enrol once compliant

\- Admin console reflects real-time device status and activity

\- Device-level controls (wipe, block, audit) are available



\---



\## Real-World Considerations



\- Advanced management may be required for corporate-owned devices

\- BYOD environments require strong identity controls (e.g. 2SV)

\- Device lifecycle management should include onboarding and offboarding processes

\- Policies should be reviewed as device usage grows



\---



\## Summary



This section demonstrates:



\- Practical device management implementation

\- Integration between identity and device security

\- Real-world policy enforcement and validation

\- Administrative control over user devices in Google Workspace

