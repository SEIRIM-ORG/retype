---
icon: triangle-right
order: 60
---


### Goals

Most cyber incidents do not begin everywhere at once.

They usually begin through a few common paths: a stolen account, a phishing email, an infected endpoint, an exposed remote access service, a risky SaaS integration, a vulnerable website, or a cloud storage mistake.

This section defines how the company watches those main attack paths.

The goal is not to monitor everything equally. That creates noise. The goal is to watch the places where attackers are most likely to enter, move, steal, disable, or abuse access.

## Step 1: Define the Main Attack Paths to Watch

Start with the attack paths most relevant to the company.

**For most SMEs, these should include:**

- Identity and account compromise
- Email phishing, business email compromise, and invoice fraud
- Endpoint and server malware
- Cloud and SaaS misuse
- Remote access and VPN abuse
- Website, CMS, and public exposure
- Data sharing and large exports
- Backup failure or backup tampering
- Admin console misuse
- Vendor, MSP, and contractor access abuse

These are the paths that most often show early warning signs.

## Step 2: Monitor Identity and Account Activity

Identity is one of the first places to watch.

The company should monitor for suspicious sign-ins, repeated failed logins, impossible travel, unusual countries, new devices, MFA failures, MFA reset activity, password reset activity, new admin roles, inactive accounts becoming active, and former employee login attempts.

Pay extra attention to executives, finance, HR, IT administrators, payroll users, accounting users, domain registrar admins, DNS admins, cloud admins, backup admins, and vendor accounts.

Useful tools include Microsoft Entra ID logs, Microsoft Defender XDR, Google Workspace audit logs, Google Security Center, Wazuh, Graylog, OpenSearch, and SIEM rules based on Sigma.

The key question is:

“Would we notice if an account was being used in a way that does not match normal business activity?”

## Step 3: Monitor Email and Business Email Compromise Signals

Email is still one of the most important attack paths for SMEs.

The company should monitor for phishing detections, malware attachments, spoofed internal senders, executive impersonation, suspicious mailbox rules, hidden forwarding, unusual outbound sending, mass email activity, unusual login locations, new mail connectors, changed delegation permissions, and finance-related email anomalies.

Look closely at shared mailboxes, finance mailboxes, HR mailboxes, executive mailboxes, customer support mailboxes, and accounts that handle invoice or payment changes.

Useful tools include Microsoft Defender for Office 365, Google Workspace Gmail logs and alerts, Proxmox Mail Gateway, Rspamd, SpamAssassin, DMARC monitoring tools, Wazuh, and SIEM alert rules.

The key question is:

“Would we notice if a mailbox was compromised and being used to read, forward, hide, or send sensitive messages?”

## Step 4: Monitor Endpoints and Servers

Endpoints and servers should be monitored for signs of malware, ransomware behavior, disabled protection tools, suspicious scripts, unauthorized remote tools, unusual command-line activity, privilege escalation, abnormal file changes, new persistence mechanisms, and unknown software.

Watch especially for PowerShell abuse, script execution, credential dumping indicators, new scheduled tasks, new services, suspicious process chains, endpoint protection being disabled, and devices that stop checking in.

For servers, also monitor administrative logins, service account activity, new listening services, unexpected outbound connections, file integrity changes, and backup agent health.

Useful tools include Microsoft Defender for Business, Wazuh, Velociraptor, osquery, Fleet, Sysmon, Security Onion, Graylog, OpenSearch, YARA, Sigma, and commercial EDR tools where budget allows.

The key question is:

“Would we notice if a device became infected, started behaving strangely, or stopped reporting?”

## Step 5: Monitor Cloud, SaaS, and File Sharing

Cloud and SaaS platforms need active visibility.

Monitor public links, external sharing, guest users, large downloads, unusual exports, new integrations, OAuth app approvals, API key creation, suspicious admin changes, new billing admins, disabled audit logs, risky marketplace apps, and access from unusual locations.

Check Microsoft 365, Google Workspace, Dropbox, Box, CRM, accounting, payroll, HR, project management tools, support tools, marketing platforms, code repositories, and cloud storage.

Pay special attention to systems where users can export customer data, employee data, finance data, credentials, source code, contracts, or confidential files.

Useful tools include Microsoft Secure Score, Microsoft Purview Audit, Microsoft Defender XDR, Google Workspace audit logs, Google Security Center, Prowler, ScoutSuite, Steampipe, Trivy, Gitleaks, TruffleHog, Wazuh, and SaaS admin reports.

The key question is:

“Would we notice if sensitive files became public, data was exported, or a risky app was granted access?”

## Step 6: Monitor Remote Access, VPN, and Network Entry Points

Remote access is a high-value attack path.

Monitor VPN logins, unusual countries, repeated failed VPN attempts, vendor logins, after-hours remote access, new remote users, disabled MFA, public RDP, public SSH, firewall rule changes, new port forwards, remote support sessions, RMM activity, and devices connecting from unexpected locations.

Also monitor network devices for firmware status, admin logins, configuration changes, exposed management interfaces, and suspicious DNS or outbound traffic.

Useful tools include firewall logs, VPN logs, Cloudflare Zero Trust, Tailscale, NetBird, Wazuh, Security Onion, Suricata, Zeek, Zabbix, LibreNMS, Nmap, Greenbone, Nuclei, Shodan, Censys, and Hardenize.

The key question is:

“Would we notice if someone entered through remote access, exposed a service, or changed the network path?”

## Step 7: Monitor Websites, CMS Platforms, and Public Exposure

Public-facing systems need regular checks.

Monitor website admin logins, CMS updates, plugin changes, file changes, new admin users, failed login spikes, web application firewall alerts, suspicious uploads, defacement indicators, form abuse, exposed staging sites, TLS issues, security header gaps, public admin panels, and vulnerable plugins.

Include WordPress, Drupal, Joomla, Magento, Shopify apps, custom websites, hosting panels, databases, staging sites, test environments, APIs, and public storage.

Useful tools include WPScan, Wordfence, ModSecurity, OWASP Core Rule Set, Coraza, Cloudflare, CrowdSec, Fail2ban, Security Headers, Mozilla Observatory, SSL Labs, Internet.nl, Nuclei, Greenbone, and Wazuh.

The key question is:

“Would we notice if our website became vulnerable, changed unexpectedly, or exposed something public?”

## Step 8: Monitor Backups and Security Control Failures

Some incidents are detected because a protection control stops working.

Monitor backup failures, missed jobs, backup deletion, backup policy changes, backup storage capacity, endpoint protection disabled, EDR agent stopped, device stopped checking in, firewall logging disabled, audit logging disabled, MFA disabled, public sharing enabled, antivirus outdated, patch failures, and lost device status.

Backups deserve special attention. Ransomware attackers often try to damage recovery options before encrypting or extorting the company.

Useful tools include backup platform alerts, Healthchecks.io, Uptime Kuma, Wazuh, Zabbix, Grafana, Prometheus, Microsoft Defender, Google Admin alerts, MSP reports, and SIEM alerts.

The key question is:

“Would we notice if an important protection stopped working before we needed it?”

## Step 9: Create a Main Attack Path Monitoring Register

Keep a simple register so monitoring does not become informal.

**Suggested fields:**

- Attack path
- System or platform
- Owner
- Log source
- Alert source
- Alert destination
- Priority
- Review frequency
- Tool used
- Last tested date
- Known gap
- Next action

This register should show which attack paths are being watched and where the company still has blind spots.

## Step 10: Test and Review the Monitoring

Monitoring should be tested.

At least quarterly, confirm that important alerts still work and still go to the right destination.

Test safe examples such as failed logins, MFA reset alerts, backup failure notifications, endpoint protection health alerts, VPN login alerts, website uptime alerts, public exposure checks, and DNS change alerts.

Also review the alert quality. Remove noisy alerts that nobody uses. Add missing alerts for systems that matter. Fix alerts going to old inboxes, inactive users, or unmonitored dashboards.

Monitoring should improve over time.

## Recommended Open Source and Affordable Tools

|Tool or Solution|Link|Type|Best Use|
|---|---|---|---|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|SIEM/XDR, endpoint monitoring, vulnerability visibility, cloud and server security monitoring|
|Security Onion|[Security Onion](https://securityonionsolutions.com/software/)|Open-source with paid support|Network security monitoring, IDS, log management, threat hunting|
|Graylog Open|[Graylog Open](https://graylog.org/products/source-available/)|Free/source-available options|Central log management, dashboards, search, alerts|
|OpenSearch Security Analytics|[OpenSearch Security Analytics](https://docs.opensearch.org/latest/security-analytics/)|Open-source|SIEM-style detection, rules, alerting, and investigation|
|Sigma|[Sigma](https://sigmahq.io/sigma/)|Open-source|Detection rule format for SIEM and log platforms|
|Microsoft Defender for Business|[Microsoft Defender for Business](https://learn.microsoft.com/en-us/defender-business/mdb-overview)|Affordable commercial|Endpoint detection and protection for SMEs using Microsoft|
|Microsoft Defender XDR|[Microsoft Defender XDR](https://www.microsoft.com/security/business/siem-and-xdr/microsoft-defender-xdr)|Commercial|Microsoft identity, endpoint, email, and cloud detection|
|Microsoft Purview Audit|[Microsoft Purview Audit](https://learn.microsoft.com/purview/audit-solutions-overview)|Included or paid by plan|Microsoft 365 audit visibility|
|Google Workspace Audit Logs|[Google Workspace Audit Logs](https://support.google.com/a/answer/4579696)|Included depending on plan|Google Workspace login, admin, Drive, Gmail, and app activity logs|
|Google Workspace Security Center|[Google Workspace Security Center](https://support.google.com/a/answer/7492330)|Included depending on edition|Google Workspace alerts, dashboards, and investigation|
|Velociraptor|[Velociraptor](https://www.rapid7.com/products/velociraptor/)|Open-source|Endpoint visibility, forensic collection, investigation, threat hunting|
|osquery|[osquery](https://www.osquery.io/)|Open-source|Endpoint state visibility and security queries|
|Fleet|[Fleet](https://fleetdm.com/)|Open-source and commercial|osquery management, device posture, endpoint visibility|
|Sysmon|[Sysmon](https://learn.microsoft.com/sysinternals/downloads/sysmon)|Free|Detailed Windows and Linux system activity logging|
|Suricata|[Suricata](https://suricata.io/)|Open-source|Network IDS/IPS and network threat detection|
|Zeek|[Zeek](https://zeek.org/)|Open-source|Network security monitoring and protocol visibility|
|Nmap|[Nmap](https://nmap.org/)|Open-source|Open port and exposed service discovery|
|Greenbone Community Edition|[Greenbone Community Edition](https://greenbone.github.io/docs/latest/)|Open-source|Vulnerability scanning across networks and systems|
|Nuclei|[Nuclei](https://github.com/projectdiscovery/nuclei)|Open-source|Template-based exposure and vulnerability checks|
|Shodan|[Shodan](https://www.shodan.io/)|Free and paid options|Internet exposure discovery|
|Censys|[Censys](https://censys.com/)|Free and paid options|Internet asset and exposure discovery|
|Hardenize|[Hardenize](https://www.hardenize.com/)|Free and paid options|Domain, email, TLS, DNS, and exposure review|
|WPScan|[WPScan](https://wpscan.com/)|Free and paid options|WordPress vulnerability and plugin scanning|
|Security Headers|[Security Headers](https://securityheaders.com/)|Free|Website security header review|
|SSL Labs Server Test|[SSL Labs SSL Test](https://www.ssllabs.com/ssltest/)|Free|TLS and HTTPS configuration testing|
|Cloudflare Zero Trust|[Cloudflare Zero Trust](https://www.cloudflare.com/zero-trust/)|Free tier and commercial|Access control, secure web gateway, DNS filtering, remote access visibility|
|Cloudflare Notifications|[Cloudflare Notifications](https://developers.cloudflare.com/notifications/)|Included depending on plan|DNS, security, account, and traffic alerts|
|Uptime Kuma|[Uptime Kuma](https://uptime.kuma.pet/)|Open-source|Uptime monitoring for websites and internal services|
|Healthchecks.io|[Healthchecks.io](https://healthchecks.io/)|Open-source and hosted plans|Monitoring backups, scripts, scheduled jobs, and recurring tasks|
|Zabbix|[Zabbix](https://www.zabbix.com/)|Open-source|Infrastructure, server, and network monitoring|
|LibreNMS|[LibreNMS](https://www.librenms.org/)|Open-source|Network monitoring and device visibility|
|OpenCanary|[OpenCanary](https://opencanary.readthedocs.io/)|Open-source|Honeypot-style internal tripwire detection|
|Canarytokens|[Canarytokens](https://canarytokens.org/)|Free|Tripwire tokens for detecting access to files, links, credentials, and systems|
|Prowler|[Prowler](https://prowler.com/)|Open-source and commercial|Cloud security posture and exposure checks|
|ScoutSuite|[ScoutSuite](https://github.com/nccgroup/ScoutSuite)|Open-source|Multi-cloud security assessment|
|Steampipe|[Steampipe](https://steampipe.io/)|Open-source|Query cloud, SaaS, and infrastructure configuration|
|Trivy|[Trivy](https://trivy.dev/)|Open-source|Container, repository, filesystem, IaC, and cloud scanning|
|Gitleaks|[Gitleaks](https://github.com/gitleaks/gitleaks)|Open-source|Secret scanning in repositories, files, and pipelines|
|TruffleHog|[TruffleHog](https://github.com/trufflesecurity/trufflehog)|Open-source and commercial|Secret discovery and verification|

## Practical Tool Stack by Company Type

#### Very small company:

Use Microsoft 365 or Google Workspace built-in alerts, endpoint protection alerts, backup failure alerts, Uptime Kuma, Healthchecks.io, Cloudflare or NextDNS filtering, Security Headers, SSL Labs, and a monitored security mailbox.

#### Microsoft-based SME:

Use Microsoft Defender for Business, Microsoft Defender XDR where available, Microsoft Purview Audit, Microsoft Secure Score, Entra ID logs, mailbox rule alerts, backup alerts, and a ticket queue.

#### Google Workspace SME:

Use Google Workspace audit logs, Google Security Center where available, Gmail security alerts, Drive sharing alerts, endpoint protection alerts, backup alerts, and regular OAuth app reviews.

#### Cost-conscious technical company:

Use Wazuh, Graylog or OpenSearch, Sysmon, osquery, Fleet, Sigma rules, Uptime Kuma, Healthchecks.io, Nmap, and Greenbone.

#### Network-heavy company:

Use Security Onion, Suricata, Zeek, Zabbix, LibreNMS, firewall logs, VPN logs, DNS logs, and regular external exposure checks.

#### Website-heavy company:

Use Cloudflare, WPScan, Wordfence, Security Headers, SSL Labs, Mozilla Observatory, Nuclei, Uptime Kuma, and hosting/CMS admin alerts.

#### Cloud-heavy company:

Use Prowler, ScoutSuite, Steampipe, Trivy, cloud-native audit logs, cloud-native alerting, Gitleaks, TruffleHog, and SIEM forwarding where possible.

## Expected Outputs from These Steps

At the end of this section, the company should have:

- A defined list of main attack paths to monitor.
- Identity monitoring for suspicious sign-ins, MFA events, and admin changes.
- Email monitoring for phishing, forwarding rules, suspicious inbox rules, and business email compromise signs.
- Endpoint and server monitoring for malware, suspicious scripts, disabled security tools, and ransomware-like behavior.
- Cloud and SaaS monitoring for public sharing, data exports, OAuth apps, API keys, and admin changes.
- Remote access and network monitoring for VPN abuse, exposed services, firewall changes, and unusual access.
- Website and CMS monitoring for public exposure, plugin risk, admin activity, and file changes.
- Backup and control failure monitoring.
- A main attack path monitoring register.
- A quarterly test and review process.

## Practical Rule

Do not monitor everything equally.

Watch the attack paths that matter most.

A company should leave this section able to say:

“We know the main ways attackers may enter or abuse our environment, and we have alerts or reviews in place for those paths.”

That is monitoring the main attack paths.

----

