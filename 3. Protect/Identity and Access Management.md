---
icon: triangle-right
order: 90
---

### Goal

Identity and Access Management controls who can access company systems, what they can access, and what they are allowed to do.

This is one of the most important parts of the Protect section. Many attacks do not begin with malware. They begin with a login. A stolen password. A reused password. An old account. A weak admin account. A vendor account nobody reviewed. A fake MFA reset request. A shared password sitting in a spreadsheet.

**The goal is simple:**

Only the right people should have access to the right systems, for the right reason, at the right level, for the right amount of time.

## Step 1: Assign IAM Ownership

Assign clear ownership for identity and access management.

The company needs one person or role responsible for keeping this process alive. This may be the IT lead, MSP contact, operations manager, security lead, or another assigned owner.

**Record the following:**

|Item|Record|
|---|---|
|IAM owner|Person responsible for the process|
|Executive sponsor|Leadership owner for decisions and enforcement|
|IT or MSP owner|Person or provider implementing changes|
|Department approvers|People who approve access for each business area|
|Review frequency|Monthly, quarterly, or another fixed schedule|

Access decisions should not be left to informal messages or memory.

## Step 2: Define the Access Rules

Create simple rules for how access is granted, changed, and removed.

**The rules should cover:**

- No access without approval.

- No shared accounts unless formally approved.

- No elevated admin access for normal daily work not requiring that level of privileges for the task at hand.

- No permanent vendor access unless there is a clear business need.

- No former employee accounts left active.

- No MFA exceptions without written approval.

- No password storage in spreadsheets, browsers, chat messages, or email.

- No personal email accounts used for company systems.

- No user receives more access than needed for their role.

The company should write these rules in plain language and make them part of normal operations.

## Step 3: Centralize Identity Where Possible

Use one main identity system wherever possible.

For many SMEs, this will be Microsoft Entra ID through Microsoft 365 or Google Workspace identity through Google Workspace. For technical teams or self-hosted environments, this may include Keycloak, authentik, Authelia, FreeIPA, or another identity provider.

The goal is to reduce scattered logins. The more separate accounts the company has, the harder it becomes to control access.

Record which system is the main identity source:

|Identity Area|Primary System|
|---|---|
|Employee login|Microsoft 365, Google Workspace, or other|
|SaaS login|SSO where available|
|Admin login|Dedicated admin accounts|
|Linux/server login|FreeIPA, directory service, SSH controls, or other|
|Self-hosted apps|Keycloak, authentik, Authelia, or other|
|Vendor login|Named vendor accounts, not shared accounts|

Where single sign-on is available, use it for important systems.

## Step 4: Enforce MFA on Critical Systems

Multi-factor authentication must be enabled on critical systems.

**Start with:**

|System Type|MFA Requirement|
|---|---|
|Email|Required|
|Microsoft 365 or Google Workspace|Required|
|VPN and remote access|Required|
|Admin accounts|Required|
|Accounting and payroll|Required|
|CRM|Required|
|Cloud storage|Required|
|Password manager|Required|
|Domain registrar and DNS|Required|
|Website admin accounts|Required|
|Backup systems|Required|
|Security tools|Required|
|Vendor portals|Required where available|

Use stronger MFA for administrators and high-risk users. Hardware security keys or passkeys are better than SMS codes.

Emergency exceptions must be documented, approved, time-limited, and reviewed.

## Step 5: Deploy a Password Manager

The company should use an approved password manager for all business passwords.

The password manager should be used to facilitate:

- Unique passwords
- Long random passwords
- Shared team credentials where unavoidable
- Secure password sharing
- Admin credentials
- Vendor portal credentials
- Recovery codes
- Emergency access records

Passwords should not be stored in spreadsheets, notebooks, browsers, chat apps, email, or personal password vaults.

**The company should define:**

|Password Manager Item|Requirement|
|---|---|
|Approved tool|Name of the company-approved password manager|
|MFA|Required for all password manager users|
|Admin access|Limited to assigned administrators|
|Shared vaults|Organized by team or system|
|Personal vaults|Separated from company vaults|
|Emergency access|Documented and tested|
|Offboarding|Company vault access removed immediately|

## Step 6: Use Least Privilege

Every user should have the lowest level of access needed to do their job.

This applies to employees, executives, contractors, vendors, administrators, and service accounts.

**For each important system, define standard access roles:**

|Role Type|Example|
|---|---|
|Viewer|Can read records only|
|Standard user|Can perform normal work|
|Power user|Can manage limited settings or team data|
|Administrator|Can manage users, settings, security, billing, or system configuration|
|Emergency admin|Used only during emergency access situations|
|Service account|Used by systems, integrations, automations, or scripts|

Do not give administrator access because it is convenient. Give it only when it is required.

## Step 7: Separate Admin Accounts from Daily User Accounts

Administrators should not use their normal everyday account for admin work.

**Each administrator should have:**

|Account Type|Use|
|---|---|
|Standard user account|Email, documents, normal daily work|
|Admin account|System administration only|
|Emergency admin account|Break-glass access only|

Admin accounts should have MFA, strong authentication, limited access, and higher monitoring. They should not be used for email, web browsing, or ordinary document work.

Break-glass accounts should be protected, documented, and reviewed regularly.

## Step 8: Remove or Restrict Shared Accounts

Shared accounts are dangerous because nobody can clearly prove who used the account.

The company should remove shared accounts wherever possible.

**Where a shared account cannot be removed immediately, document:**

|Shared Account Field|Record|
|---|---|
|System|Where the account is used|
|Business reason|Why it still exists|
|Users with access|Who can use it|
|Password storage|Approved password manager only|
|MFA status|Enabled where possible|
|Owner|Person responsible|
|Replacement plan|How the account will be removed|
|Review date|When it will be checked again|

Shared admin accounts should be treated as high risk.

## Step 9: Control Service Accounts and API Access

Service accounts are used by systems, scripts, integrations, automations, APIs, backup tools, monitoring tools, and SaaS connections.

These accounts are often forgotten which makes them dangerous.

**For each service account, record:**

|Service Account Field|Record|
|---|---|
|Account name|Name of the account|
|System|Where it is used|
|Purpose|What it does|
|Owner|Person responsible|
|Permissions|What access it has|
|Credential type|Password, key, token, certificate, API key|
|Storage location|Where the secret is stored|
|Rotation schedule|When the credential is changed|
|Last reviewed|Review date|
|Decommission plan|What happens when no longer needed|

Service accounts should not have broad admin rights unless absolutely required.

## Step 10: Protect Vendor and Contractor Access

Vendors and contractors should use named accounts. They should not use shared internal accounts.

Vendor access should be:

- Approved before use.
- Limited to the systems needed.
- Time-limited where possible.
- Protected with MFA.
- Removed when the work ends.
- Reviewed regularly.
- Logged where possible.

**The company should record:**

|Vendor Access Field|Record|
|---|---|
|Vendor name|Company or contractor|
|Business owner|Internal sponsor|
|Systems accessed|Systems or data they can access|
|Access level|User, admin, support, API, remote access|
|MFA status|Enabled or not available|
|Start date|When access began|
|End date|When access should end|
|Review date|Next review|
|Removal process|How access is terminated|

Do not allow permanent vendor access without a clear owner and review date.

## Step 11: Create a Joiner, Mover, Leaver Process

Access must change when people join, change roles, or leave.

**Use a simple process:**

|Event|Required Action|
|---|---|
|New employee joins|Create approved accounts based on role|
|Employee changes role|Remove old access and add new access|
|Employee leaves|Disable accounts immediately|
|Contractor starts|Create time-limited access|
|Contractor finishes|Remove access immediately|
|Vendor support ends|Remove vendor access|
|Emergency access used|Review and close after use|

Offboarding should include email, SaaS platforms, cloud storage, VPN, password manager, devices, admin tools, vendor portals, code repositories, and shared folders.

Do not only disable the main email account. That is not enough.

## Step 12: Review Access Regularly

Access reviews should happen on a fixed schedule.

For most SMEs, review critical systems quarterly and lower-risk systems at least annually.

**Review:**

- Email accounts
- Microsoft 365 or Google Workspace users
- Admin accounts
- Accounting and payroll users
- CRM users
- Cloud storage access
- Password manager users
- VPN and remote access users
- Website admin accounts
- Backup system users
- Security tool users
- Vendor accounts
- Former employees and contractors
- Shared accounts
- Service accounts

**The review should answer:**

- Who has access?
- Do they still need access?
- Is the access level correct?
- Is MFA enabled?
- Are any accounts inactive?
- Are there unknown users?
- Are there old vendor accounts?
- Are there shared accounts?
- Are there admin accounts that should be removed?

Record the review date, reviewer, findings, and actions taken.

## Step 13: Secure Account Recovery

Account recovery is often a weak point.

Attackers may not need a password if they can trick support staff into resetting MFA, changing a phone number, or sending a recovery link.

**The company should define recovery rules:**

- Verify identity before password resets.
- Verify identity before MFA resets.
- Use a known contact method, not the one provided during the request.
- Require manager approval for high-risk resets.
- Do not reset executive, finance, HR, IT, or admin accounts based only on email or chat.
- Record all emergency resets.
- Review all MFA resets for high-risk accounts.

Help desk and MSP staff must follow the same rules.

## Step 14: Protect High-Risk Roles

Some roles need stronger controls.

**High-risk roles include:**

- Executives
- Finance staff
- HR staff
- IT administrators
- MSP administrators
- Help desk staff
- Payroll users
- Accounting users
- Sales operations
- Customer data owners
- Developers
- Anyone with access to large data exports
- Anyone who can approve payments

**For these users, apply stronger protections:**

- MFA or passkeys.
- Hardware security keys where practical.
- Password manager required.
- No shared accounts.
- Reduced admin rights.
- Access reviewed more often.
- Extra verification for payment and account changes.
- Clear reporting path for suspicious requests.

## Step 15: Document Exceptions

Some systems may not support MFA, SSO, strong password rules, or proper role-based access.

Do not ignore those systems, record them.

**For each exception, document:**

|Exception Field|Record|
|---|---|
|System|Name of system|
|Missing control|MFA, SSO, logging, role control, or other|
|Reason|Why the control is missing|
|Risk|What could go wrong|
|Compensating control|Password manager, limited access, IP restriction, extra review, or other|
|Owner|Person responsible|
|Expiration date|When the exception must be reviewed|

Permanent exceptions are usually a sign of a bad system, weak vendor, or unfinished work.

## Step 16: Keep Evidence

The company should keep proof that IAM controls are working.

**Useful evidence includes:**

- MFA reports
- User lists
- Admin account lists
- Access review records
- Offboarding records
- Password manager user reports
- Vendor access records
- Service account register
- Screenshots of security settings
- SSO configuration records
- Conditional access settings
- Emergency access records
- Exception approvals

Keep this evidence in a controlled folder. It will help with audits, insurance, customer reviews, incident response, and management reporting.

## IAM Register Template

|Field|What to Record|
|---|---|
|System|Name of application, platform, device, or service|
|Business Owner|Person responsible for business use|
|Technical Owner|IT, MSP, or system admin|
|User Groups|Teams or roles with access|
|Admin Users|Named administrators|
|Vendor Users|External users with access|
|MFA Status|Enabled, partial, unavailable, or unknown|
|SSO Status|Enabled, unavailable, or not configured|
|Shared Accounts|Yes or no|
|Service Accounts|Yes or no|
|Access Review Frequency|Monthly, quarterly, annually|
|Last Review Date|Date last checked|
|Main Issue|Current weakness|
|Next Action|Required fix|

## Recommended Tools

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Microsoft Entra ID|[Microsoft Entra ID](https://www.microsoft.com/security/business/microsoft-entra)|Low-cost or included with Microsoft plans|Central identity, MFA, SSO, conditional access, admin controls|
|Microsoft Entra MFA|[Microsoft Entra MFA](https://learn.microsoft.com/en-us/entra/identity/authentication/concept-mfa-howitworks)|Included or paid depending on plan|MFA for Microsoft environments|
|Google Workspace 2-Step Verification|[Google Workspace 2-Step Verification](https://knowledge.workspace.google.com/admin/security/deploy-2-step-verification)|Included with Google Workspace|MFA for Google Workspace users|
|Google Admin Console|[Google Admin Console](https://admin.google.com/)|Included with Google Workspace|User management, admin roles, access review, security settings|
|Bitwarden|[Bitwarden](https://bitwarden.com/)|Open-source, low-cost|Business password manager, secure sharing, vaults, admin controls|
|Bitwarden Open Source|[Bitwarden Open Source](https://bitwarden.com/open-source/)|Open-source|Password manager with source transparency|
|KeePassXC|[KeePassXC](https://keepassxc.org/)|Open-source|Offline password vault for very small teams or special admin vaults|
|Psono|[Psono](https://psono.com/)|Open-source, self-hosted|Business password manager with self-hosting options|
|Passbolt|[Passbolt](https://www.passbolt.com/)|Open-source, low-cost|Team password management and secure credential sharing|
|Keycloak|[Keycloak](https://www.keycloak.org/)|Open-source|SSO and IAM for self-hosted applications|
|authentik|[authentik](https://goauthentik.io/)|Open-source, self-hosted|Identity provider, SSO, application access control|
|Authelia|[Authelia](https://www.authelia.com/)|Open-source|MFA and SSO portal for self-hosted applications through reverse proxies|
|FreeIPA|[FreeIPA](https://www.freeipa.org/)|Open-source|Central identity, policy, and access control for Linux/Unix environments|
|Windows LAPS|[Windows LAPS](https://learn.microsoft.com/en-us/windows-server/identity/laps/laps-overview)|Included in Windows environments|Local administrator password management|
|OpenBao|[OpenBao](https://openbao.org/)|Open-source|Secrets management for technical teams|
|Infisical|[Infisical](https://infisical.com/)|Open-source, low-cost|Secrets management for developers, apps, and infrastructure|
|Yubico Security Keys|[Yubico](https://www.yubico.com/)|Low-cost hardware security keys|Strong phishing-resistant MFA for admins and high-risk users|
|SoloKeys|[SoloKeys](https://solokeys.com/)|Open-source hardware security key project|Hardware security keys for passkeys and MFA|
|Excel|[Microsoft Excel](https://www.microsoft.com/microsoft-365/excel)|Low-cost|IAM register, access review tracker, exception tracker|
|Google Sheets|[Google Sheets](https://www.google.com/sheets/about/)|Low-cost|Shared access review and IAM tracking|

## Practical Tool Stack for SMEs

### Very small company:

- Google Workspace or Microsoft 365 identity
- Built-in MFA
- Bitwarden or KeePassXC
- Google Sheets or Excel access review tracker

### Small company with Microsoft 365:

- Microsoft Entra ID
- Microsoft Entra MFA
- Bitwarden or Passbolt
- Windows LAPS
- Excel or SharePoint register

### Small company with Google Workspace:

- Google Admin Console
- Google 2-Step Verification
- Bitwarden or Psono
- Google Sheets register

### Self-hosted or technical company:

- Keycloak or authentik
- Authelia for protected internal apps
- FreeIPA for Linux/Unix access
- Bitwarden, Psono, or Passbolt
- OpenBao or Infisical for secrets

## Expected Outputs from This IAM Stage

**At the end of this section, the company should have:**

- An IAM owner
- Clear access rules
- A main identity provider or identity source
- MFA enabled on critical systems
- An approved password manager
- Separate admin accounts
- A list of shared accounts and removal plans
- A service account register
- A vendor access register
- A joiner, mover, leaver process
- A recurring access review process
- Documented account recovery rules
- Stronger controls for high-risk roles
- An exception register

Evidence showing that IAM controls are actually working.


## Objectives

- Do not make access control informal.

- Every account should have a purpose.

- Every admin should be named.

- Every vendor should have an owner.

- Every exception should expire.

- Every leaver should be removed quickly.

- Every critical system should use MFA.

- If the company cannot explain who has access and why, access is not under control.

---

