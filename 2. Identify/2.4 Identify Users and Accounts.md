---
icon: triangle-right
---
### Goals


Identify every human and non-human identity that can access company systems, data, devices, cloud resources, applications, or services; record who owns each account, what it can access, whether it is still needed, and whether it is managed through a proper lifecycle.

### Task

- Identify users, administrators, contractors, service accounts, shared accounts, vendor accounts, API keys, and automation identities. 
- The aim is to understand every access point into the environment, especially privileged or unmanaged access.


## Main steps in the Identify Users and Accounts process

### 1. Define what counts as a user or account

Do not limit this to employees. That is the first failure point.

Include employees, executives, contractors, temporary workers, interns, vendors, MSP accounts, administrators, shared accounts, break-glass accounts, test accounts, service accounts, API accounts, OAuth applications, SSH keys, cloud IAM users, cloud roles, database users, local device accounts, bot accounts, automation accounts, mailbox accounts, and disabled or dormant accounts.

Answer the key question: **Who or what can authenticate into company systems, applications, devices, or data stores?**

### 2. Create a standard identity/account inventory record

Before collecting anything, define the fields. Otherwise you end up with exports that cannot be compared.

**Minimum fields should include:**

- Account name  
- Account type  
- Human or non-human  
- Person assigned, if applicable  
- Business owner  
- Technical owner  
- Department  
- System/application  
- Identity source  
- Email/username/login ID  
- Role/group membership  
- Privilege level  
- Authentication method  
- MFA status  
- Last login date  
- Creation date  
- Status: active, disabled, dormant, shared, orphaned, service, vendor, emergency, pending review  
- Data/systems accessible  
- Manager or approver  
- Review frequency  
- Last reviewed date  
- Offboarding status

**For non-human accounts, also include:**

- Service purpose  
- Application owner  
- Secret/key location  
- Credential rotation date  
- Token/API key expiry  
- Systems using it  
- Whether it is interactive or non-interactive

**In this age of AI, also include a section for:**

- AI agents
- Apps and services incorporating AI agents
- Employees and contractors deploying AI agents


Answer the key question: **Can we explain what this account is, who owns it, what it accesses, and why it exists?**

### 3. Identify authoritative identity sources

Find the systems that create or control identities. These are the places where account inventory should start.

**Typical sources:**

- HR system  
- Payroll system  
- Microsoft Entra ID  
- Active Directory  
- Google Workspace  
- LDAP directory  
- Identity provider or SSO platform  
- MDM/endpoint platform  
- Cloud IAM consoles  
- Password manager  
- VPN/firewall accounts  
- Database platforms  
- SaaS admin portals  
- Local administrator accounts  
- Developer platforms such as GitHub, GitLab, Bitbucket  
- CI/CD systems  
- Secrets managers

Useful links:

[Microsoft Entra user management](https://learn.microsoft.com/en-us/entra/identity/users/)  
[Google Workspace Admin Directory API](https://developers.google.com/workspace/admin/directory/v1/guides/manage-users)

Answer the key question: **Where are identities created, stored, authenticated, and assigned access?**

### 4. Export all human user accounts

Pull account lists from the main identity systems first.

**Export from:**

- Microsoft Entra ID / Active Directory  
- Google Workspace  
- HR/payroll  
- VPN  
- MDM  
- Email platform  
- Core SaaS tools  
- Financial systems  
- CRM/ERP  
- Helpdesk  
- Password manager  
- Cloud IAM  
- Developer tools

Capture employees, contractors, vendors, and admins separately. Do not merge them too early; you need to see account type and employment relationship.

Answer the key question: **Which human users exist across every major system, and are they linked to a real person?**

### 5. Identify privileged and administrator accounts

Privileged accounts deserve separate handling because they can change systems, access sensitive data, disable controls, create users, or approve access.

**Look for:**

- Global admins  
- Domain admins  
- Local admins  
- Cloud admins  
- Database admins  
- SaaS admins  
- Finance admins  
- HR admins  
- Security admins  
- Helpdesk admins  
- Root accounts  
- Break-glass accounts  
- Privileged vendor accounts

Answer the key question: **Which accounts can materially change systems, access sensitive data, or bypass normal controls?**

### 6. Identify non-human accounts

This is where many SMEs are blind. Non-human identities often outlive the people who created them.

**Include:**

- Service accounts  
- API keys  
- OAuth applications  
- Cloud IAM roles  
- Automation accounts  
- CI/CD tokens  
- Database service users  
- Backup service accounts  
- Monitoring accounts  
- Webhook credentials  
- SSH keys  
- Certificates  
- Bot accounts  
- Shared mailbox accounts  
- Application registrations  
- Secrets in scripts or environment files

**Useful links:**

[Google Cloud service accounts overview](https://cloud.google.com/iam/docs/service-account-overview)  
[Microsoft Entra application and service principal objects](https://learn.microsoft.com/en-us/entra/identity-platform/app-objects-and-service-principals)

Answer the key question: **What non-human identities exist, what systems use them, and who owns them?**

### 7. Identify shared accounts and generic accounts

Shared accounts are operationally convenient but problematic from a security accountability perspective as they dramatically increase risk by increasing the likelihood the account credentials will be leaked, if there is a leak it can be untraceable, and the impact of attacks is worsened.

**Examples:**

- admin  
- reception  
- sales  
- warehouse  
- finance  
- support  
- scanner  
- backup  
- contractor  
- temp  
- root  
- localadmin  
- service

**For each one, record:**

- Who uses it  
- Why it exists  
- Where credentials are stored  
- Whether access is logged  
- Who approves use  
- Whether it can be replaced by named accounts

Where possible, prohibit shared accounts from being used and require every user and service to have their own accounts.

Answer the key question: **Which accounts are not tied to one accountable person or service owner?**

### 8. Map users and accounts to systems, roles, and data

An account list alone is weak, it must show access relationships.

**Map each account to:**

- Applications  
- Groups  
- Roles  
- Devices  
- Cloud accounts/projects/subscriptions  
- Databases  
- Shared drives  
- Mailboxes  
- Privileged functions  
- Sensitive data categories  
- Business process supported

Answer the key question: **What can this account actually access or control?**

This is the difference between an identity inventory and a useless username dump.

### 9. Reconcile accounts against HR and vendor records

Compare user accounts against the authoritative people list.

**Flag:**

- Former employees with active accounts  
- Contractors past end date  
- Vendor accounts with no sponsor  
- Duplicate accounts  
- Users with no department  
- Users with no manager  
- Users with no owner  
- Disabled users still assigned licenses  
- Active accounts with no recent login  
- Admin accounts with no documented approval

Answer the key question: **Does every human account map to an active person, sponsor, or approved business need?**

### 10. Review authentication and MFA status

For each account or account category, identify authentication posture.

**Capture:**

- Password-only  
- MFA enabled  
- MFA required  
- SSO enabled  
- Local login  
- Federated login  
- Passwordless  
- Hardware key  
- Break-glass exception  
- Legacy authentication  
- API key/token  
- Certificate-based authentication  
- SSH key

Here we are recording the critical info that is the precursor for designing the protection controls that will increase and improve security.

Answer the key question: **How does this account authenticate, and is that method known?**

### 11. Identify dormant, orphaned, stale, and risky accounts

Flag accounts that need later action.

**Examples:**

- No login in 30/60/90 days  
- No owner  
- No manager  
- No MFA  
- Admin account with no approval  
- Service account with no technical owner  
- API key with no expiry  
- Cloud access key not rotated  
- Vendor account still active after project end  
- Shared account used by multiple people  
- Former employee account still enabled  
- Local admin account reused across endpoints

Answer the key question: **Which accounts are active but not clearly justified, owned, or controlled?**

### 12. Validate with business and technical owners

Send the account inventory to department heads, application owners, IT, HR, finance, and vendor managers.

**Ask:**

- Is this person still active?  
- Does this person still need access?  
- Who owns this service account?  
- Who approves this admin access?  
- Is this vendor account still needed?  
- Can this shared account be removed or replaced?  
- Are these roles correct?  
- Is anything missing?

Answer the key question: **Can the people accountable for the system confirm that the account list is accurate?**

### 13. Maintain the account inventory through lifecycle triggers

Identity inventories go stale quickly unless tied to business events.

**Update when:**

- Employee joins  
- Employee changes role  
- Employee leaves  
- Contractor starts or ends  
- Vendor is onboarded  
- Vendor project ends  
- New SaaS app is approved  
- New service account is created  
- API key/token is issued  
- Admin role is granted  
- Cloud account/project/subscription is created  
- Break-glass account is used  
- Application is retired  
- System owner changes

**Recommend Process**

- Monthly review of privileged accounts  
- Monthly review of new, dormant, and disabled accounts  
- Quarterly review of all user access for critical systems  
- Quarterly review of service accounts and API keys  
- Immediate review after terminations, vendor offboarding, or admin role changes

Answer the key question: **How do we prevent accounts from accumulating forever?**

## Recommended open-source or lower-cost tools

|Tool|Best use|Why it fits|Watch-out|
|---|---|---|---|
|[Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/identity/users/)|Microsoft-based user, group, role, application, and service-principal inventory|Often already present in Microsoft 365 environments; useful for users, groups, licenses, enterprise apps, app registrations, and service principals.|Not open source. It will not find accounts outside Microsoft unless integrated.|
|[Google Workspace Admin / Directory API](https://developers.google.com/workspace/admin/directory/v1/guides/manage-users)|Google Workspace user and group inventory|Useful for listing users, groups, suspended users, aliases, and Workspace identities.|Does not automatically find external SaaS accounts paid outside Google.|
|[Google OAuth log events](https://knowledge.workspace.google.com/admin/reports/oauth-log-events)|Identifying third-party apps connected to Google identities|Helps identify OAuth-connected applications and users.|Visibility depends on logging, edition, and retention.|
|[Keycloak](https://www.keycloak.org/)|Open-source identity and access management|Strong option for SSO and centralized identity for applications; supports authentication and securing apps/services.|Better for application IAM than discovering all existing accounts across legacy tools.|
|[authentik](https://goauthentik.io/)|Self-hosted open-source identity provider|Good for SSO, identity provider consolidation, and access policy enforcement.|Needs competent self-hosting and identity architecture.|
|[ZITADEL](https://zitadel.com/opensource)|Open-source IAM for modern applications|Good for developer-oriented identity infrastructure, SSO, OIDC, SAML, SCIM, passkeys, and multi-tenancy.|More useful for app identity than general SME account discovery.|
|[FreeIPA](https://www.freeipa.org/)|Linux/Unix identity management|Provides centralized authentication, authorization, account information, users, groups, hosts, and policy management for Linux/Unix environments.|Best for Linux-heavy environments. Not a universal Windows AD replacement.|
|[OpenLDAP](https://www.openldap.org/)|LDAP directory services|Open-source LDAP implementation for directory-based user and group management.|Powerful but low-level. More administration burden than modern identity providers.|
|[Samba AD DC](https://wiki.samba.org/index.php/Setting_up_Samba_as_an_Active_Directory_Domain_Controller)|Open-source Active Directory-compatible domain controller|Can provide AD-style domain authentication, especially for cost-sensitive environments.|Serious operational responsibility. Do not deploy casually.|
|[midPoint](https://evolveum.com/midpoint/)|Open-source identity governance and administration|Strong for identity governance, provisioning, account correlation, lifecycle, and access review workflows.|More complex than a simple directory export. Better for mature SMEs or regulated environments.|
|[GLPI](https://www.glpi-project.org/en/)|Central register for users, ownership, assets, and support records|Useful as a lightweight system of record tying users, assets, tickets, and responsibilities together.|Not a dedicated IAM/IGA tool. Use it for organization and workflow, not authentication.|
|[iTop](https://www.itophub.io/)|CMDB-style relationship mapping|Useful for linking users, teams, services, applications, and dependencies in a CMDB model.|Requires modeling discipline. Bad data model equals bad CMDB.|
|[ADRecon](https://github.com/adrecon/ADRecon)|Active Directory inventory and reporting|Generates reports to provide a holistic picture of an AD environment.|Good for discovery and assessment, not ongoing identity governance.|
|[BloodHound Community Edition](https://specterops.io/bloodhound-community-edition/)|Identity relationship and attack-path mapping|Maps identity relationships and privilege paths across environments; useful for understanding hidden privilege relationships.|Not a basic inventory tool. Use only with authorization and care.|
|[AzureHound CE](https://bloodhound.specterops.io/collect-data/ce-collection/azurehound)|Entra ID / Azure collection for BloodHound CE|Collects Entra ID and AzureRM data using Microsoft Graph and Azure REST APIs.|Security-analysis tool, not a general account register.|
|[PingCastle](https://www.pingcastle.com/)|Active Directory and Entra ID assessment|Helps assess AD and Entra ID exposure and misconfiguration posture.|Check licensing and usage terms for commercial use.|
|[Purple Knight](https://www.semperis.com/purple-knight/)|Free AD, Entra ID, and Okta exposure assessment|Free assessment tool for indicators of exposure and compromise in hybrid identity environments.|Assessment tool, not a live inventory platform.|
|[Wazuh system inventory](https://documentation.wazuh.com/current/user-manual/capabilities/system-inventory/index.html)|Endpoint-local users, groups, services, and software|Useful for identifying local users/groups on endpoints and servers, plus processes, services, ports, and software.|Do not use it as your only identity source. It sees endpoints, not all SaaS/cloud accounts.|
|[Fleet](https://fleetdm.com/) / [osquery](https://www.osquery.io/)|Endpoint querying for local users and system state|Good for querying local accounts, groups, processes, and device state across endpoints.|More technical than a standard admin console.|
|[CloudQuery](https://www.cloudquery.io/docs/platform/features/asset-inventory)|Cloud IAM and resource inventory|Useful for syncing cloud identity/resource metadata into a searchable data store.|Cloud-focused. Needs SQL/data handling capability.|
|[Steampipe](https://steampipe.io/)|Query cloud/SaaS identity data with SQL|Useful for querying IAM users, roles, groups, policies, service accounts, and cloud metadata through plugins.|Query layer, not a governance platform.|
|[Prowler](https://github.com/prowler-cloud/prowler)|Cloud IAM/security assessment|Open-source cloud security platform with IAM checks and multi-cloud assessment capability.|More security assessment than inventory. Good companion tool.|
|[Bitwarden Business](https://bitwarden.com/pricing/business/)|Shared credentials and password vault organization|Low-cost business password manager; Teams and Enterprise plans are positioned for organization-wide credential management.|Password manager is not identity governance. It helps organize credentials, not replace accounts.|
|[Passbolt](https://www.passbolt.com/)|Team credential sharing|Open-source password and credential manager for teams; supports self-hosted and cloud-hosted use.|Better for shared credentials and technical teams than broad user lifecycle management.|
|[HashiCorp Vault](https://developer.hashicorp.com/vault)|Secrets, tokens, certificates, keys|Stores and tightly controls access to tokens, passwords, certificates, encryption keys, and other secrets.|Licensing and product editions need review. Also operationally heavy if mismanaged.|
|[OpenBao](https://openbao.org/)|Open-source secrets management|Manages, stores, and distributes secrets, certificates, and keys under an open-governance model.|Younger ecosystem than Vault. Evaluate maturity for your use case.|
|[Infisical](https://infisical.com/)|Developer secrets, service credentials, certificates|Manages secrets, certificates, SSH keys, and privileged access for developers and infrastructure.|More developer/infrastructure-focused than general business password management.|
|[Authelia](https://www.authelia.com/)|Open-source SSO/MFA in front of web apps|Open-source authentication and authorization server providing SSO and MFA, usually with reverse proxies.|Good for protecting apps; not a full identity inventory or IGA platform.|
|[Pomerium](https://www.pomerium.com/)|Identity-aware access to internal apps|Provides clientless, identity-aware access to applications without a VPN.|Access proxy, not your source of identity truth.|

## Practical stack recommendations

#### For a small Microsoft 365 SME, use:

- **Microsoft Entra ID + Microsoft 365 admin exports + Bitwarden Business + GLPI/iTop + quarterly access review spreadsheet.**

This is realistic. Entra gives your main identity source. Bitwarden handles shared credentials. GLPI or iTop stores ownership and review records.

#### For a small Google Workspace SME, use:

- **Google Workspace Admin + Google OAuth logs + Bitwarden or Passbolt + GLPI/iTop + quarterly access review spreadsheet.**

This catches users, suspended users, groups, aliases, and many third-party connected apps.

#### For a Linux-heavy SME, use:

- **FreeIPA + Keycloak or authentik + Bitwarden/Passbolt + Wazuh/Fleet.**

FreeIPA handles Linux users/hosts. Keycloak/authentik gives SSO. Wazuh/Fleet helps find local endpoint accounts.

#### For a cloud-heavy SME, use:

- **Microsoft Entra or Google Workspace + CloudQuery + Steampipe + Prowler + Vault/OpenBao/Infisical.**

This is better for AWS/Azure/GCP IAM roles, service accounts, cloud access keys, and secrets.

#### For an AD-heavy company, use:

- **Active Directory/Entra exports + ADRecon + BloodHound CE/AzureHound + PingCastle or Purple Knight + GLPI/iTop.**

This gives identity inventory plus privilege-path visibility. BloodHound-style tools are powerful and should only be run with explicit authorization.

#### For a more mature or regulated SME, use:

**midPoint + Entra/Google/AD connectors + password manager + secrets manager + CMDB.**

midPoint is the most serious open-source option here for identity governance and administration, but it is not the right first move for a company that cannot already maintain a clean account inventory.

## Suggested account inventory fields

Use these fields in the playbook or spreadsheet:

- Account ID  
- Display name  
- Username/email/login  
- Account type  
- Human or non-human  
- Employment type: employee, contractor, vendor, service, automation, shared, emergency  
- Department  
- Manager  
- Business owner  
- Technical owner  
- System/application  
- Identity source  
- Group/role membership  
- Privilege level  
- Authentication method  
- MFA status  
- SSO/federated login status  
- Last login date  
- Created date  
- Password/key/token last rotated  
- Expiration date  
- Access review frequency  
- Data accessible  
- Systems accessible  
- Approved by  
- Status  
- Offboarding status  
- Last reviewed date  
- Notes

**For service accounts/API keys, add:**

- Service purpose  
- Application using it  
- Secret location  
- Rotation owner  
- Rotation frequency  
- Credential expiry  
- Interactive login allowed?  
- Break-glass use?  
- Systems dependent on it

## Steps Summary

**Identify Users and Accounts Process**

1. Define all human and non-human account types in scope.
    
2. Create a standard account inventory record.
    
3. Identify authoritative identity sources such as HR, Microsoft Entra, Active Directory, Google Workspace, LDAP, cloud IAM, SaaS admin portals, and password managers.
    
4. Export all human user accounts from core systems.
    
5. Identify privileged and administrator accounts.
    
6. Identify service accounts, API keys, OAuth apps, SSH keys, certificates, bots, automation accounts, and cloud roles.
    
7. Identify shared, generic, emergency, vendor, and dormant accounts.
    
8. Map accounts to systems, applications, groups, roles, data, devices, and business processes.
    
9. Reconcile accounts against HR, contractor, and vendor records.
    
10. Record authentication method, MFA status, SSO status, and last login activity.
    
11. Flag stale, orphaned, unmanaged, overprivileged, shared, expired, or ownerless accounts.
    
12. Validate account records with business owners, technical owners, HR, IT, and vendor sponsors.
    
13. Maintain the inventory through joiner, mover, leaver, vendor onboarding, vendor offboarding, admin-role change, service-account creation, and periodic review triggers.
    

## Summary

If the company cannot answer **who has access, what they can access, which accounts are privileged, which accounts are shared, which accounts belong to former users, and which service accounts have no owner**, then access management is mostly theater. The company does not have identity visibility; it has login sprawl.


----

