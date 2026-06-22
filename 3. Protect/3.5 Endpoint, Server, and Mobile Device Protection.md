---
icon: triangle-right
order: 50
---

### Goal

Endpoints are where company work happens.

Laptops, desktops, servers, phones, tablets, and remote devices are used every day to access email, files, financial systems, customer records, admin portals, cloud services, and internal tools.

If these devices are weak, the company is weak.

This section defines how the company protects the devices and servers used to access company systems and data. It covers endpoint protection, mobile device controls, server protection, local firewalls, encryption, software control, removable media, remote wipe, device health, and lost-device handling.

## Step 1: Assign Device Protection Ownership

Name the people responsible for endpoint, server, and mobile device protection.

|Role|Responsibility|
|---|---|
|Device Protection Owner|Owns the full process|
|Endpoint Technical Owner|Manages laptops, desktops, endpoint tools, and device settings|
|Server Technical Owner|Manages servers and server protection tools|
|Mobile Device Owner|Manages phones, tablets, BYOD rules, and MDM settings|
|MSP or Vendor Contact|Handles managed devices or outsourced support|
|Executive Sponsor|Approves standards, exceptions, and budget|

Do not leave this as “devices are handled by IT.”

Every device type needs an owner.

## Step 2: Define Which Devices Are Allowed

The company should define which devices are allowed to access company systems.

Use clear categories.

|Device Type|Access Rule|
|---|---|
|Company-owned laptop|Full access if enrolled, protected, encrypted, and current|
|Company-owned desktop|Full access if protected, encrypted where needed, and current|
|Company-owned phone or tablet|Access allowed through approved mobile controls|
|Personal phone|Limited access only if approved and controlled|
|Personal laptop|Avoid for company systems unless formally approved|
|Contractor device|Limited access, time-limited, and reviewed|
|Vendor support device|Controlled through approved remote support process|
|Unknown device|No access|

Unknown devices should not be trusted.

If the company does not manage the device, access should be limited.

## Step 3: Create a Device Protection Standard

Create one basic protection standard for each device type.

**Suggested standards:**

|Device Type|Required Protection|
|---|---|
|Windows laptop|Endpoint protection, encryption, firewall, screen lock, updates, no normal local admin|
|Mac laptop|Endpoint protection, FileVault, firewall, screen lock, updates, managed admin rights|
|Linux workstation|Endpoint monitoring, firewall, updates, disk encryption where needed, restricted sudo|
|Windows server|EDR or server protection, firewall, logging, restricted admin access, backup agent|
|Linux server|Monitoring agent, firewall, SSH restrictions, logging, package updates, backup agent|
|iPhone or iPad|Passcode, encryption, remote wipe, managed apps, OS updates|
|Android device|Passcode, encryption, remote wipe, managed work profile, OS updates|
|Shared device|Assigned owner, restricted login, limited data storage, wipe/reset process|

The standard should be short enough to use, but strong enough to enforce.

## Step 4: Enroll Devices in a Management System

Company-owned devices should be enrolled into a device management or endpoint management system.

**The management system should be able to show:**

|Management Need|Requirement|
|---|---|
|Device inventory|Know which devices exist|
|User assignment|Know who uses each device|
|Operating system version|Know whether OS is supported|
|Encryption status|Confirm encryption is enabled|
|Security tool status|Confirm endpoint protection is running|
|Patch status|Confirm updates are applied|
|Compliance status|Flag risky devices|
|Remote wipe|Wipe lost or stolen devices|
|Configuration policy|Apply standard settings|
|Software inventory|Know installed applications|

A device that cannot be seen or managed should not receive normal access to company systems.

## Step 5: Deploy Endpoint Protection

Every laptop, desktop, and server should have approved protection.

**At minimum, endpoint protection should provide:**

|Capability|Purpose|
|---|---|
|Malware protection|Block known malicious files and activity|
|Behavioral protection|Detect suspicious behavior, not only known signatures|
|Ransomware protection|Help detect or block mass file changes and encryption behavior|
|Web protection|Block known malicious sites where supported|
|Exploit protection|Reduce common exploit paths|
|Central reporting|Show which devices are protected|
|Alerting|Notify the owner when protection fails or detects activity|
|Tamper protection|Stop users or malware from disabling the tool|
|Isolation capability|Isolate a compromised endpoint where supported|

Free antivirus alone may be better than nothing, but it is not enough for higher-risk environments.

For most SMEs, use a centrally managed endpoint protection or EDR solution.

## Step 6: Protect Servers Separately from User Devices

Servers need stricter protection than normal endpoints.

**Check every server for:**

|Server Protection Area|Requirement|
|---|---|
|Security agent|Installed and active where supported|
|Firewall|Enabled and restricted|
|Remote access|Limited to approved admins|
|Admin accounts|Named and reviewed|
|Service accounts|Documented|
|Logging|Enabled|
|Backup agent|Installed and tested|
|Malware scanning|Enabled where appropriate|
|File integrity monitoring|Used on important servers where practical|
|Public exposure|Avoided unless required|
|Change control|Important changes recorded|
|Resource monitoring|Disk, memory, CPU, and service health monitored|

Do not treat servers like ordinary workstations.

A compromised server can affect many users at once.

## Step 7: Enable Full-Disk Encryption

Devices that store or access company data should be encrypted.

**Use:**

|Platform|Common Option|
|---|---|
|Windows|BitLocker|
|macOS|FileVault|
|Linux|LUKS or approved disk encryption|
|iOS and iPadOS|Built-in encryption with passcode|
|Android|Built-in encryption with passcode|
|External drives|Approved encrypted storage only|

Store recovery keys in a controlled system.

Do not leave recovery keys only with the user.

Do not store recovery keys in plain spreadsheets.

## Step 8: Enforce Screen Lock and Session Lock

All devices should lock automatically when not in use.

**Suggested starting settings:**

|Device Type|Lock Requirement|
|---|---|
|Laptops and desktops|Auto-lock after 5 to 15 minutes|
|Servers|Admin sessions lock when idle|
|Mobile devices|Auto-lock after short idle time|
|Shared devices|Shorter timeout|
|High-risk roles|Shorter timeout and stronger unlock method|

Use PINs, passwords, biometrics, or passkeys depending on the device and company standard.

A lost unlocked laptop is not a small problem.

## Step 9: Restrict Local Administrator Rights

Normal users should not have local administrator rights for daily work.

**Check:**

|Platform|Required Action|
|---|---|
|Windows|Remove normal users from local administrators group|
|macOS|Use standard accounts for daily use|
|Linux|Limit sudo access|
|Servers|Admin rights only for approved administrators|
|Shared devices|No local admin for normal users|
|Developer devices|Admin access approved only where justified|

Where local admin is required, document the reason and review it regularly.

## Step 10: Enable and Manage Local Firewalls

Local firewalls should be enabled on laptops, desktops, and servers.

**Check:**

|Device Type|Firewall Requirement|
|---|---|
|Windows laptops|Windows firewall enabled|
|Mac laptops|macOS firewall enabled where appropriate|
|Linux devices|UFW, firewalld, nftables, or iptables configured|
|Windows servers|Inbound access restricted|
|Linux servers|Only required ports open|
|Mobile devices|Managed through OS and app controls|

Do not leave unnecessary inbound access open.

## Step 11: Control Software Installation

Users should not install any software they want.

**Create rules for software installation:**

|Software Type|Rule|
|---|---|
|Approved business software|Allowed|
|Security tools|Installed by IT or MSP|
|Remote access tools|Approved only|
|Browser extensions|Approved only|
|Free utilities|Reviewed before use|
|Cracked software|Prohibited|
|Personal software|Restricted|
|Developer tools|Approved by role|
|AI desktop apps|Reviewed before installation|
|Unknown installers|Blocked or reviewed|

Software control reduces malware, shadow IT, privacy risk, and licensing risk.

## Step 12: Control Remote Access Tools

Remote access software can be useful. It can also become an attacker’s favorite door.

**Check all devices for:**

|Remote Tool Area|Requirement|
|---|---|
|Approved tools|Only company-approved remote tools allowed|
|Unapproved tools|Removed|
|Vendor access|Named accounts only|
|MFA|Required where supported|
|Session logging|Enabled where available|
|Unattended access|Limited and reviewed|
|Personal remote tools|Prohibited|
|Admin remote tools|Restricted to approved support users|
|Old agents|Removed from devices no longer supported|

Examples of tools to review include AnyDesk, TeamViewer, Splashtop, ConnectWise, ScreenConnect, RustDesk, Chrome Remote Desktop, RDP, VNC, SSH, and RMM agents.

## Step 13: Protect Mobile Devices

Mobile devices need real controls, especially when they access email, files, MFA apps, customer data, or admin portals.

**Set mobile requirements:**

|Mobile Control|Requirement|
|---|---|
|Passcode|Required|
|Encryption|Required|
|OS updates|Required|
|Remote wipe|Required for company data|
|Lost-device reporting|Required immediately|
|Work profile|Used where available for BYOD|
|App control|Company apps managed|
|Jailbreak/root detection|Block or alert where supported|
|Copy/paste control|Used where needed for sensitive data|
|Cloud backup|Controlled for company data|
|Screen lock|Required|
|MFA apps|Protected and recoverable|
|Device ownership|Company-owned or BYOD clearly marked|

For BYOD, protect company data without taking unnecessary control over personal data.

Use mobile application management where full device management is not appropriate.

## Step 14: Separate Work and Personal Data

Work data should not mix freely with personal apps and personal accounts.

**Check:**

|Area|What to Control|
|---|---|
|Mobile email|Use managed mail apps where possible|
|File storage|Block saving company files to personal storage|
|Copy and paste|Restrict between work and personal apps where needed|
|Personal cloud sync|Block company data sync to personal accounts|
|Personal email|Do not use for company work|
|Messaging apps|Do not use for sensitive company files unless approved|
|Screenshots|Restrict where needed for sensitive apps|
|Backups|Do not allow company data into personal backups where avoidable|

This is especially important for HR, finance, executives, sales, customer support, and administrators.

## Step 15: Protect Removable Media

USB drives and external disks can introduce malware or remove data.

**Set rules:**

|Removable Media Area|Requirement|
|---|---|
|USB storage|Block, restrict, or approve by business need|
|External drives|Encryption required|
|Unknown USB devices|Prohibited|
|Vendor USB devices|Scanned before use|
|Data transfer|Approved method preferred|
|Logging|Record removable media use where practical|
|Exceptions|Documented and approved|

If USB storage is allowed, it should be controlled.

## Step 16: Protect Remote Workers

Remote workers need the same level of device protection as office workers.

**Check:**

|Remote Work Area|Requirement|
|---|---|
|Company device|Preferred|
|Personal device|Limited access only|
|VPN or secure access|Used where required|
|Wi-Fi|No open public Wi-Fi without protection|
|Local storage|Controlled|
|Screen privacy|Required in public places|
|Device updates|Required|
|Endpoint protection|Required|
|Lost-device process|Known by user|
|Family/shared use|Not allowed on company devices|
|Printing|Restricted where sensitive data is involved|

A remote laptop is still part of the company environment.

## Step 17: Protect High-Risk Devices

Some devices need stronger controls.

**High-risk devices include:**

|Device Type|Reason|
|---|---|
|Executive laptops|Targeted for fraud, email access, and sensitive decisions|
|Finance devices|Payment, bank, invoice, and payroll access|
|HR devices|Employee data and personal records|
|IT admin devices|Admin portals and privileged access|
|Developer devices|Code, secrets, keys, repositories|
|Server admin workstations|Access to infrastructure|
|Shared reception devices|High physical exposure|
|Travel devices|Higher loss and theft risk|

**Apply stronger rules to these devices:**

|Stronger Control|Use|
|---|---|
|Hardware security keys|High-risk users and admins|
|Stricter local admin control|Admin and finance devices|
|Stronger endpoint protection|Admin, executive, and finance devices|
|More frequent patch checks|High-risk devices|
|Limited browser extensions|Admin and finance devices|
|Restricted USB|High-risk devices|
|More frequent access review|High-risk users and devices|
|Travel mode|Reduced data stored locally during travel|

Do not protect every device as if it carries the same risk.

## Step 18: Protect Device Management and EDR Consoles

The tools that manage devices are high-value targets.

**Protect these consoles carefully:**

|Console Type|Protection Required|
|---|---|
|MDM console|MFA, limited admins, logging|
|EDR console|MFA, limited admins, role separation|
|RMM console|MFA, named accounts, vendor access review|
|Patch management console|MFA and limited admin rights|
|Remote support console|MFA and session logging|
|Antivirus console|Tamper protection and limited admins|
|Cloud endpoint console|MFA and admin review|

If attackers control the device management console, they may control the fleet.

## Step 19: Monitor Device Health

Device protection must be checked regularly.

**Track:**

|Health Check|What to Confirm|
|---|---|
|Endpoint protection active|Agent installed and running|
|Endpoint protection updated|Signatures and engine current|
|Device encrypted|Encryption active|
|Firewall enabled|Local firewall active|
|OS supported|Device not end-of-life|
|OS patched|Updates current|
|Reboot needed|Pending reboot cleared|
|Disk space|Enough space for updates and logs|
|Last check-in|Device still reporting|
|Risk status|No high-risk alerts open|
|MDM status|Device compliant|
|Local admin status|No unauthorized admin|
|Lost or stale devices|Investigated|

A device that has not checked in for weeks should be investigated.

## Step 20: Create a Lost or Stolen Device Process

Lost devices must be handled quickly.

**The process should include:**

|Action|Requirement|
|---|---|
|User reports loss|Immediately to IT, MSP, or security contact|
|Device marked lost|Record time, user, device, and location|
|Account risk checked|Review recent logins|
|Remote lock|Trigger where available|
|Remote wipe|Trigger when needed|
|Password reset|Reset if compromise is possible|
|MFA reset|Review if mobile device had MFA apps|
|Data exposure check|Identify what data may be on the device|
|Replacement device|Issued through standard build|
|Incident record|Keep documentation|
|Insurance or legal review|Escalate where needed|

A lost phone may also mean lost MFA access.

A lost laptop may also mean exposed files.

Do not treat lost devices casually.

## Step 21: Manage Device Offboarding

When a user leaves, their devices must be handled properly.

**Check:**

|Offboarding Item|Requirement|
|---|---|
|Laptop returned|Confirmed|
|Phone returned|Confirmed if company-owned|
|Tablet returned|Confirmed if company-owned|
|Device wiped|Completed before reassignment|
|Local files reviewed|Important files transferred|
|Encryption recovery|Confirmed|
|Security agent removed or reassigned|Completed|
|MDM record updated|Completed|
|Asset inventory updated|Completed|
|Lost device escalated|If not returned|
|BYOD work profile removed|Completed|

Do not reassign devices without wiping and rebuilding them.

## Step 22: Handle BYOD Carefully

Bring-your-own-device access should be limited and controlled.

**Set a BYOD rule:**

|BYOD Area|Requirement|
|---|---|
|Allowed systems|Define what BYOD can access|
|Prohibited systems|Define what BYOD cannot access|
|Company data|Keep in managed apps where possible|
|Device security|Passcode and supported OS required|
|Remote wipe|Company data wipe where supported|
|Personal privacy|Do not collect unnecessary personal data|
|Exit process|Remove company data when user leaves|
|Consent|User agrees to BYOD rules|
|Exceptions|Approved and reviewed|

For many SMEs, the safest rule is simple: personal phones may access email through managed apps, but personal laptops may not access sensitive systems.

## Step 23: Keep Evidence

Keep proof that device protection is working.

**Useful evidence includes:**

|Evidence Type|Example|
|---|---|
|Device inventory export|List of managed devices|
|Endpoint protection report|Protected, unprotected, and unhealthy devices|
|Encryption report|Devices with BitLocker, FileVault, or mobile encryption|
|MDM compliance report|Compliant and non-compliant devices|
|Patch status report|Devices current or overdue|
|Local admin report|Devices with local admin users|
|Lost-device record|Lock, wipe, or recovery evidence|
|BYOD consent record|User acceptance of BYOD rules|
|Exception approval|Device exception with expiration date|
|Server protection report|Server agents and health status|
|Remote support tool inventory|Approved and unapproved agents|

If the company cannot prove a device is protected, assume it needs review.

## Step 24: Review the Process Regularly

Review endpoint, server, and mobile device protection at least quarterly.

**Check:**

|Review Area|Question|
|---|---|
|Device inventory|Are all devices known?|
|Endpoint protection|Are all devices protected?|
|Encryption|Are all required devices encrypted?|
|Mobile access|Are mobile devices managed or controlled?|
|Local admin|Are local admin rights still limited?|
|Remote tools|Are only approved remote tools installed?|
|Lost devices|Are unresolved lost devices closed out?|
|Servers|Are server protection agents healthy?|
|BYOD|Are personal devices still appropriate?|
|Exceptions|Are exceptions still valid?|
|Evidence|Can the company prove protection is working?|

Do not wait for an incident to find out half the devices are unmanaged.

## Places Commonly Missed

|Missed Area|What to Check|
|---|---|
|Personal phones|Email, MFA apps, file access, screenshots, personal backups|
|Personal laptops|Access to webmail, SaaS, CRM, finance, and file storage|
|Old employee laptops|Returned, wiped, removed from management|
|Shared tablets|Passcodes, managed apps, wipe process|
|Reception or warehouse PCs|Shared login, local admin, browser sessions|
|Developer laptops|Secrets, SSH keys, package managers, local admin|
|Finance laptops|Banking portals, spreadsheet exports, invoice files|
|Executive devices|Email, confidential files, fraud risk|
|Backup servers|Agent health, admin access, tamper protection|
|RMM agents|Old agents, vendor access, MFA, unattended access|
|Remote support tools|Unapproved tools and unattended access|
|Browser extensions|Data access and risky permissions|
|USB drives|Data copies and malware risk|
|Printers and scan workstations|Stored documents and address books|
|Old phones|Still signed into email or MFA|
|Devices that stopped checking in|Lost, powered off, unmanaged, or tampered|
|Test servers|No endpoint protection, weak passwords, old software|
|Linux servers|No EDR, no audit logs, no file integrity monitoring|
|Contractor devices|Temporary access that became permanent|

## Recommended Tools and Solutions

|Tool or Solution|Link|Type|Best Use|
|---|---|---|---|
|Microsoft Defender for Business|[Microsoft Defender for Business](https://www.microsoft.com/security/business/endpoint-security/microsoft-defender-business)|Affordable commercial|Endpoint protection and EDR for SMEs using Microsoft 365|
|Microsoft Intune|[Microsoft Intune](https://www.microsoft.com/security/business/microsoft-intune)|Commercial, often bundled|Endpoint management, MDM, app management, device compliance|
|Google Endpoint Management|[Google Endpoint Management](https://workspace.google.com/products/admin/endpoint/)|Included with Google Workspace, advanced features by plan|Managing and securing devices that access Google Workspace|
|Google Admin Console|[Google Admin Console](https://admin.google.com/)|Included with Google Workspace|Device, user, app, and access management|
|Apple Business|[Apple Business](https://business.apple.com/)|Apple platform service|Apple device enrollment, deployment, and management support|
|Apple Platform Deployment|[Apple Platform Deployment](https://support.apple.com/guide/deployment/welcome/web)|Free guidance|Apple device deployment and management guidance|
|Android Enterprise|[Android Enterprise](https://www.android.com/enterprise/management/)|Android business platform|Android device and work profile management|
|Fleet|[Fleet](https://fleetdm.com/)|Open-source and commercial|Open device management, MDM, patch visibility, osquery-based reporting|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|Endpoint and server security monitoring, XDR, SIEM, compliance visibility|
|osquery|[osquery](https://osquery.io/)|Open-source|Endpoint visibility and querying device state across operating systems|
|Velociraptor|[Velociraptor](https://www.rapid7.com/products/velociraptor/)|Open-source|Endpoint visibility, digital forensics, and incident response collection|
|ClamAV|[ClamAV](https://www.clamav.net/)|Open-source|Malware scanning, especially for servers, mail gateways, and file scanning|
|Sysmon|[Sysmon](https://learn.microsoft.com/sysinternals/downloads/sysmon)|Free|Windows and Linux system activity logging|
|YARA|[YARA](https://virustotal.github.io/yara/)|Open-source|Malware pattern matching and file scanning rules|
|Sigma|[Sigma](https://sigmahq.io/)|Open-source|Detection rule format for logs and security tools|
|ManageEngine Endpoint Central|[ManageEngine Endpoint Central](https://www.manageengine.com/products/desktop-central/)|Commercial with free edition options|Endpoint management, patching, software deployment, MDM|
|Action1|[Action1](https://www.action1.com/)|Free tier and commercial|Remote patching and vulnerability remediation|
|JumpCloud Device Management|[JumpCloud Device Management](https://jumpcloud.com/platform/cloud-device-management)|Commercial with SMB options|Cross-platform device, identity, and access management|
|Snipe-IT|[Snipe-IT](https://snipeitapp.com/)|Open-source and hosted|Device asset tracking|
|GLPI|[GLPI](https://glpi-project.org/)|Open-source|IT asset and service management|
|Windows LAPS|[Windows LAPS](https://learn.microsoft.com/windows-server/identity/laps/laps-overview)|Included in Windows environments|Local administrator password management|
|BitLocker|[BitLocker](https://learn.microsoft.com/windows/security/operating-system-security/data-protection/bitlocker/)|Included in Windows business editions|Windows disk encryption|
|FileVault|[FileVault](https://support.apple.com/guide/security/volume-encryption-with-filevault-sec4c6dc1b6e/web)|Included in macOS|Mac disk encryption|
|USBGuard|[USBGuard](https://usbguard.github.io/)|Open-source|USB device control for Linux|
|Fail2ban|[Fail2ban](https://www.fail2ban.org/)|Open-source|Server protection against repeated failed login attempts|
|CrowdSec|[CrowdSec](https://www.crowdsec.net/)|Open-source and commercial|Collaborative intrusion prevention and server protection|
|Lynis|[Lynis](https://cisofy.com/lynis/)|Open-source|Linux, macOS, and Unix security auditing|
|OpenSCAP|[OpenSCAP](https://www.open-scap.org/)|Open-source|Security compliance and configuration assessment|
|UFW|[UFW](https://help.ubuntu.com/community/UFW)|Open-source|Simple Linux firewall management|
|firewalld|[firewalld](https://firewalld.org/)|Open-source|Linux firewall management|
|AppArmor|[AppArmor](https://apparmor.net/)|Open-source|Linux application access restriction|
|SELinux|[SELinux Project](https://selinuxproject.org/)|Open-source|Linux mandatory access control|
|MicroMDM|[MicroMDM](https://micromdm.io/)|Open-source|Apple MDM for technical teams; verify current project status before use|
|Mosyle|[Mosyle](https://mosyle.com/)|Affordable commercial|Apple device management for small teams and schools|
|Jamf Now|[Jamf Now](https://www.jamf.com/products/jamf-now/)|Affordable commercial|Simple Apple device management for small organizations|

## Practical Tool Stack for SMEs

| Company Type                             | Suggested Stack                                                                                                                                                  |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Very small company**                   | Built-in Microsoft or Google device controls, Defender for Business or affordable endpoint protection, BitLocker or FileVault, Snipe-IT or spreadsheet inventory |
| **Microsoft-based SME**                  | Microsoft Defender for Business, Microsoft Intune, Windows LAPS, BitLocker, Microsoft 365 device compliance reporting                                            |
| **Google Workspace SME**                 | Google Endpoint Management, Google Admin Console, Android Enterprise, Apple Business or Apple MDM, third-party endpoint protection                               |
| **Mixed Windows and Mac company**        | Fleet, JumpCloud, ManageEngine Endpoint Central, Defender for Business, Jamf Now or Mosyle for Apple-heavy teams                                                 |
| **Linux or server-heavy company**        | Wazuh, osquery, Lynis, OpenSCAP, ClamAV, Fail2ban, CrowdSec, UFW or firewalld                                                                                    |
| **Company with many mobile devices**     | Intune, Google Endpoint Management, Android Enterprise, Apple Business, Jamf Now, Mosyle                                                                         |
| **Technical or security-mature company** | Wazuh, Velociraptor, Fleet, osquery, YARA, Sigma, OpenSCAP, centralized logging                                                                                  |

## Device Protection Register Template

|Field|What to Record|
|---|---|
|Device Name|Laptop, desktop, server, phone, tablet, or VM name|
|Device Type|Windows, macOS, Linux, iOS, Android, server, shared device|
|Owner|Assigned employee, department, or technical owner|
|Business Use|What the device is used for|
|Managed|Yes or no|
|Management Tool|Intune, Google Endpoint Management, Fleet, Jamf, Mosyle, other|
|Endpoint Protection|Tool installed|
|Protection Status|Healthy, warning, missing, unknown|
|Encryption|Enabled, disabled, unknown|
|Firewall|Enabled, disabled, unknown|
|OS Version|Current operating system version|
|Patch Status|Current, overdue, unknown|
|Local Admin|Yes, no, approved exception|
|Remote Access Tool|Installed tool if any|
|Last Check-In|Last time device reported|
|Lost or Stale|Yes or no|
|BYOD|Yes or no|
|Exception|Yes or no|
|Next Action|Required fix|
|Review Date|Next review date|

## Expected Outputs from This Section

At the end of this section, the company should have:

- A named owner for endpoint, server, and mobile device protection.
- A clear rule for which devices can access company systems.
- A protection standard for laptops, desktops, servers, phones, and tablets.
- A device management or endpoint management process.
- Endpoint protection installed on required devices.
- Server protection installed where supported.
- Full-disk encryption enabled on required devices.
- Screen lock rules enforced.
- Local administrator rights restricted.
- Local firewalls enabled.
- Software installation rules defined.
- Remote access tools controlled.
- Mobile devices protected.
- Work and personal data separated where possible.
- Removable media controlled.
- Remote worker devices protected.
- High-risk devices identified.
- EDR, MDM, and RMM consoles protected.
- Device health monitored.
- Lost-device process documented.
- Device offboarding process documented.
- BYOD rules documented.
- Evidence stored.
- Quarterly review process established.


## Objective

Do not treat devices casually - every device that touches company data should be known, assigned, protected, and reviewable.

A company should leave this section able to say:

“We know which devices access our systems, who owns them, whether they are protected, whether they are encrypted, whether they are patched, and what happens if they are lost or compromised.”

That is endpoint, server, and mobile device protection.


------

