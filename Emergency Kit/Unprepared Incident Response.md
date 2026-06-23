---
icon: triangle-right
order: 30
---
### Emergency Kit: 10-Step Cyber Incident Response Plan for an Underprepared Company

#### Purpose of This Emergency Kit

This plan is for a company that has not yet done enough cybersecurity preparation but is now facing a serious incident.

This may include ransomware, business email compromise, stolen passwords, payment fraud, data exposure, malware infection, website compromise, cloud account compromise, vendor account compromise, or suspicious activity that could affect business operations.

The goal is to stabilize the situation, reduce damage, preserve evidence, communicate clearly, recover safely, and begin fixing the weaknesses that allowed the incident to happen.

This is not a substitute for qualified incident response, legal, insurance, or forensic support. If the incident is serious, the company should escalate quickly.

## Step 1: Do Not Panic and Assign an Incident Lead

Immediately assign one person to coordinate the response.

This person should control the incident record, decisions, communication, evidence tracking, and next actions.

Also assign a backup lead in case the first person becomes unavailable.

The incident lead does not need to solve every technical issue personally. Their job is to keep the response coordinated.

**Immediate actions:**

1. Name the incident lead.
2. Name a backup lead.
3. Create one central incident record.
4. Start a timeline.
5. Record who is involved.
6. Stop employees from taking random uncoordinated actions.

**Practical rule:**

One person coordinates. Many people may help, but no one should improvise alone.

## Step 2: Identify What Kind of Incident This Is

Quickly classify the situation.

**Common emergency categories include:**

- Ransomware or mass file encryption
- Business email compromise
- Stolen password or account takeover
- Payment fraud or bank-detail change fraud
- Lost or stolen device
- Data exposure or accidental public sharing
- Malware infection
- Website compromise
- Cloud or SaaS compromise
- Vendor or third-party account compromise
- Suspicious admin activity
- Unknown incident with unclear scope

Do not wait for perfect certainty. Use the best available facts and update the classification as more information appears.

**Immediate actions:**

- Record what was first noticed.
- Record who noticed it.
- Record which systems, accounts, data, or business processes may be affected.
- Record whether the incident appears active.
- Record whether business operations are currently disrupted.

**Practical rule:**

Classify quickly, then update as facts improve.

## Step 3: Preserve Evidence Before Changing Too Much

Before wiping systems, deleting emails, resetting everything, or rebuilding devices, preserve the most important evidence.

**Useful evidence includes:**

- Screenshots
- Suspicious emails and email headers
- Alert messages
- Log exports
- Affected usernames
- Device names
- IP addresses
- File names
- Ransom notes
- Payment fraud messages
- Chat messages
- Timeline notes
- Vendor messages
- Actions already taken

Do not rely on memory. Write things down.

**Immediate actions:**

- Create an evidence folder in a controlled location.
- Export or screenshot important records.
- Record timestamps.
- Record who collected each item.
- Restrict access to sensitive evidence.
- Do not delete suspicious emails, logs, accounts, or files until evidence needs are considered.

**Practical rule:**

Preserve first, then clean.

## Step 4: Contain the Damage

Containment means stopping the incident from spreading or continuing.

The right containment action depends on the incident type.

**Possible containment actions include:**

- Disconnect affected devices from the network.
- Disable compromised accounts.
- Revoke active sessions.
- Reset passwords only after sessions are controlled.
- Block malicious email senders, domains, links, or IP addresses.
- Remove malicious mailbox rules or forwarding.
- Suspend suspicious vendor access.
- Close exposed remote access.
- Stop public file sharing.
- Pause suspicious payments.
- Freeze risky business processes.
- Protect backups from deletion or encryption.

Be careful with shutdowns. In some cases, powering off a system can destroy volatile evidence or make investigation harder. If unsure, isolate from the network first and consult technical support.

**Immediate actions:**

- Contain the most obviously affected account, device, system, or process.
- Verify that containment worked.
- Record every containment action.
- Record business impact caused by containment.

**Practical rule:**

Stop the bleeding, but do not destroy the evidence.

## Step 5: Escalate to the Right Outside Support

An underprepared company should not try to handle a serious incident alone.

Escalate quickly to the right parties.

**Possible contacts include:**

- MSP or IT provider
- Cyber insurance carrier
- Incident response provider
- Legal counsel
- Cloud or SaaS provider support
- Email provider support
- Backup provider support
- Bank or payment processor
- Domain registrar or hosting provider
- Law enforcement or national cyber reporting body where appropriate

Do not contact attackers, negotiate ransom, or make payment decisions without leadership, legal, insurance, and incident response guidance.

**Immediate actions:**

- Check cyber insurance contact instructions.
- Contact the MSP or IT provider.
- Contact legal counsel if data, customers, employees, contracts, or regulation may be involved.
- Contact the bank immediately if payment fraud is involved.
- Contact qualified incident response support if ransomware, data theft, privileged account compromise, or broad compromise is suspected.

**Practical rule:**

Get expert help early, not after evidence is lost and systems are rebuilt incorrectly.

## Step 6: Communicate Through Safe Channels

If email, chat, identity systems, or devices may be compromised, do not use them blindly for incident coordination.

Use a safer communication channel if needed.

**Options may include:**

- Phone calls
- A clean external conference bridge
- A temporary secure chat space
- Personal phone numbers for key leadership
- A clean device not connected to the compromised environment
- A separate emergency email account approved by leadership and legal

Communication should be controlled. Employees should receive clear instructions. Customers, vendors, insurers, regulators, and external parties should only receive approved messages.

**Immediate actions:**

- Create a small incident response group.
- Tell employees what to do and what not to do.
- Avoid broad speculation.
- Avoid statements such as “no data was affected” unless verified.
- Record important communications and decisions.

**Practical rule:**

Communicate clearly, but only from facts.

## Step 7: Find the Scope

Scope means understanding what is affected and what may still be at risk.

**Start with the most critical questions:**

- Which accounts are compromised?
- Which devices are affected?
- Which servers or SaaS systems are affected?
- Which data may have been accessed or exposed?
- Which vendors or customers may be involved?
- Which business processes are disrupted?
- Are backups affected?
- Is attacker access still active?
- Has the incident spread?

Scope should be expanded from the obvious affected system to similar systems, related accounts, shared credentials, admin accounts, vendor access, remote access, cloud services, and backups.

**Immediate actions:**

- List affected accounts, systems, data, and vendors.
- Check admin accounts first.
- Check email forwarding and mailbox rules.
- Check recent sign-ins.
- Check remote access logs.
- Check backup status.
- Check similar systems for the same signs.
- Record unknowns separately.

**Practical rule:**

Do not assume the first visible problem is the whole incident.

## Step 8: Eradicate the Cause Before Full Recovery

Eradication means removing attacker access, malware, persistence, exploited weaknesses, and unsafe configurations.

Do not rush straight to recovery if the attacker can still access the environment.

**Possible eradication actions include:**

- Remove malware.
- Rebuild affected devices.
- Patch exploited systems.
- Disable unsafe remote access.
- Rotate compromised passwords.
- Rotate exposed API keys, tokens, and secrets.
- Remove malicious mailbox rules.
- Remove unauthorized OAuth apps.
- Close exposed services.
- Remove suspicious admin accounts.
- Fix misconfigurations.
- Review vendor access.

Eradication should be verified before the company reconnects systems or restores normal access.

**Immediate actions:**

- Identify the weakness that allowed the incident.
- Remove attacker access.
- Fix the exposed weakness.
- Rebuild high-risk systems where needed.
- Rotate credentials after containment.
- Confirm the same issue is not present elsewhere.

**Practical rule:**

Do not restore normal operations while the door is still open.

## Step 9: Recover Carefully and Validate Before Normal Use

Recovery should restore business operations safely.

Start with critical business processes, not random systems.

**Recovery priorities may include:**

- Identity and access
- Email
- Finance and payments
- Customer service
- Core operational systems
- File storage
- Payroll
- Websites and customer portals
- Backups
- Monitoring and security tools

Before returning systems to normal use, validate that they are clean, patched, monitored, backed up, and approved by the business owner.

**Immediate actions:**

- Restore from trusted sources.
- Use known-good backups.
- Restore in priority order.
- Restore access in stages.
- Validate data integrity.
- Confirm security controls are active.
- Confirm monitoring is working.
- Confirm backups resume.
- Get business owner approval.
- Record recovery decisions.

**Practical rule:**

Recovery is not complete until systems, data, access, monitoring, and business processes are validated.

## Step 10: Close the Emergency With a Short Review and Improvement Plan

After the immediate emergency is controlled, do not simply move on.

Create a short review.

**Document:**

- What happened
- When it started
- How it was detected
- What was affected
- What actions were taken
- What business impact occurred
- What evidence was preserved
- What caused the incident
- What controls failed
- What worked well
- What slowed the response
- What still needs investigation
- What must change immediately
- Assign owners and due dates for urgent fixes.

**High-priority improvements often include:**

- MFA enforcement
- Admin account cleanup
- Password manager rollout
- Backup testing
- Logging and alerting
- Endpoint protection
- Patch management
- Remote access hardening
- Email security
- Vendor access review
- Payment verification process
- Employee reporting instructions
- Incident response plan creation

**Practical rule:**

The emergency is not finished until the company has assigned corrective actions.

## Emergency Tool Recommendations

The tools below can help, but they should be used carefully. In a serious incident, avoid installing tools directly onto compromised systems unless a qualified technical responder approves the approach.

|Work Area|Free, Open-Source, or Affordable Tools|Best Use|
|---|---|---|
|Incident tracking|[TheHive](https://strangebee.com/thehive/), [Zammad](https://zammad.org/), [osTicket](https://osticket.com/), [GLPI](https://glpi-project.org/), [Jira Service Management](https://www.atlassian.com/software/jira/service-management)|Incident record, triage, action tracking, communication tracking|
|Secure documentation|[CryptPad](https://cryptpad.org/), [Nextcloud](https://nextcloud.com/), [BookStack](https://www.bookstackapp.com/), [Wiki.js](https://js.wiki/)|Evidence notes, timelines, decision records, emergency procedures|
|Endpoint investigation|[Velociraptor](https://docs.velociraptor.app/), [osquery](https://www.osquery.io/), [Fleet](https://fleetdm.com/), [Sysmon](https://learn.microsoft.com/sysinternals/downloads/sysmon)|Endpoint visibility, process history, suspicious activity review, artifact collection|
|Log review and detection|[Wazuh](https://wazuh.com/), [Security Onion](https://securityonionsolutions.com/software/), [Graylog Open](https://graylog.org/products/source-available/), [OpenSearch](https://opensearch.org/)|Logs, alerts, event correlation, endpoint and network visibility|
|Forensics and timeline support|[Autopsy](https://www.autopsy.com/), [Volatility](https://volatilityfoundation.org/), [Timesketch](https://timesketch.org/), [Plaso](https://plaso.readthedocs.io/), [Hayabusa](https://github.com/Yamato-Security/hayabusa), [Chainsaw](https://github.com/WithSecureLabs/chainsaw)|Disk review, memory analysis, timeline reconstruction, Windows event log review|
|Malware and indicator review|[CyberChef](https://gchq.github.io/CyberChef/), [VirusTotal](https://www.virustotal.com/), [urlscan.io](https://urlscan.io/), [MISP](https://www.misp-project.org/)|Decode artifacts, check suspicious files/links/domains, organize indicators|
|Network containment|[OPNsense](https://opnsense.org/), [pfSense CE](https://www.pfsense.org/), [CrowdSec](https://www.crowdsec.net/), [Fail2ban](https://github.com/fail2ban/fail2ban)|Firewall rules, traffic blocking, exposed service reduction, brute-force protection|
|Remote access emergency controls|[Cloudflare Zero Trust](https://www.cloudflare.com/zero-trust/), [Tailscale](https://tailscale.com/), [NetBird](https://netbird.io/)|Safer emergency remote access, access restriction, VPN replacement or tightening|
|Backup and recovery|[restic](https://restic.net/), [BorgBackup](https://www.borgbackup.org/), [Kopia](https://kopia.io/), [Proxmox Backup Server](https://www.proxmox.com/en/proxmox-backup-server), [Veeam Community Edition](https://www.veeam.com/products/free/backup-recovery.html)|Backup creation, backup validation, restore testing, recovery support|
|Status and alerting|[Uptime Kuma](https://uptime.kuma.pet/), [Healthchecks.io](https://healthchecks.io/), [ntfy](https://ntfy.sh/), [Gotify](https://gotify.net/)|Service monitoring, backup-job alerts, incident notifications|
|Cloud and configuration checks|[Prowler](https://prowler.com/), [ScoutSuite](https://github.com/nccgroup/ScoutSuite), [Steampipe](https://steampipe.io/), [Trivy](https://trivy.dev/), [Gitleaks](https://gitleaks.io/)|Cloud posture checks, configuration review, exposed secrets, container and code scanning|

## Minimum Emergency Records to Create

**Even if the company has no formal incident response system, create these records immediately:**

- Incident timeline
- Affected systems list
- Affected accounts list
- Evidence folder
- Containment action log
- Communication log
- Decision log
- External support contact list
- Recovery priority list
- Improvement action list

These records can start in a spreadsheet or shared document. The important point is that they exist and are controlled.

## Emergency First-Hour Checklist

**In the first hour, focus on:**

- Assign incident lead.
- Start incident record and timeline.
- Preserve evidence.
- Contain the obvious affected account, device, system, or process.
- Protect backups.
- Contact IT/MSP and cyber insurance if applicable.
- Contact bank immediately if payment fraud is involved.
- Use safe communication channels.
- Tell employees what to do and what not to do.
- Record every major action.

## Practical Emergency Objective

In a serious incident, the company should prioritize five things:

- Coordinate.
- Preserve evidence.
- Contain damage.
- Escalate to qualified help.
- Recover safely.

If the company does those five things, it has a much better chance of reducing damage even if it was underprepared.

---

