---
icon: triangle-right
order: 70
---
## Goals

Logs show what happened, while alerts show what may need attention.

Security visibility means the company can see important activity across its accounts, devices, systems, cloud platforms, SaaS tools, network, websites, and backup systems.

Without logs, the company may not know who logged in, what changed, what was deleted, what was downloaded, what failed, or how an attacker moved through the environment.

Without alerts, the company may only find out after damage is already done.

The goal is not to collect every possible log as that becomes expensive and noisy. The goal is to collect the logs that matter, alert on the events that matter, and make sure someone reviews them.

## Step 1: Assign Logging and Alert Ownership

Assign one owner for logging and alert visibility.

This may be the IT lead, MSP, security lead, outsourced SOC, or assigned technical owner.

The owner is responsible for making sure important logs are enabled, alerts go somewhere monitored, alert failures are investigated, and evidence is retained.

Also assign a backup owner. Alerts should not depend on one person being available.

## Step 2: Decide Which Systems Need Logs First

Start with the systems most likely to show compromise or business disruption.

**Priority systems include:**

- Email
- Microsoft 365 or Google Workspace
- Identity provider
- Admin accounts
- Password manager
- Endpoint protection or EDR
- Laptops and desktops
- Servers
- Firewalls
- VPN and remote access tools
- Backup systems
- Cloud storage
- Critical SaaS platforms
- Accounting and payroll systems
- CRM
- Website and CMS
- Domain registrar
- DNS provider
- Remote support and RMM tools
- Cloud platforms

Do not begin by logging everything. Begin by logging the systems that matter most.

## Step 3: Enable the Most Important Logs

Each important platform should have the right logs turned on.

**Focus first on logs that show:**

- User sign-ins
- Failed logins
- MFA failures and resets
- New users
- Deleted users
- New admin accounts
- Privilege changes
- Password resets
- Mailbox forwarding rules
- Suspicious inbox rules
- Email threats
- Malware detections
- Endpoint protection failures
- VPN logins
- Firewall rule changes
- Backup failures
- Backup deletion activity
- Public file sharing
- Large downloads
- SaaS admin changes
- OAuth app approvals
- API key activity
- Cloud storage exposure
- Website admin logins
- Domain and DNS changes

These are the records that help the company notice trouble and understand what happened.

## Step 4: Send Alerts to a Monitored Destination

Important alerts must go somewhere that is checked.

Good destinations include a monitored security mailbox, ticketing system, MSP dashboard, SIEM, logging platform, or incident queue.

Avoid sending alerts only to one person’s inbox. That person may be unavailable, on leave, or overloaded.

Critical alerts should also have an escalation path. For serious events, email alone may not be enough.

## Step 5: Define Alert Priority Levels

Not every alert is equal.

Use simple priority levels.

#### Critical alerts need immediate review

These include ransomware signs, confirmed malware, unauthorized admin access, backup deletion activity, public exposure of sensitive data, domain compromise, suspicious MFA reset, or confirmed account compromise.

#### High alerts should be reviewed the same business day 

These include suspicious sign-ins, repeated failed logins, new admin roles, unusual VPN access, endpoint protection disabled, mailbox forwarding created, or unusual data downloads.

#### Normal alerts should be reviewed on a defined schedule

These include routine policy warnings, non-critical configuration changes, low-severity detections, or informational platform notices.

If every alert is treated as urgent, the company will stop paying attention.

## Step 6: Create the Core Alert List

The company should begin with a small set of alerts that are worth reviewing.

**Core alerts should include:**

- Suspicious login or impossible travel
- Multiple failed login attempts
- MFA failures or MFA reset activity
- New administrator account
- Privilege escalation
- Former employee login
- Vendor login outside expected pattern
- Mailbox forwarding rule created
- Suspicious inbox rule created
- Malware or ransomware detection
- Endpoint protection disabled
- Device stops reporting
- Backup job failure
- Backup deletion or backup policy change
- VPN login from unusual location
- Firewall rule change
- Public file-sharing link created
- Large data download or export
- OAuth app approved
- API key created or changed
- Website admin login or file change
- Domain registrar or DNS change

Start here. Add more later after the first alerts are working.

## Step 7: Keep Logs Long Enough to Be Useful

Logs are only useful if they still exist when needed.

Set retention based on business need, risk, cost, and tool limits.

**As a practical starting point:**

- Keep critical security logs for at least 90 days where practical.
- Keep identity, email, admin, endpoint, VPN, firewall, backup, cloud, and SaaS logs long enough to investigate delayed discovery.
- Keep incident-related logs separately if an investigation begins.
- Know which platforms have short default retention.
- Know which logs require paid licensing or extra configuration.

The company should not discover during an incident that useful logs expired last week.

## Step 8: Protect the Logging System

The logging platform itself must be protected.

Limit admin access. Require MFA. Separate logging admin accounts from daily user accounts. Restrict who can delete logs. Back up important log configurations. Keep the logging system patched.

Where possible, send important logs to a place attackers cannot easily alter or delete.

If an attacker can erase the logs, the company may lose the timeline of the incident.

## Step 9: Test Alerts

Do not assume alerts work.

Test the important ones.

**Examples:**

- Create a test failed-login event.
- Confirm MFA reset alerts are received.
- Confirm malware test alerts are received safely using approved methods.
- Confirm backup failure alerts go to the right destination.
- Confirm VPN login alerts appear.
- Confirm firewall change alerts are recorded.
- Confirm website or CMS admin alerts work where available.
- Confirm domain or DNS change alerts are received.
- Document the test date, alert name, result, and next action.

An alert that nobody has tested is only a hope.

## Step 10: Review Alerts on a Schedule

Set a review schedule.

- **Critical alerts** should be reviewed immediately or as soon as reasonably possible.

- **High alerts** should be reviewed the same business day.

- **Normal alert** queues should be reviewed daily or weekly depending on the company’s size and risk.

Monthly review should check whether alerts are still useful, whether noise is too high, whether important systems are missing, and whether alert destinations still work.

Do not create alerts nobody reviews.

## Step 11: Create a Log and Alert Register

Keep a simple register.

**Suggested fields:**

- System name
- System owner
- Log type
- Alert type
- Alert destination
- Priority
- Review frequency
- Retention period
- Tool or platform
- Last tested date
- Known gap
- Next action

This register helps the company see what is covered and what is still blind.

## Step 12: Keep Evidence

Store proof that logging and alerting are working.

**Useful evidence includes:**

- Screenshots of log settings
- Alert configuration exports
- SIEM or log platform dashboards
- Alert test records
- Ticket examples
- MSP alert reports
- Email security reports
- Endpoint protection reports
- Backup alert reports
- Firewall log exports
- VPN login reports
- Cloud audit log settings
- SaaS audit log screenshots
- Retention settings
- Exception approvals

This evidence helps with audits, insurance, customer reviews, incident response, and internal review.

## Common Logging Blind Spots

**Common blind spots include:**

- Mailbox forwarding rules
- Suspicious inbox rules
- MFA reset events
- OAuth app approvals
- Shared mailbox access
- Guest access changes
- Former employee logins
- Vendor remote access
- Backup failures
- Backup deletion activity
- RMM tool activity
- Remote support sessions
- Domain registrar changes
- DNS record changes
- Website admin logins
- Cloud storage public sharing
- Large SaaS data exports
- Endpoint tools disabled
- Devices that stop checking in
- Firewall rule changes
- Public IP exposure changes

These are worth checking because they often show real risk early.

## Recommended Open Source and Affordable Tools

|Tool or Resource|Link|Type|Best Use|
|---|---|---|---|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|SIEM/XDR, endpoint visibility, log collection, vulnerability visibility, compliance support|
|Security Onion|[Security Onion](https://securityonionsolutions.com/software/)|Open-source with paid support|Network security monitoring, host visibility, IDS, log management, case management|
|Graylog Open|[Graylog Open](https://graylog.org/products/source-available/)|Source-available/free edition options|Centralized log management, search, dashboards, alerts|
|OpenSearch Security Analytics|[OpenSearch Security Analytics](https://docs.opensearch.org/latest/security-analytics/)|Open-source|SIEM-style security analytics, detection rules, alerts, investigation|
|Grafana Loki|[Grafana Loki](https://grafana.com/oss/loki/)|Open-source|Cost-conscious log aggregation and search|
|Grafana|[Grafana](https://grafana.com/oss/grafana/)|Open-source|Dashboards and visibility across logs, metrics, and alerts|
|Prometheus|[Prometheus](https://prometheus.io/)|Open-source|Metrics and infrastructure monitoring|
|Zabbix|[Zabbix](https://www.zabbix.com/)|Open-source|Infrastructure monitoring, alerting, server and network health|
|LibreNMS|[LibreNMS](https://www.librenms.org/)|Open-source|Network monitoring and device visibility|
|Uptime Kuma|[Uptime Kuma](https://uptime.kuma.pet/)|Open-source|Simple uptime monitoring for websites, services, and internal systems|
|Healthchecks.io|[Healthchecks.io](https://healthchecks.io/)|Open-source and hosted plans|Monitoring scheduled jobs, scripts, backups, and recurring tasks|
|Suricata|[Suricata](https://suricata.io/)|Open-source|Network IDS/IPS and network threat detection|
|Zeek|[Zeek](https://zeek.org/)|Open-source|Network security monitoring and protocol visibility|
|Sysmon|[Sysmon](https://learn.microsoft.com/sysinternals/downloads/sysmon)|Free|Detailed Windows and Linux system activity logging|
|osquery|[osquery](https://www.osquery.io/)|Open-source|Query endpoint state, processes, users, software, and security posture|
|Fleet|[Fleet](https://fleetdm.com/)|Open-source and commercial|osquery management, endpoint visibility, device posture|
|Fluent Bit|[Fluent Bit](https://fluentbit.io/)|Open-source|Lightweight log forwarding from systems, containers, and cloud environments|
|NXLog Community Edition|[NXLog Community Edition](https://nxlog.co/products/nxlog-community-edition)|Free/community edition|Log collection and forwarding, especially Windows event logs|
|Sigma|[Sigma](https://sigmahq.io/)|Open-source|Generic detection rule format for SIEM and log platforms|
|ElastAlert 2|[ElastAlert 2](https://github.com/jertel/elastalert2)|Open-source|Alerting from Elasticsearch/OpenSearch-style log data|
|Microsoft Sentinel|[Microsoft Sentinel](https://azure.microsoft.com/products/microsoft-sentinel)|Commercial, cloud-native|SIEM/SOAR for Microsoft and cloud-heavy environments|
|Microsoft Defender XDR|[Microsoft Defender XDR](https://www.microsoft.com/security/business/siem-and-xdr/microsoft-defender-xdr)|Commercial, often bundled|Microsoft identity, endpoint, email, cloud, and SaaS detection|
|Microsoft 365 Audit Logs|[Microsoft Purview Audit](https://learn.microsoft.com/purview/audit-solutions-overview)|Included or paid depending on plan|Microsoft 365 audit visibility|
|Google Workspace Audit Logs|[Google Workspace Audit Logs](https://support.google.com/a/answer/4579696)|Included depending on plan|Google Workspace login, admin, Drive, Gmail, and app activity visibility|
|Google Security Center|[Google Workspace Security Center](https://support.google.com/a/answer/7492330)|Included depending on edition|Google Workspace security dashboards, alerts, and investigation|
|Cloudflare Notifications|[Cloudflare Notifications](https://developers.cloudflare.com/notifications/)|Included depending on plan|Alerts for DNS, security, traffic, and account events|
|AWS CloudTrail|[AWS CloudTrail](https://aws.amazon.com/cloudtrail/)|Cloud-native, paid by usage|AWS API and account activity logging|
|Azure Monitor|[Azure Monitor](https://azure.microsoft.com/products/monitor)|Cloud-native, paid by usage|Azure logs, metrics, alerts, and dashboards|
|Google Cloud Logging|[Google Cloud Logging](https://cloud.google.com/logging)|Cloud-native, paid by usage|Google Cloud logs, metrics, alerts, and audit visibility|

## Practical Tool Stack for SMEs

#### Very small company:

Use Microsoft 365 or Google Workspace built-in audit logs, endpoint protection alerts, backup failure emails, firewall/VPN alerts, Uptime Kuma, Healthchecks.io, and a monitored security mailbox.

#### Microsoft-based SME:

Use Microsoft Defender XDR, Microsoft Purview Audit, Microsoft Sentinel where budget allows, Microsoft Secure Score, Defender for Endpoint or Defender for Business, and a ticket queue for alerts.

#### Google Workspace SME:

Use Google Workspace audit logs, Google Security Center where available, endpoint protection alerts, backup alerts, DNS or web filtering alerts, and a simple alert register.

#### Cost-conscious technical company:

Use Wazuh, Graylog Open or OpenSearch, Sysmon, osquery, Fluent Bit, Suricata, Zeek, Uptime Kuma, and Healthchecks.io.

#### Network-heavy company:

Use Security Onion, Suricata, Zeek, Zabbix, LibreNMS, firewall logs, VPN logs, DNS logs, and external exposure checks.

#### Cloud-heavy company:

Use AWS CloudTrail, Azure Monitor, Google Cloud Logging, OpenSearch, Wazuh, Grafana, Prowler outputs, cloud-native alerts, and security posture reports.

## Log and Alert Register Template

The company should maintain a simple register with these fields:

- System name
- Business owner
- Technical owner
- Log source
- Alert source
- Alert destination
- Alert priority
- Review frequency
- Retention period
- Last tested date
- Known gap
- Next action

## Expected Outputs from These Steps

At the end of this section, the company should have:

- A logging and alert owner.
- A list of priority systems that need logs.
- Key logs enabled for identity, email, endpoint, server, network, cloud, SaaS, backup, website, domain, and DNS activity.
- Important alerts sent to a monitored destination.
- Alert priority levels defined.
- A core alert list.
- Log retention expectations.
- Protected logging infrastructure.
- Tested alert paths.
- A review schedule.
- A log and alert register.
- Evidence showing logs and alerts are working.

## Practical Rule

Do not collect logs nobody reviews.

Do not create alerts nobody owns.

A company should leave this section able to say:

“We know which logs matter, where they go, who reviews alerts, how long logs are kept, and whether the alert path actually works.”

That is logging, alerts, and security visibility.

---

