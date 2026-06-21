---
icon: shield-check
order: -10
---

Use this checklist to confirm that the company has implemented practical safeguards to reduce the likelihood and impact of cybersecurity incidents.

The goal of Protect is to make the company harder to compromise, harder to abuse, and easier to keep operating when something goes wrong.

## Protect Overview Checklist

☐ Assign an owner to coordinate the Protect section.

☐ Confirm which systems, data, users, devices, vendors, and business processes need protection first.

☐ Use the Assess and Identify outputs to prioritize the most important controls.

☐ Create one central place to store protection standards, checklists, evidence, exceptions, and review notes.

☐ Confirm which controls are handled internally, by IT, by an MSP, or by vendors.

☐ Record exceptions where a control cannot be applied immediately.

☐ Set a review schedule for all major protection controls.

## Identity and Access Management Checklist

☐ Assign an owner for identity and access management.

☐ Define clear rules for access approval, changes, and removal.

☐ Centralize identity where possible through Microsoft 365, Google Workspace, SSO, or another identity provider.

☐ Require MFA for email, VPN, admin accounts, accounting, payroll, CRM, cloud storage, password managers, backup systems, and critical SaaS platforms.

☐ Deploy an approved password manager.

☐ Remove passwords from spreadsheets, browsers, email, chat messages, and personal vaults.

☐ Apply least privilege to employees, executives, vendors, contractors, administrators, and service accounts.

☐ Separate admin accounts from normal daily-use accounts.

☐ Remove or restrict shared accounts.

☐ Create a register of service accounts, API accounts, automation accounts, and integration accounts.

☐ Protect vendor and contractor access with named accounts, MFA, limited access, and review dates.

☐ Create a joiner, mover, leaver process for account creation, role changes, and offboarding.

☐ Review access to critical systems regularly.

☐ Secure password resets, MFA resets, and account recovery processes.

☐ Apply stronger access controls to executives, finance, HR, IT administrators, payroll users, and other high-risk roles.

☐ Keep evidence of MFA status, access reviews, admin accounts, offboarding, and vendor access.

## Backup Regimes and Recovery Readiness Checklist

☐ Assign a backup owner.

☐ Identify which systems, data, SaaS platforms, servers, websites, databases, and configurations must be backed up.

☐ Mark backup priority for critical, high, medium, and low importance systems.

☐ Define backup frequency, retention period, recovery point expectations, and recovery time expectations.

☐ Use a 3-2-1-1-0 backup approach where practical.

☐ Keep at least one offsite backup copy for critical data.

☐ Keep at least one offline or immutable backup copy for critical data where practical.

☐ Encrypt backups where supported.

☐ Protect backup consoles and storage with MFA and restricted admin access.

☐ Use separate backup credentials instead of normal daily admin accounts.

☐ Confirm SaaS backup or recovery options for Microsoft 365, Google Workspace, CRM, accounting, HR, payroll, file storage, and other key platforms.

☐ Back up important configurations, including firewall, router, VPN, website, DNS, cloud, and server settings.

☐ Monitor backup jobs for success, failure, missed jobs, storage capacity, and unusual deletion activity.

☐ Test restores on a scheduled basis.

☐ Document restore test results.

☐ Create a backup runbook.

☐ Keep backup evidence, reports, configuration records, restore test records, and exception approvals.

## Systems Hardening Checklist

☐ Choose hardening baselines, such as CIS Benchmarks, Microsoft Security Baselines, Google Workspace checklists, or vendor guidance.

☐ Create a systems hardening register.

☐ Harden new systems before they go into use.

☐ Remove default accounts, default passwords, unused accounts, and old setup accounts.

☐ Restrict administrator rights on endpoints, servers, SaaS platforms, cloud platforms, websites, and network devices.

☐ Enable device encryption where supported.

☐ Harden Windows, macOS, Linux, and server systems using approved baseline settings.

☐ Harden Microsoft 365 or Google Workspace admin settings.

☐ Harden SaaS platforms, cloud accounts, databases, websites, and CMS platforms.

☐ Harden firewalls, routers, switches, VPN systems, Wi-Fi equipment, printers, cameras, and IoT devices.

☐ Restrict browser extensions, browser password storage, risky downloads, and unsafe browser settings.

☐ Secure developer environments, repositories, API keys, SSH keys, CI/CD tools, and secrets.

☐ Enable useful logging and time synchronization on important systems.

☐ Create standard build checklists for laptops, servers, cloud systems, SaaS tools, websites, and network devices.

☐ Test hardening changes before broad rollout.

☐ Record hardening exceptions with owners, risks, compensating controls, and expiration dates.

☐ Keep evidence showing which systems were hardened and when.

## Vulnerability and Patch Management Checklist

☐ Assign vulnerability and patch management owners.

☐ Define the systems covered by the patch process.

☐ Create a vulnerability and patch register.

☐ Track trusted vulnerability sources, vendor advisories, known exploited vulnerabilities, and scanner findings.

☐ Run regular vulnerability scans where appropriate.

☐ Prioritize vulnerabilities based on exploitation, internet exposure, business criticality, sensitive data, severity, and available exploit code.

☐ Define remediation timelines for emergency, critical, high, medium, and low findings.

☐ Create a standard monthly patch cycle.

☐ Create an emergency patch process for exploited or high-risk vulnerabilities.

☐ Test patches before wide rollout where practical.

☐ Patch endpoints, servers, network devices, websites, cloud systems, containers, third-party applications, and developer dependencies.

☐ Track unsupported and end-of-life software, systems, firmware, plugins, and devices.

☐ Apply temporary mitigations where a patch cannot be applied immediately.

☐ Verify that patches or mitigations worked.

☐ Record exceptions with owners, compensating controls, approvals, and expiration dates.

☐ Report overdue critical vulnerabilities, known exploited vulnerabilities, internet-facing issues, and end-of-life systems to leadership.

## Endpoint, Server, and Mobile Device Protection Checklist

☐ Assign an owner for endpoint, server, and mobile device protection.

☐ Define which devices are allowed to access company systems.

☐ Create protection standards for laptops, desktops, servers, phones, tablets, shared devices, and remote devices.

☐ Enroll company-owned devices in a management or monitoring system where practical.

☐ Deploy centrally managed endpoint protection or EDR where appropriate.

☐ Protect servers separately from user devices.

☐ Enable full-disk encryption on required devices.

☐ Enforce screen lock and session lock rules.

☐ Restrict local administrator rights.

☐ Enable and manage local firewalls.

☐ Control software installation and remove unauthorized software.

☐ Control remote access tools, remote support tools, and RMM agents.

☐ Protect mobile devices with passcodes, encryption, OS updates, remote wipe, and managed apps where appropriate.

☐ Separate work data from personal data where possible.

☐ Restrict removable media where needed.

☐ Apply stronger controls to executive, finance, HR, IT, developer, and other high-risk devices.

☐ Protect endpoint management, EDR, MDM, RMM, and remote support consoles with MFA and limited admin access.

☐ Monitor device health, encryption, patch status, endpoint protection status, and last check-in.

☐ Create a lost or stolen device process.

☐ Create a device offboarding process.

☐ Document BYOD rules and exceptions.

## Email, Web, Cloud, and SaaS Protection Checklist

☐ Assign owners for email, websites, domains, DNS, cloud platforms, SaaS tools, and business-critical applications.

☐ Create a platform protection register.

☐ Configure SPF, DKIM, and DMARC for company email domains.

☐ Review DMARC reports and move toward enforcement where appropriate.

☐ Enable inbound email protection against spam, malware, phishing, spoofing, suspicious links, and dangerous attachments.

☐ Restrict external email forwarding and suspicious mailbox rules.

☐ Protect high-risk mailboxes, including executive, finance, HR, IT, shared, support, and sales mailboxes.

☐ Protect website and CMS platforms with updates, MFA, limited admin access, backups, HTTPS, secure forms, and WAF protection where appropriate.

☐ Protect domain registrar and DNS access with MFA, limited admins, domain lock, and controlled recovery settings.

☐ Restrict cloud file sharing, public links, guest access, and anonymous access.

☐ Review Microsoft 365 or Google Workspace security settings.

☐ Review SaaS admin users, MFA, SSO, guest access, external sharing, data exports, audit logs, and backup options.

☐ Review OAuth apps, SaaS integrations, API keys, webhooks, browser extensions, and marketplace apps.

☐ Protect cloud platforms with MFA, least privilege, logging, restricted public storage, secure secrets, and public exposure checks.

☐ Review website forms and customer data collection points.

☐ Store API keys, tokens, secrets, and service credentials securely.

☐ Use secure DNS or web filtering where appropriate.

☐ Review public sharing across cloud storage, SaaS pages, calendars, groups, repositories, dashboards, buckets, and public folders.

☐ Enable platform logging and keep evidence of key security settings.

## Network, Remote Access, and Internet Exposure Protection Checklist

☐ Assign owners for firewall, Wi-Fi, VPN, remote access, network devices, public IPs, domains, and internet exposure.

☐ Create a network and exposure register.

☐ Draw a simple network map.

☐ Review firewall rules and remove or restrict old, broad, temporary, or unnecessary rules.

☐ Remove direct internet exposure to admin interfaces.

☐ Protect VPN, ZTNA, remote desktop gateways, remote support tools, and vendor access paths.

☐ Remove or replace direct public RDP exposure.

☐ Require MFA for remote access.

☐ Remove shared remote access accounts.

☐ Review VPN users, former users, old vendor users, and split tunneling.

☐ Segment the network where practical.

☐ Separate guest Wi-Fi from business systems.

☐ Separate printers, cameras, IoT devices, backup systems, and admin systems where practical.

☐ Maintain firewalls, routers, switches, VPN appliances, Wi-Fi controllers, and ISP modems.

☐ Disable unsafe services such as Telnet, UPnP, and exposed management interfaces where possible.

☐ Use secure DNS or web filtering where appropriate.

☐ Review public IPs, domains, subdomains, SSL/TLS certificates, old websites, staging sites, APIs, and cloud exposure.

☐ Run authorized external exposure checks.

☐ Reduce unnecessary internet-facing services.

☐ Control vendor, MSP, RMM, and remote support access.

☐ Enable network logging and configuration backups.

☐ Create a change process for firewall rules, VPN changes, port forwards, DNS changes, and vendor access.

☐ Document network exceptions with owners, risks, compensating controls, approvals, and expiration dates.

## Final Protect Section Outputs

☐ Protect section owner assigned.

☐ Protection priorities confirmed from Assess and Identify outputs.

☐ Identity and access controls implemented.

☐ MFA enabled on critical systems.

☐ Password manager deployed.

☐ Access review process created.

☐ Backup scope, schedule, protection, monitoring, and restore testing defined.

☐ Systems hardening baselines selected.

☐ Key systems hardened.

☐ Vulnerability and patch management process created.

☐ Endpoint, server, and mobile device protections implemented.

☐ Email, web, cloud, and SaaS protections reviewed and improved.

☐ Network, remote access, and internet exposure protections reviewed and improved.

☐ Admin access restricted across critical systems.

☐ Vendor access controlled.

☐ Internet-facing exposure reduced.

☐ Exceptions documented.

☐ Evidence stored.

☐ Review schedule created.

☐ Priority unresolved issues carried forward into Detect, Respond, Recover, Review, or future improvement plans.