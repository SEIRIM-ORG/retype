---
icon: triangle-right
order: 90
---

## Goal

Detection only works when someone is responsible for watching the right systems and acting on important alerts.

Many SMEs already have alerts coming from email, Microsoft 365, Google Workspace, endpoint protection, firewalls, backups, websites, SaaS tools, or an MSP. The problem is often not that alerts do not exist. The problem is that nobody is clearly assigned to review them, confirm what matters, and escalate when needed.

This section defines who owns detection and which systems are included.

## Step 1: Assign a Detection Owner

Assign one person or provider to own detection.

This may be an internal IT lead, security lead, MSP, outsourced SOC, or assigned operations manager.

The detection owner is responsible for making sure alerts are received, reviewed, escalated, and recorded.

The company should also assign a backup owner in case the main person is unavailable.

**Record:**

- Detection owner
- Backup detection owner
- MSP or vendor contact, if applicable
- Executive escalation contact
- Normal review schedule
- Emergency escalation method

Do not leave detection ownership informal. “IT will see it” is not a process.

## Step 2: Decide Which Systems Must Be Covered

The company should define which systems need monitoring coverage.

Start with the systems that are most likely to show early signs of compromise or business disruption.

**Include:**

- Email platform
- Microsoft 365 or Google Workspace
- Identity provider
- Password manager
- Endpoint protection or EDR
- Laptops and desktops
- Servers
- Firewalls
- VPN or remote access tools
- Backup systems
- Cloud storage
- Critical SaaS platforms
- Accounting and payroll systems
- CRM
- Website and CMS
- Domain registrar
- DNS provider
- Remote support or RMM tools
- Cloud platforms

Not every system needs advanced monitoring on day one. But every critical system should have someone responsible for reviewing important warnings.

## Step 3: Define Where Alerts Go

Every important alert should have a destination.

**Alerts may go to:**

- A monitored security mailbox
- A ticketing system
- An MSP dashboard
- An internal IT queue
- A SIEM or logging platform
- A vendor portal
- A phone or SMS escalation path for critical issues

Avoid alerts going only to one person’s inbox. If that person is unavailable, the alert may be missed.

For critical alerts, use a destination that is checked daily or escalates immediately.

## Step 4: Define What the Detection Owner Must Review

The detection owner should not try to review everything with equal urgency.

Focus on the warning signs that matter most.

**At minimum, review alerts related to:**

- Suspicious sign-ins
- MFA failures or resets
- New admin accounts
- Privilege changes
- Mailbox forwarding rules
- Malware or ransomware detections
- Endpoint protection failures
- Backup failures
- VPN logins from unusual locations
- Public file sharing
- Large or unusual data downloads
- Cloud or SaaS admin changes
- Website security alerts
- Domain or DNS changes
- Remote support tool activity
- Former employee access
- Vendor access activity

These are the alerts most likely to show that something important has changed or may be under attack.

## Step 5: Define Review Timing

Set clear timing expectations.

Critical alerts should be reviewed immediately or as soon as reasonably possible.

- **High-priority** alerts should be reviewed the same business day.

- **Normal** alerts should be reviewed on a defined schedule.

- **Low-value** informational alerts can be reviewed during routine checks.

The company should not create alerts that nobody has time to review. Too many unmanaged alerts create noise, not security.

## Step 6: Define Escalation Rules

The detection owner should know when to escalate.

**Escalate immediately when there are signs of:**

- Ransomware
- Confirmed malware
- Compromised email account
- Unauthorized admin access
- Suspicious MFA reset
- Former employee login
- Vendor account abuse
- Sensitive data exposed publicly
- Backup deletion or backup failure affecting critical systems
- Suspicious financial request or invoice fraud
- Unusual access to accounting, payroll, HR, or customer data
- Domain, DNS, website, or cloud account compromise

These events should move from Detect into the Respond section.

## Step 7: Keep a Detection Coverage Register

Create a simple register showing which systems are covered.

**Suggested fields:**

- System name
- System owner
- Detection owner
- Alert source
- Alert destination
- Review frequency
- Critical alerts enabled
- Last alert test
- Known gaps
- Next action

This register helps leadership see which systems are being watched and which systems are still blind spots.

## Step 8: Review Coverage Regularly

Detection coverage should be reviewed at least quarterly.

**Also review it after:**

- New SaaS platform added
- New website launched
- New remote access tool deployed
- New MSP or vendor onboarded
- New cloud platform created
- Major system migration
- Security incident
- Change in backup, firewall, endpoint, or identity platform

The company should not assume new systems are automatically monitored.

## Expected Outputs from This Section

**At the end of this work, the company should have:**

- A named detection owner.
- A backup detection owner.
- A clear escalation contact.
- A list of systems included in detection coverage.
- A defined destination for important alerts.
- A basic list of alerts the detection owner must review.
- Review timing expectations.
- Escalation rules.
- A detection coverage register.
- A schedule for reviewing detection coverage.


## Objectives

Detection is not owned by software.

Detection is owned by people.

The company should leave this section able to say:

“We know which systems are being watched, who receives the alerts, how often they are reviewed, and when suspicious activity gets escalated.”

That is detection ownership and coverage.

----

