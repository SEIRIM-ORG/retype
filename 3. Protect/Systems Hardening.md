---
icon: triangle-right
order: 70
---
## Systems Hardening and Secure Configuration

### Goal

Systems hardening means reducing the ways a system can be misused, attacked, or exposed.

The work is practical. Remove what is not needed. Turn on safer settings. Close weak defaults. Restrict risky features. Apply a clear baseline. Check the baseline again over time.

This section covers laptops, desktops, servers, cloud platforms, SaaS tools, browsers, network equipment, websites, databases, remote access systems, and administrative tools.

Hardening does not replace patching, monitoring, backup, or incident response. It makes those other controls work better by giving attackers fewer easy paths in.

## Step 1: Choose the Hardening Baseline

Start with a known baseline. Do not invent every setting from scratch.

**Use one or more of these:**

|Baseline or Checklist|Link|Best Use|
|---|---|---|
|CIS Benchmarks|[CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks)|Secure configuration guides for operating systems, cloud platforms, browsers, network devices, databases, and SaaS tools.|
|Microsoft Security Baselines|[Microsoft Security Baselines](https://learn.microsoft.com/en-us/windows/security/operating-system-security/device-management/windows-security-configuration-framework/windows-security-baselines)|Windows, Windows Server, Microsoft Edge, Microsoft 365 Apps, and Microsoft security configuration guidance.|
|Microsoft Security Compliance Toolkit|[Microsoft Security Compliance Toolkit](https://www.microsoft.com/en-us/download/details.aspx?id=55319)|Download, compare, test, and manage Microsoft security baselines.|
|Google Workspace Security Checklists|[Google Workspace Security Checklists](https://knowledge.workspace.google.com/admin/security/security-checklists)|Google Workspace and Cloud Identity admin security checklist.|
|CISA Cybersecurity Performance Goals|[CISA CPG 2.0](https://www.cisa.gov/cybersecurity-performance-goals-2-0-cpg-2-0)|High-impact baseline security practices for organizations.|
|NSA Cybersecurity Guidance|[NSA Cybersecurity Advisories and Guidance](https://www.nsa.gov/Press-Room/Cybersecurity-Advisories-Guidance/)|Hardening guidance for higher-security environments and common enterprise technologies.|
|DISA STIGs|[DISA STIGs](https://public.cyber.mil/stigs/)|Strict configuration guides, mainly for regulated or government-related environments.|

For most SMEs, start with CIS Benchmarks, Microsoft Security Baselines, Google Workspace checklists, and CISA Cybersecurity Performance Goals.

Do not apply every setting blindly. Test changes before applying them widely.

## Step 2: Create a Hardening Register

Track the systems that need hardening.

**Use a simple register.**

|Field|What to Record|
|---|---|
|System Name|Laptop group, server, firewall, SaaS platform, website, database, cloud account|
|System Type|Windows, macOS, Linux, firewall, router, SaaS, cloud, database, website|
|Business Owner|Department or person responsible|
|Technical Owner|IT, MSP, vendor, or administrator|
|Baseline Used|CIS, Microsoft, Google, vendor checklist, internal standard|
|Current Status|Not started, in progress, hardened, exception, needs review|
|Main Gaps|Weak settings, unused services, exposed ports, old protocols, missing encryption|
|Last Review Date|Date last checked|
|Next Review Date|Date next review is due|
|Evidence Location|Screenshot, report, exported configuration, checklist, ticket|

The register keeps the work from becoming random.

## Step 3: Harden New Systems Before Use

Do not wait until after a system is already in production.

Before a new laptop, server, cloud platform, SaaS tool, website, or network device is used, apply the standard configuration.

**Check:**

|Area|Required Check|
|---|---|
|Default accounts|Removed, disabled, or changed|
|Admin access|Limited to approved administrators|
|MFA|Enabled where supported|
|Passwords|Unique and stored in approved password manager|
|Updates|Current before deployment|
|Encryption|Enabled where supported|
|Logging|Turned on where available|
|Remote access|Disabled unless required|
|Unused services|Disabled|
|Unused software|Removed|
|Security tools|Installed and active|
|Backup coverage|Confirmed where applicable|
|Owner|Assigned|
|Documentation|Stored in the hardening register|

A system should not go live until the basic hardening checks are complete.

## Step 4: Remove Default and Unused Accounts

Default accounts are a common weakness.

**Check:**

|Place to Check|What to Do|
|---|---|
|Windows local accounts|Disable unused local accounts and manage local admin passwords|
|macOS local accounts|Remove old admin accounts and unused users|
|Linux local accounts|Disable unused users, default users, and unnecessary shell access|
|Firewalls and routers|Remove default admin accounts where possible|
|SaaS admin portals|Remove test admins and old setup accounts|
|Website CMS|Remove default admin names and old developer accounts|
|Databases|Remove sample, test, and unused database accounts|
|Applications|Remove demo users and vendor setup accounts|

No system should keep a default password.

No system should keep an old setup account “just in case.”

## Step 5: Restrict Administrator Rights

Normal users should not have administrator rights for daily work.

**Check:**

|Area|What to Check|
|---|---|
|Windows laptops|Local admin removed from normal users|
|macOS devices|Standard users used for daily work|
|Linux systems|Sudo access limited to approved admins|
|Servers|Admin rights limited to named administrators|
|SaaS platforms|Admin roles limited and reviewed|
|Cloud platforms|Root or owner access restricted|
|Website CMS|Administrator roles limited|
|Databases|DBA and root-level roles limited|
|Network devices|Admin access limited to approved personnel|

Admin access should be named, justified, and reviewed.

## Step 6: Enable Device Encryption

Enable encryption on company devices and systems that store business data.

**Check:**

|System|Common Option|
|---|---|
|Windows|BitLocker|
|macOS|FileVault|
|Linux|LUKS or approved disk encryption|
|Mobile devices|Built-in device encryption|
|External drives|Hardware encryption or approved encrypted volumes|
|Cloud storage|Provider encryption and access controls|
|Backup media|Backup encryption|

Store recovery keys securely.

Do not leave recovery keys only on the device they protect.

## Step 7: Harden Workstations and Laptops

Company workstations and laptops need a standard build.

**Check:**

|Setting Area|Required Check|
|---|---|
|Operating system|Supported version only|
|Updates|Automatic updates enabled where appropriate|
|Endpoint protection|Installed and active|
|Firewall|Enabled|
|Disk encryption|Enabled|
|Screen lock|Enabled with short timeout|
|Local admin|Removed from normal users|
|Browser|Managed settings applied|
|Password storage|Browser password saving restricted where appropriate|
|USB storage|Restricted where needed|
|Remote access|Disabled unless approved|
|Personal software|Restricted|
|Unapproved tools|Removed|
|Macro behavior|Restricted|
|Script execution|Restricted where appropriate|
|RDP|Disabled unless approved|
|File sharing|Disabled unless needed|
|Printer sharing|Disabled unless needed|
|Bluetooth|Disabled or restricted where not needed|
|Developer tools|Approved only where needed|
|Logging|Enabled and forwarded where possible|

Do not let every laptop become a custom island.

Use standard configurations.

## Step 8: Harden Windows Systems

Windows environments need special attention because they are common targets.

**Check:**

|Windows Area|What to Check|
|---|---|
|Local admin passwords|Use Windows LAPS where possible|
|SMB|Disable SMBv1|
|RDP|Disable by default; restrict if required|
|PowerShell|Logging enabled; risky use restricted where appropriate|
|Windows Defender|Enabled if no other EDR is used|
|Firewall|Enabled on all profiles|
|BitLocker|Enabled on laptops|
|Autorun and AutoPlay|Disabled where appropriate|
|Macros|Block internet-sourced macros where possible|
|Credential storage|Reduce cached credential exposure|
|Guest account|Disabled|
|Remote registry|Disabled unless required|
|Windows Script Host|Restricted where appropriate|
|UAC|Enabled|
|Event logging|Enabled and retained|
|Security baselines|Apply Microsoft or CIS baseline|
|Legacy protocols|Disable where possible|
|Unneeded services|Disabled|

Use Microsoft Security Baselines or CIS Windows Benchmarks as the standard reference.

## Step 9: Harden macOS Systems

Mac devices also need a standard configuration.

**Check:**

|macOS Area|What to Check|
|---|---|
|FileVault|Enabled|
|Firewall|Enabled|
|Automatic updates|Enabled or centrally managed|
|Admin accounts|Limited|
|Screen lock|Enabled|
|Gatekeeper|Enabled|
|System Integrity Protection|Enabled|
|Remote login|Disabled unless approved|
|Remote management|Restricted|
|Sharing services|Disabled unless needed|
|Browser security|Managed where possible|
|MDM|Used where available|
|iCloud sync|Controlled for company data|
|Local accounts|Reviewed|
|Lost device process|Documented|

For larger Mac fleets, use an MDM.

## Step 10: Harden Linux Servers

Linux systems need consistent baseline settings.

**Check:**

|Linux Area|What to Check|
|---|---|
|SSH|Key-based access preferred; root login disabled|
|Sudo|Limited to approved administrators|
|Firewall|Enabled and restricted|
|Open ports|Only required ports allowed|
|Unused packages|Removed|
|Unused services|Disabled|
|Updates|Managed and current|
|Logs|Enabled and retained|
|Time sync|Enabled|
|File permissions|Reviewed on sensitive paths|
|Kernel hardening|Apply baseline settings where appropriate|
|SELinux or AppArmor|Enabled where practical|
|Password authentication|Disabled for SSH where possible|
|Fail2ban or equivalent|Used where suitable|
|Audit logging|Enabled on important servers|
|Cron jobs|Reviewed|
|Service accounts|Documented|
|Backup agent|Configured where needed|

Use CIS Linux Benchmarks, Lynis, OpenSCAP, or DevSec hardening roles to guide the work.

## Step 11: Harden Servers and Virtual Machines

Servers need stricter controls than normal endpoints.

**Check:**

|Server Area|What to Check|
|---|---|
|Server role|Clearly defined|
|Installed software|Only required software installed|
|Open ports|Only required ports exposed|
|Admin access|Limited and named|
|Service accounts|Documented and restricted|
|Firewall|Enabled|
|Logging|Enabled and sent to central location where possible|
|Backup|Confirmed|
|Time sync|Enabled|
|Security tools|Installed where supported|
|Remote access|Restricted|
|Internet exposure|Avoided unless required|
|Configuration baseline|Applied|
|Test systems|Separated from production|
|Old snapshots|Removed or controlled|
|Default services|Disabled|
|Unused shares|Removed|

Do not use a server for unrelated roles because it is convenient.

A file server, database server, web server, and backup server should not be mixed casually.

## Step 12: Harden Active Directory or Directory Services

If the company uses Active Directory, it must be hardened carefully.

**Check:**

|Directory Area|What to Check|
|---|---|
|Domain admins|Limited to the smallest possible number|
|Admin accounts|Separate from daily accounts|
|Old users|Disabled or removed|
|Old computers|Reviewed and removed|
|Group Policy|Reviewed and documented|
|Password policy|Enforced|
|Lockout policy|Configured|
|LAPS|Used for local admin passwords|
|Legacy protocols|Disabled where possible|
|NTLM|Reduced where possible|
|LDAP signing|Enabled where appropriate|
|Kerberos settings|Reviewed|
|Service accounts|Documented and restricted|
|Privileged groups|Reviewed|
|Default groups|Reviewed|
|DNS admin rights|Limited|
|Domain controllers|Protected and monitored|
|Backups|Confirmed for domain recovery|
|Time sync|Healthy|
|Admin workstations|Used for high-risk administration where possible|

Domain controllers are high-value systems. Treat them that way.

## Step 13: Harden Microsoft 365

Microsoft 365 is a major business platform and a major attack target.

**Check:**

|Microsoft 365 Area|What to Check|
|---|---|
|MFA|Required for all users, stronger for admins|
|Security defaults|Enabled if suitable|
|Conditional access|Used where licensing allows|
|Admin roles|Limited and reviewed|
|Global admins|Kept to a very small number|
|Legacy authentication|Disabled|
|Mail forwarding|External forwarding restricted or monitored|
|Audit logging|Enabled|
|SharePoint sharing|External sharing controlled|
|OneDrive sharing|External sharing controlled|
|Teams guests|Controlled|
|OAuth apps|Reviewed|
|App consent|Restricted|
|DKIM|Enabled|
|DMARC|Configured|
|SPF|Configured|
|Anti-phishing policies|Enabled where available|
|Safe links and attachments|Used where licensing allows|
|Password reset|Secured|
|Break-glass accounts|Protected and documented|
|Secure Score|Reviewed regularly|

Do not assume Microsoft 365 is secure by default for every business need.

## Step 14: Harden Google Workspace

Google Workspace also needs deliberate configuration.

**Check:**

|Google Workspace Area|What to Check|
|---|---|
|2-Step Verification|Enforced for all users|
|Admin accounts|Limited and reviewed|
|Super admins|Kept to a very small number|
|Context-aware access|Used where available|
|Login challenges|Enabled|
|External sharing|Controlled|
|Drive sharing|Restricted by business need|
|Shared drives|Owned and reviewed|
|OAuth apps|Reviewed and restricted|
|Third-party app access|Controlled|
|Gmail authentication|SPF, DKIM, and DMARC configured|
|Email routing rules|Reviewed|
|Groups|Reviewed for public or external exposure|
|Mobile management|Enabled where appropriate|
|Audit logs|Reviewed|
|Security center|Used where available|
|Recovery settings|Secured|
|Suspicious login alerts|Enabled|
|Data export permissions|Restricted|

Do not let employees approve unknown third-party apps without review.

## Step 15: Harden SaaS Platforms

Every business-critical SaaS tool needs a basic security check.

**Check:**

|SaaS Area|What to Check|
|---|---|
|Admin users|Named and limited|
|MFA|Enabled|
|SSO|Enabled where possible|
|Guest access|Reviewed|
|External sharing|Restricted|
|Public links|Disabled or controlled|
|API keys|Documented and rotated|
|OAuth apps|Reviewed|
|Audit logs|Enabled where available|
|Data export rights|Limited|
|Password policy|Enforced if no SSO|
|Vendor support access|Controlled|
|Default settings|Reviewed|
|Old users|Removed|
|Integrations|Reviewed|
|Billing admins|Controlled|
|Backup or export options|Known|

Apply this to CRM, accounting, HR, payroll, project management, ticketing, e-commerce, marketing, file storage, and collaboration platforms.

## Step 16: Harden Cloud Accounts

Cloud platforms need strong guardrails.

**Check:**

|Cloud Area|What to Check|
|---|---|
|Root account|Protected with MFA and not used for daily work|
|Admin roles|Limited|
|IAM permissions|Least privilege|
|Public storage|Blocked unless approved|
|Security logging|Enabled|
|Network exposure|Restricted|
|Security groups|Reviewed|
|Default VPCs|Reviewed|
|Unused resources|Removed|
|Secrets|Stored in approved secrets manager|
|Keys|Rotated and restricted|
|Object storage|Versioning and protection where needed|
|Snapshots|Protected|
|Databases|Not publicly exposed unless approved|
|Backups|Enabled where required|
|Billing alerts|Enabled|
|Regions|Limited where possible|
|Infrastructure as code|Used where practical|

Cloud errors can expose data fast. Review default settings carefully.

## Step 17: Harden Network Devices

Firewalls, routers, switches, VPNs, and Wi-Fi equipment are often missed.

**Check:**

|Network Device Area|What to Check|
|---|---|
|Default passwords|Changed|
|Admin access|Limited|
|MFA|Enabled where supported|
|Firmware|Current|
|Remote admin|Disabled from internet unless required and protected|
|Management interface|Restricted to admin network|
|Unused services|Disabled|
|SNMP|Disabled or secured|
|Telnet|Disabled|
|SSH|Preferred over Telnet|
|HTTPS management|Used where possible|
|Logging|Enabled and exported where possible|
|Configuration backups|Saved after changes|
|Guest Wi-Fi|Separated from business network|
|Wi-Fi encryption|WPA2/WPA3|
|Old VPN users|Removed|
|Firewall rules|Reviewed|
|Open ports|Reviewed|
|UPnP|Disabled where possible|
|DNS settings|Controlled|

Network devices are not “set and forget.”

## Step 18: Harden Remote Access

Remote access must be tightly controlled.

**Check:**

|Remote Access Area|What to Check|
|---|---|
|VPN|MFA required|
|RDP|Not exposed directly to the internet|
|Remote support tools|Approved and controlled|
|Vendor access|Named accounts only|
|Split tunneling|Reviewed|
|Device posture|Checked where available|
|Geo restrictions|Used where appropriate|
|Idle timeout|Enabled|
|Session logging|Enabled where possible|
|Old users|Removed|
|Emergency access|Documented|
|Personal devices|Restricted or controlled|

Do not expose RDP directly to the internet.

Do not allow unmanaged remote support tools without approval.

## Step 19: Harden Browsers

The browser is now one of the main work tools.

**Check:**

|Browser Area|What to Check|
|---|---|
|Browser updates|Automatic updates enabled|
|Extensions|Restricted to approved extensions|
|Password saving|Disabled or controlled where company password manager is used|
|Pop-ups|Restricted|
|Dangerous downloads|Blocked where possible|
|Safe browsing|Enabled|
|Site permissions|Reviewed|
|Autofill|Controlled|
|Sync|Controlled for company accounts|
|Developer tools|Limited where appropriate|
|Third-party cookies|Controlled where practical|
|Default browser|Standardized where practical|

Browser extensions can become a serious risk. Review them.

## Step 20: Harden Website and CMS Platforms

Company websites are often forgotten after launch.

**Check:**

|Website Area|What to Check|
|---|---|
|CMS version|Current|
|Plugins and themes|Current and necessary|
|Unused plugins|Removed|
|Admin users|Limited|
|MFA|Enabled where supported|
|Default admin usernames|Removed|
|File permissions|Reviewed|
|Web application firewall|Used where appropriate|
|Admin login URL|Restricted where possible|
|Backups|Confirmed|
|Staging site|Protected|
|Debug mode|Disabled in production|
|Database access|Restricted|
|HTTPS|Enforced|
|TLS settings|Current|
|Security headers|Added where appropriate|
|Upload forms|Restricted and scanned where possible|
|Contact forms|Protected from abuse|
|Public directories|Reviewed|
|Error messages|Do not expose sensitive details|

Websites are public-facing systems. Treat them as exposed assets.

## Step 21: Harden Databases

Databases often hold sensitive data.

**Check:**

|Database Area|What to Check|
|---|---|
|Public exposure|Disabled unless formally approved|
|Admin accounts|Limited|
|Default accounts|Removed or disabled|
|Passwords|Strong and stored securely|
|Encryption|Enabled where supported|
|Backups|Confirmed|
|Logging|Enabled|
|Test databases|Protected|
|Sample data|Removed|
|Least privilege|Applied to applications and users|
|Network access|Restricted|
|Remote access|Limited|
|Database versions|Supported|
|Unused databases|Removed|
|Stored procedures|Reviewed where needed|
|Export permissions|Limited|
|Service accounts|Documented|

Do not leave old databases running because nobody is sure what they do.

## Step 22: Harden Printers, Cameras, and IoT Devices

Small devices are commonly ignored.

**Check:**

|Device Area|What to Check|
|---|---|
|Default passwords|Changed|
|Firmware|Updated|
|Internet access|Blocked unless required|
|Admin interface|Restricted|
|Unused services|Disabled|
|Cloud access|Reviewed|
|Guest access|Disabled|
|Network segment|Separated where possible|
|Logging|Enabled where available|
|Old devices|Removed|
|Vendor support access|Controlled|

Printers, cameras, door systems, and IoT devices should not sit on the same flat network as business systems where avoidable.

## Step 23: Harden Developer and Code Environments

If the company writes code or manages websites, developer environments need attention.

**Check:**

|Developer Area|What to Check|
|---|---|
|Code repositories|Private by default|
|Branch protection|Enabled where appropriate|
|Secrets scanning|Enabled|
|API keys|Not stored in code|
|Personal access tokens|Limited and rotated|
|Admin access|Limited|
|CI/CD secrets|Stored securely|
|Build runners|Secured|
|Dependencies|Reviewed|
|Package publishing rights|Limited|
|Webhooks|Reviewed|
|Old repositories|Archived or removed|
|Developer laptops|Hardened|
|SSH keys|Managed and reviewed|

One leaked token can become a full system compromise.

## Step 24: Harden Logging and Time Settings

Hardening includes making sure systems record useful events.

**Check:**

|Logging Area|What to Check|
|---|---|
|Time sync|Enabled on all systems|
|Security logs|Enabled|
|Admin actions|Logged where possible|
|Login events|Logged|
|Failed login events|Logged|
|Configuration changes|Logged|
|Cloud audit logs|Enabled|
|SaaS audit logs|Enabled where available|
|Network device logs|Exported where possible|
|Log retention|Defined|
|Log deletion|Restricted|

Detection belongs in the Detect section, but systems need logging enabled here.

## Step 25: Create Standard Build Checklists

Create standard hardening checklists for the systems the company uses most.

**Suggested checklists:**

|Checklist|Use|
|---|---|
|Windows laptop build checklist|New and rebuilt Windows devices|
|macOS laptop build checklist|New and rebuilt Mac devices|
|Linux server checklist|New Linux servers|
|Windows Server checklist|New Windows servers|
|Microsoft 365 checklist|Microsoft tenant review|
|Google Workspace checklist|Google tenant review|
|SaaS checklist|CRM, HR, payroll, accounting, project tools|
|Firewall checklist|Firewall and router review|
|Website checklist|CMS and hosting review|
|Database checklist|Database review|
|Cloud account checklist|AWS, Azure, Google Cloud, or other platforms|

Keep the checklists short enough that people will actually use them.

## Step 26: Test Hardening Before Full Rollout

Hardening can break workflows if applied carelessly.

**Before broad rollout:**

|Test Area|What to Do|
|---|---|
|Pilot group|Test with a small set of users|
|Business apps|Confirm key apps still work|
|Login process|Confirm users can access required systems|
|Printing and scanning|Test if needed|
|Remote work|Test VPN and remote tools|
|File sharing|Confirm permissions still work|
|Browser apps|Test common web apps|
|Backup agents|Confirm backup still runs|
|Security tools|Confirm monitoring still works|
|Rollback plan|Prepare a way to undo harmful changes|

Security settings that break business operations will be bypassed.

Test first.

## Step 27: Record Exceptions

Some settings cannot be applied immediately.

**Record every exception.**

|Exception Field|What to Record|
|---|---|
|System|Affected system|
|Setting|Hardening control not applied|
|Reason|Business, technical, vendor, compatibility, legacy|
|Risk|What exposure remains|
|Temporary control|Compensating measure|
|Owner|Person responsible|
|Expiration date|When it must be reviewed|
|Approval|Who accepted the exception|

No exception should last forever without review.

## Step 28: Review Hardening Regularly

Hardening is not a one-time project.

**Review:**

|Review Area|Frequency|
|---|---|
|Critical systems|Quarterly|
|Internet-facing systems|Monthly or after major changes|
|SaaS admin settings|Quarterly|
|Laptops and endpoints|Quarterly or through device management|
|Servers|Quarterly|
|Network devices|Quarterly and after firmware changes|
|Websites|Monthly or before major changes|
|Cloud platforms|Monthly or quarterly|
|Exceptions|Monthly or quarterly|

Every major change should trigger a hardening review.

**Examples:**

- New SaaS platform
- New server
- New office
- New firewall
- New website
- New vendor
- New cloud account
- New remote access tool
- Major software upgrade
- Security incident

## Step 29: Keep Evidence

Store proof that hardening was completed.

**Useful evidence includes:**

|Evidence Type|Example|
|---|---|
|Checklist|Completed hardening checklist|
|Screenshot|Security setting screenshot|
|Export|Firewall, router, GPO, SaaS, or cloud configuration export|
|Report|CIS-CAT, Lynis, OpenSCAP, Secure Score, or other report|
|Ticket|Change ticket showing completed work|
|Approval|Exception approval|
|Review log|Date and reviewer|
|Baseline file|Security baseline used|
|Test record|Pilot test results|
|Rollback record|Rollback notes if needed|

If the company cannot prove a system was hardened, assume it needs review.

## Places Commonly Missed

|Missed Area|What to Check|
|---|---|
|Domain registrar|MFA, admin users, DNS change access, recovery email|
|DNS provider|MFA, admin users, old records, API keys|
|Website hosting|Admin accounts, SFTP, backups, PHP versions, database access|
|Old websites|Forgotten microsites, staging sites, test domains|
|Former employee folders|Shared links, ownership, access|
|Mail forwarding rules|External forwarding and hidden rules|
|Public cloud links|SharePoint, OneDrive, Google Drive, Dropbox, Box|
|OAuth apps|Apps connected to Microsoft 365, Google Workspace, CRM|
|Browser extensions|Unapproved extensions with data access|
|Local admin accounts|Laptops, desktops, servers|
|Backup consoles|Admin access, MFA, deletion protection|
|Printers|Default passwords, scan-to-email, address books|
|Cameras and NVRs|Default passwords, internet exposure|
|Wi-Fi|Guest separation, old passwords, WPA settings|
|Firewall rules|Old port forwards, temporary rules never removed|
|VPN accounts|Old users and vendors|
|RDP|Direct internet exposure|
|SaaS exports|Who can export large data sets|
|API keys|Old keys and broad permissions|
|Developer repositories|Secrets, public repos, old tokens|
|Test systems|Weak passwords, exposed admin panels|
|Shadow IT|Apps bought directly by departments|
|Shared mailboxes|Delegates, forwarding, old access|
|Service accounts|Broad permissions and no owner|
|Old vendors|Accounts still active|

## Recommended Tools and Checklists

|Tool or Resource|Link|Type|Best Use|
|---|---|---|---|
|CIS Benchmarks|[CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks)|Free for non-commercial PDF use, paid tooling available|Secure configuration checklists for many platforms|
|CIS-CAT Lite|[CIS-CAT Lite](https://learn.cisecurity.org/cis-cat-lite)|Free|Assess configuration against selected CIS Benchmarks|
|CIS-CAT Pro|[CIS-CAT Pro](https://www.cisecurity.org/cybersecurity-tools/cis-cat-pro)|Paid|More complete CIS benchmark assessment and reporting|
|Microsoft Security Baselines|[Microsoft Security Baselines](https://learn.microsoft.com/en-us/windows/security/operating-system-security/device-management/windows-security-configuration-framework/windows-security-baselines)|Free|Microsoft-recommended secure settings|
|Microsoft Security Compliance Toolkit|[Microsoft Security Compliance Toolkit](https://www.microsoft.com/en-us/download/details.aspx?id=55319)|Free|Compare and manage Microsoft security baselines|
|Microsoft Intune|[Microsoft Intune](https://www.microsoft.com/security/business/endpoint-management/microsoft-intune)|Commercial, often included in Microsoft plans|Device configuration, compliance policies, endpoint hardening|
|Microsoft Secure Score|[Microsoft Secure Score](https://learn.microsoft.com/en-us/defender-xdr/microsoft-secure-score)|Included with Microsoft security portals|Review Microsoft security posture and recommendations|
|Google Workspace Security Checklists|[Google Workspace Security Checklists](https://knowledge.workspace.google.com/admin/security/security-checklists)|Free guidance|Google Workspace hardening checklist|
|Google Admin Security Center|[Google Workspace Security Center](https://support.google.com/a/answer/7492330)|Included depending on edition|Google Workspace security dashboard and investigation features|
|Lynis|[Lynis](https://cisofy.com/lynis/)|Open-source|Linux, macOS, and Unix hardening audits|
|OpenSCAP|[OpenSCAP](https://www.open-scap.org/)|Open-source|Compliance and configuration assessment using SCAP content|
|SCAP Security Guide|[ComplianceAsCode](https://github.com/ComplianceAsCode/content)|Open-source|Security policies for Linux systems using SCAP|
|DevSec Hardening Framework|[DevSec Hardening Framework](https://github.com/dev-sec)|Open-source|Hardening baselines and automation for Linux and services|
|HardeningKitty|[HardeningKitty](https://github.com/0x6d69636b/windows_hardening)|Open-source|Windows hardening auditing and checklist-based review|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|Security monitoring, configuration assessment, compliance support|
|osquery|[osquery](https://www.osquery.io/)|Open-source|Query endpoint configuration and system state|
|Ansible|[Ansible Community](https://www.ansible.com/community)|Open-source|Automate Linux and server configuration|
|PowerShell DSC|[PowerShell DSC](https://learn.microsoft.com/en-us/powershell/dsc/overview)|Free|Configure and enforce Windows and some cross-platform settings|
|Windows LAPS|[Windows LAPS](https://learn.microsoft.com/en-us/windows-server/identity/laps/laps-overview)|Included in Windows environments|Manage local administrator passwords|
|GPOZaurr|[GPOZaurr](https://github.com/EvotecIT/GPOZaurr)|Open-source|Review and clean up Group Policy environments|
|PingCastle|[PingCastle](https://www.pingcastle.com/)|Free/community and commercial options|Active Directory security assessment|
|Purple Knight|[Purple Knight](https://www.semperis.com/purple-knight/)|Free|Active Directory and Entra ID security assessment|
|ScoutSuite|[ScoutSuite](https://github.com/nccgroup/ScoutSuite)|Open-source|Cloud security posture review for AWS, Azure, Google Cloud, and others|
|Prowler|[Prowler](https://prowler.com/)|Open-source and commercial|Cloud security assessment, especially AWS, Azure, Google Cloud, Kubernetes|
|Steampipe|[Steampipe](https://steampipe.io/)|Open-source|Query cloud, SaaS, and infrastructure configuration|
|Trivy|[Trivy](https://trivy.dev/)|Open-source|Scan containers, infrastructure as code, repositories, and configurations|
|kube-bench|[kube-bench](https://github.com/aquasecurity/kube-bench)|Open-source|Kubernetes CIS benchmark checks|
|kube-hunter|[kube-hunter](https://github.com/aquasecurity/kube-hunter)|Open-source|Kubernetes security testing|
|WPScan|[WPScan](https://wpscan.com/)|Free and commercial options|WordPress security scanning|
|Mozilla Observatory|[Mozilla Observatory](https://observatory.mozilla.org/)|Free|Website security header checks|
|Security Headers|[Security Headers](https://securityheaders.com/)|Free|Website security header checks|
|SSL Labs Server Test|[SSL Labs SSL Test](https://www.ssllabs.com/ssltest/)|Free|TLS and HTTPS configuration testing|
|Nmap|[Nmap](https://nmap.org/)|Open-source|Identify open ports and exposed services|
|Hardenize|[Hardenize](https://www.hardenize.com/)|Free and paid options|Internet-facing domain, TLS, email, and DNS security review|
|Internet.nl|[Internet.nl](https://internet.nl/)|Free|Test website, email, and connection standards|
|OpenVAS / Greenbone Community Edition|[Greenbone Community Edition](https://greenbone.github.io/docs/latest/)|Open-source|Vulnerability and configuration visibility for networks and systems|
|GLPI|[GLPI](https://glpi-project.org/)|Open-source|IT asset and configuration tracking|
|Snipe-IT|[Snipe-IT](https://snipeitapp.com/)|Open-source and hosted options|Device and asset tracking|
|Excel|[Microsoft Excel](https://www.microsoft.com/microsoft-365/excel)|Low-cost|Hardening register and checklist tracking|
|Google Sheets|[Google Sheets](https://www.google.com/sheets/about/)|Low-cost|Shared hardening tracker|

## Practical Tool Stack for SMEs

### Very small company:

- Microsoft Secure Score or Google Workspace security checklist
- CIS Benchmarks
- Excel or Google Sheets hardening register
- SSL Labs, Security Headers, Internet.nl, and Mozilla Observatory for websites and domains
- Nmap for basic exposed-service review

### Small Microsoft-based company:

- Microsoft Security Baselines
- Microsoft Security Compliance Toolkit
- Microsoft Intune
- Microsoft Secure Score
- Windows LAPS
- HardeningKitty
- PingCastle or Purple Knight for Active Directory and Entra ID review

### Small Google Workspace company:

- Google Workspace Security Checklists
- Google Admin Security Center where available
- Google Admin audit logs
- Hardenize, Internet.nl, SSL Labs, and Security Headers for public-facing services

### Linux or self-hosted company:

- CIS Linux Benchmarks
- Lynis
- OpenSCAP
- DevSec Hardening Framework
- Ansible
- Wazuh
- Nmap
- OpenVAS / Greenbone Community Edition

### Cloud-heavy company:

- Prowler
- ScoutSuite
- Steampipe
- Trivy
- CIS Cloud Benchmarks
- Provider-native security tools

### Website-heavy company:

- WPScan for WordPress
- SSL Labs
- Mozilla Observatory
- Security Headers
- Internet.nl
- Hardenize
- CMS vendor checklists

## Systems Hardening Register Template

|Field|What to Record|
|---|---|
|System|Name of laptop group, server, SaaS, firewall, website, cloud account, or database|
|Type|Windows, macOS, Linux, SaaS, cloud, network device, website, database|
|Owner|Business owner and technical owner|
|Baseline|CIS, Microsoft, Google, vendor checklist, internal standard|
|Hardening Status|Not started, in progress, hardened, exception, review needed|
|Key Settings Applied|Short summary|
|Missing Settings|Known gaps|
|Exception|Yes or no|
|Evidence|Report, screenshot, export, checklist, ticket|
|Last Review|Date|
|Next Review|Date|
|Priority|Critical, High, Medium, Low|

## Expected Outputs from This Section

At the end of this section, the company should have:

- A selected hardening baseline.
- A systems hardening register.
- Standard build checklists for common system types.
- Hardened workstation and laptop settings.
- Hardened server settings.
- Hardened Microsoft 365 or Google Workspace settings.
- Hardened SaaS admin settings.
- Hardened cloud account settings.
- Hardened network device settings.
- Hardened remote access settings.
- Hardened website and CMS settings.
- Hardened database settings.
- A list of missed or unmanaged systems.
- A list of hardening exceptions.
- Evidence showing what was checked and changed.
- A review schedule.


## Objectives

- Do not leave systems with factory settings.

- Do not keep features nobody uses.

- Do not keep admin access because it is convenient.

- Do not assume SaaS defaults are safe.

- Do not forget network devices, websites, browsers, printers, and old systems.

**A company should leave this section able to say:**

“We know which systems need hardening, which baseline we use, what settings have been applied, what exceptions remain, and when each system was last reviewed.”


----

