---
icon: triangle-right
order: 50
---


### Goal

External exposure detection helps the company notice when something becomes visible to the internet that should not be.

Control failure detection helps the company notice when an important security control stops working.

A company may have good protections in place, but those protections can fail quietly. A backup job stops. Endpoint protection stops reporting. MFA is disabled for one account. A public file link is created. A firewall rule exposes a service. A website plugin becomes vulnerable. A DNS record points to an old system. A cloud storage bucket becomes public. A remote access tool is left open.

This section defines how the company checks for those failures before they become incidents.

## Step 1: Define What Must Never Be Public

Start by listing systems and services that should not be reachable from the public internet.

This should include admin panels, databases, backup consoles, network device management pages, hypervisor consoles, NAS devices, RDP, SSH, internal dashboards, test sites, staging sites, printer interfaces, camera systems, and internal APIs.

Also list sensitive data locations that should not be publicly shared, such as HR folders, finance folders, customer records, contracts, payroll files, source code, credentials, backup files, and internal reports.

The company should be able to say clearly:

“These systems and files should never be public.”

## Step 2: Build an External Exposure Watchlist

Create a simple watchlist of internet-facing assets.

Include company domains, subdomains, public IP addresses, cloud public IPs, websites, portals, APIs, VPN portals, remote access portals, DNS records, SSL/TLS certificates, hosting accounts, cloud storage locations, and externally shared SaaS folders.

Common names to check include: vpn.company.com, remote.company.com, admin.company.com, dev.company.com etc.

Every public-facing item should have an owner, purpose, and review date.

Unknown exposure should be investigated.

## Step 3: Run Regular External Exposure Checks

The company should check what can be seen from outside the network.

Only scan systems the company owns or has written permission to test.

External checks should look for open ports, exposed services, public admin panels, exposed databases, old websites, staging sites, weak TLS settings, missing security headers, risky DNS records, weak email security records, public cloud storage, public repositories, and vulnerable internet-facing systems.

**Suggested review schedule:**

- Monthly for domains, public IPs, VPN portals, websites, DNS, and public cloud exposure.
- After every major firewall, hosting, cloud, DNS, website, or remote access change.
- Immediately after a security advisory affecting an internet-facing system the company uses.

If a service does not need to be public, remove it from public exposure.

## Step 4: Monitor Critical Control Failures

Some failures are not about exposure. They are about important controls stopping quietly.

**The company should monitor for:**

- Backup jobs failing
- Backup storage filling up
- Backup deletion or backup policy changes
- Endpoint protection disabled
- EDR or antivirus agent stopped
- Device stops checking in
- Firewall logging disabled
- VPN logging disabled
- MFA disabled
- Admin account added
- Audit logging disabled
- Security tool alerting disabled
- Patch deployment failures
- Public file sharing enabled
- Cloud bucket or storage made public
- Suspicious OAuth app approved
- Website monitoring failure
- Domain or DNS record changed
- SSL/TLS certificate near expiry

Control failures should be treated as warning signs, not routine noise.

## Step 5: Send Exposure and Failure Alerts Somewhere Monitored

Alerts must go to a monitored destination.

Good options include a security mailbox, IT ticket queue, MSP dashboard, SIEM, monitoring platform, or incident queue.

Do not send critical alerts only to one person’s inbox.

Critical alerts should include backup failures for critical systems, public exposure of sensitive data, public RDP or database exposure, endpoint protection failure across multiple devices, MFA disabled for privileged accounts, DNS or domain registrar changes, and backup deletion activity.

The alert destination should be tested.

## Step 6: Verify and Fix Findings

External exposure and control failure alerts need confirmation.

For each finding, confirm whether it is real, identify the owner, decide the required action, apply the fix, and record evidence.

**Possible actions include:**

- Remove the exposure.
- Restrict access to VPN, ZTNA, trusted IPs, or admin network.
- Disable the exposed service.
- Patch or update the exposed system.
- Remove public file sharing.
- Restore the failed control.
- Re-enable logging.
- Fix the backup job.
- Replace or isolate unsupported systems.
- Create a temporary exception only when needed.

Do not close a finding until the fix has been verified.

## Step 7: Keep an Exposure and Control Failure Register

Track findings in one place.

**Suggested fields:**

- Finding ID
- Date found
- System or service
- Domain, subdomain, IP, file, or platform
- Finding type
- Owner
- Severity
- Public exposure status
- Business impact
- Required action
- Due date
- Status
- Verification evidence
- Exception status
- Review date

This register keeps repeated problems visible. If the same type of failure keeps coming back, the process needs improvement.

## Common Exposure and Control Failure Blind Spots

Commonly missed areas include old subdomains, staging websites, public RDP, public SSH, exposed databases, old firewall rules, cloud storage buckets, SharePoint or Google Drive public links, DNS records, expired domains, domain registrar accounts, hosting panels, backup consoles, VPN portals, RMM tools, remote support agents, website plugins, test APIs, forgotten cloud servers, public code repositories, endpoint agents that stopped reporting, backup jobs that failed silently, and audit logs that were never enabled.

These are the places where quiet exposure often lives.

## Recommended Open Source and Affordable Tools

|Tool or Solution|Link|Type|Best Use|
|---|---|---|---|
|Nmap|[Nmap](https://nmap.org/)|Open-source|Open port and exposed service discovery|
|Greenbone Community Edition / OpenVAS|[Greenbone Community Edition](https://greenbone.github.io/docs/latest/)|Open-source|Vulnerability scanning for networks and internet-facing systems|
|Nuclei|[Nuclei](https://github.com/projectdiscovery/nuclei)|Open-source|Template-based exposure and vulnerability checks|
|Hardenize|[Hardenize](https://www.hardenize.com/)|Free and paid options|Domain, DNS, TLS, email, and internet exposure monitoring|
|Internet.nl|[Internet.nl](https://internet.nl/)|Free|Website, email, TLS, DNSSEC, and standards testing|
|Security Headers|[Security Headers](https://securityheaders.com/)|Free|Website security header checks|
|MDN HTTP Observatory|[MDN HTTP Observatory](https://developer.mozilla.org/en-US/observatory)|Free|HTTP header and web security checks|
|SSL Labs Server Test|[SSL Labs SSL Test](https://www.ssllabs.com/ssltest/)|Free|TLS and HTTPS configuration testing|
|Shodan|[Shodan](https://www.shodan.io/)|Free and paid options|Internet exposure discovery for public IPs and services|
|Censys|[Censys](https://censys.com/)|Free and paid options|Internet asset and exposure discovery|
|SecurityTrails|[SecurityTrails](https://securitytrails.com/)|Free and paid options|DNS history, subdomain discovery, and asset research|
|Prowler|[Prowler](https://prowler.com/)|Open-source and commercial|Cloud security posture and public exposure checks|
|ScoutSuite|[ScoutSuite](https://github.com/nccgroup/ScoutSuite)|Open-source|Multi-cloud security auditing|
|Steampipe|[Steampipe](https://steampipe.io/)|Open-source|Query cloud, SaaS, DNS, and infrastructure configuration|
|Checkov|[Checkov](https://www.checkov.io/)|Open-source and commercial|Infrastructure-as-code and cloud misconfiguration scanning|
|Trivy|[Trivy](https://trivy.dev/)|Open-source|Cloud, container, repository, IaC, and filesystem scanning|
|Gitleaks|[Gitleaks](https://github.com/gitleaks/gitleaks)|Open-source|Secret scanning in repositories and files|
|TruffleHog|[TruffleHog](https://github.com/trufflesecurity/trufflehog)|Open-source and commercial|Secret discovery and verification|
|Uptime Kuma|[Uptime Kuma](https://uptime.kuma.pet/)|Open-source|Website, service, and endpoint uptime monitoring|
|Healthchecks.io|[Healthchecks.io](https://healthchecks.io/)|Open-source and hosted plans|Monitoring backup jobs, cron jobs, scripts, and scheduled tasks|
|Zabbix|[Zabbix](https://www.zabbix.com/)|Open-source|Infrastructure, network, and service monitoring|
|LibreNMS|[LibreNMS](https://www.librenms.org/)|Open-source|Network device monitoring and alerting|
|Grafana|[Grafana](https://grafana.com/oss/grafana/)|Open-source|Dashboards and alert visibility|
|Prometheus|[Prometheus](https://prometheus.io/)|Open-source|Metrics monitoring and alerting|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|SIEM/XDR, control failure alerts, endpoint and cloud visibility|
|Security Onion|[Security Onion](https://securityonionsolutions.com/software/)|Open-source with paid support|Network security monitoring and log visibility|
|Suricata|[Suricata](https://suricata.io/)|Open-source|Network threat detection and IDS/IPS|
|Zeek|[Zeek](https://zeek.org/)|Open-source|Network security monitoring and protocol visibility|
|OpenCanary|[OpenCanary](https://opencanary.readthedocs.io/)|Open-source|Honeypot-style tripwire detection|
|Canarytokens|[Canarytokens](https://canarytokens.org/)|Free|Tripwire alerts for files, links, credentials, and systems|

## Practical Tool Stack for SMEs

#### Very small company:

Use Uptime Kuma, Healthchecks.io, Security Headers, SSL Labs, Internet.nl, Hardenize, Nmap, backup failure alerts, endpoint protection alerts, and a monitored security mailbox.

#### Microsoft-based SME:

Use Microsoft Defender, Microsoft Secure Score, Microsoft Purview Audit, Microsoft 365 alert policies, Healthchecks.io, Uptime Kuma, Hardenize, and external scans with Nmap or Greenbone.

#### Google Workspace SME:

Use Google Admin alerts, Google Workspace audit logs, Drive sharing reports, Healthchecks.io, Uptime Kuma, Hardenize, Internet.nl, and external checks with Nmap or Greenbone.

#### Website-heavy company:

Use Cloudflare alerts, WPScan, Nuclei, Security Headers, MDN HTTP Observatory, SSL Labs, Internet.nl, Uptime Kuma, and Hardenize.

#### Cloud-heavy company:

Use Prowler, ScoutSuite, Steampipe, Checkov, Trivy, cloud-native audit alerts, Censys, Shodan, and Gitleaks or TruffleHog for exposed secrets.

#### Network-heavy company:

Use Nmap, Greenbone, Security Onion, Suricata, Zeek, LibreNMS, Zabbix, Wazuh, firewall alerts, VPN alerts, and external exposure monitoring.

## Expected Outputs from This Section

At the end of this section, the company should have:

- A list of systems and data that should never be public.
- An external exposure watchlist.
- A schedule for external exposure checks.
- A list of critical controls that must be monitored for failure.
- Alerts sent to a monitored destination.
- A process for verifying and fixing findings.
- An exposure and control failure register.
- Evidence showing checks were performed and issues were closed.

## Objectives

Many incidents begin as something small that quietly changed.

A company should leave this section able to say:

“We know what should never be public. We check for accidental exposure. We monitor critical controls for failure. We verify findings and record the fix.”

That is external exposure and control failure detection.

----

