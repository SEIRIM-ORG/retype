---
icon: triangle-right
order: 100
---


## Purpose of This Page

This page is for a company that knows its cybersecurity preparation is not good enough and needs to make meaningful progress quickly.

While we recommend a methodical approach proceeding through all 8 stages of our playbook process, your company might be under some pressure or concern that some threat is very near on the horizon and require a more expedited short-term plan of action. 

It is not intended to complete the entire playbook in one day or one week. The goal is to reduce the most serious and common risks first, establish basic ownership, and create enough visibility and resilience to continue improving in a controlled way.

If the company is already experiencing an active cyber incident, use the [[Unprepared Incident Response]] page first.

**The priorities on this page focus on four immediate outcomes:**

- Protect the accounts attackers are most likely to target.

- Make sure critical data and systems can be recovered.

- Reduce obvious exposure and unsupported access.

- Make sure employees and leadership know what to do if something suspicious happens.

## 1. If You Only Have 24 Hours

The first 24 hours should focus on controls that can materially reduce risk immediately.

Do not attempt a full cybersecurity transformation. Concentrate on the highest-value actions.

## Priority 1: Assign One Cybersecurity Owner

Name one person responsible for coordinating the 24-hour effort.

This may be the IT lead, operations manager, MSP contact, security owner, or another senior employee.

**Also identify:**

- Leadership decision-maker
- IT or MSP contact
- Backup contact
- Cyber insurance contact, if applicable

The immediate goal is to make sure somebody owns the work.

## Priority 2: Protect the Most Important Accounts With MFA

Confirm MFA is enabled on the accounts that could cause the most damage if compromised.

**Prioritize:**

- Email
- Microsoft 365 or Google Workspace administration
- Cloud administrator accounts
- Finance and payment systems
- Payroll
- Remote access and VPN
- Backup systems
- Domain registrar and DNS
- Password manager
- Security tools
- Privileged administrator accounts
- Vendor or MSP administrator access

Do not assume MFA is enabled because the company purchased a service that supports it. Verify it.

Unexpected MFA prompts should be denied and reported immediately.

## Priority 3: Secure Administrator Access

Identify who currently has administrator or privileged access.

**Immediately review:**

- Global administrators
- Domain administrators
- Cloud administrators
- SaaS administrators
- Backup administrators
- Finance administrators
- Vendor or MSP admin accounts

Remove obviously unnecessary admin access.

**Where possible:**

- Separate admin accounts from normal user accounts
- Require MFA
- Disable unused administrator accounts
- Remove former employee accounts
- Avoid shared administrator credentials

## Priority 4: Confirm Backups Actually Exist

Do not rely on assumptions.

**Identify the company's most important data and systems and confirm:**

- Backups are running
- Recent backups exist
- Backup failures are not being ignored
- At least one backup is protected from normal user or administrator compromise where practical
- The company knows who owns recovery

If practical within the time available, test restoration of one important file or small data set.


## Priority 5: Check the Most Obvious Internet Exposure

Identify the company’s main public-facing systems, including websites, VPNs, remote access services, firewalls, cloud servers, and administrative portals.

Use free services such as [Shodan](https://www.shodan.io/), [Censys](https://search.censys.io/), [Security Headers](https://securityheaders.com/), or [SSL Labs](https://www.ssllabs.com/ssltest/) to check what is publicly visible and identify obvious configuration problems.

A technical administrator or MSP can also use [Nmap](https://nmap.org/) to check company-owned public IP addresses for exposed services. Can use 

**Pay particular attention to:**

- RDP, SSH, or remote administration exposed directly to the internet
- Old VPNs, firewalls, servers, or network appliances
- Unexpected websites, subdomains, IP addresses, or services
- Administrative interfaces that should not be public
- Unsupported or unpatched internet-facing systems

Review public websites and portals for obvious security problems.

**Useful free checks include:**

- [Security Headers](https://securityheaders.com/) for web security headers
- [Qualys SSL Labs](https://www.ssllabs.com/ssltest/) for TLS and certificate configuration
- [Internet.nl](https://internet.nl/) for website, email, DNSSEC, TLS, and related internet standards
- [Hardenize](https://www.hardenize.com/) for broader domain, email, and TLS configuration review

Close, restrict, patch, or investigate anything that is unnecessary or unexpected.

If the company does not have the technical capability to perform these checks safely, ask its MSP or IT provider like us at [SEIRIM](https://seirim.com/en/home) for an **external internet exposure review**.

## Priority 6: Patch Critical Internet-Facing Systems

Confirm that important internet-facing systems are supported and patched.

**Prioritize:**

- Firewalls
- VPN appliances
- Remote access systems
- Web servers
- CMS platforms and plugins
- Email infrastructure
- Network appliances
- Cloud workloads

Do not attempt to patch everything in the company in one day.

Start with the systems attackers can reach from outside.

## Priority 7: Check Former Employee and Vendor Access

Review recently departed employees, contractors, and vendors.

**Confirm that unnecessary access has been removed from:**

- Email
- VPN
- Cloud services
- File storage
- Finance systems
- CRM
- HR systems
- Admin consoles
- Vendor portals
- Remote support systems

Old access that nobody remembers is one of the easiest risks to remove quickly.

## Priority 8: Create a Simple Incident Reporting Path

**Every employee should know where to report:**

- Suspicious emails
- Unexpected MFA prompts
- Fake login pages
- Lost devices
- Payment fraud attempts
- Data sent to the wrong person
- Strange device behavior
- Possible malware
- Create one simple reporting route such as:
- A security email address
- A helpdesk category
- A phishing report button
- A designated IT/MSP contact

**Tell employees:**

“If something suspicious happens, report it immediately. If you made a mistake, report it immediately.”

## Priority 9: Warn Finance and Leadership About Fraud

Send a short immediate reminder to finance, executives, HR, procurement, and anyone who can approve payments or account changes.

**Require independent verification for:**

- Bank-detail changes
- Payment destination changes
- Urgent executive requests
- Payroll changes
- Vendor account changes
- Password or MFA reset requests

Do not rely only on email confirmation for high-risk changes.

## Priority 10: Create a One-Page Emergency Contact Sheet

**Record:**

- Cybersecurity owner
- Leadership decision-maker
- IT/MSP
- Cloud provider support
- Email provider support
- Backup provider
- Cyber insurance
- Legal counsel
- Bank or payment provider
- Domain/hosting provider
- Key vendors

Store the contact sheet somewhere that remains available if normal company systems become unavailable.

## 24-Hour Outputs

**By the end of the first 24 hours, the company should have:**

- A cybersecurity owner
- Critical accounts protected with MFA
- Privileged accounts reviewed
- Former employee and unnecessary vendor access removed
- Backups confirmed
- At least basic recovery confidence
- Critical internet exposure reviewed
- High-priority external systems checked for patching
- An employee reporting path
- Payment and fraud verification instructions
- An emergency contact list
- A list of unresolved high-risk issues for the next seven days

## What Good Looks Like After 24 Hours

The company should be able to say:

“We know who is responsible, our most important accounts are better protected, unnecessary access has been reduced, backups have been checked, obvious external exposure has been reviewed, employees know how to report problems, and we know what high-risk work must happen next.”

---

## 2. If You Have 7 Days

The seven-day plan builds on the first 24 hours.

The goal is to move from emergency risk reduction to a basic but functioning cybersecurity foundation.

Complete the 24-hour actions first, then continue with the following work.

## Day 1: Complete the 24-Hour Priorities

Finish the immediate actions above.

**Do not move on while major gaps remain in:**

- MFA
- Admin access
- Backups
- Critical internet exposure
- Former employee access
- Incident reporting
- Emergency contacts

Record unresolved issues and assign owners.

## Day 2: Build a Basic Asset, Account, and Vendor Inventory

**Identify the company's most important:**

- Laptops and desktops
- Servers
- Network devices
- Cloud systems
- Applications
- SaaS platforms
- Websites and domains
- Email systems
- Admin accounts
- Shared accounts
- Service accounts
- Vendors
- MSPs
- Backup providers

Critical systems do not need perfect documentation yet.

The objective is to know what exists and who owns it.

**Mark anything that is:**

- Critical
- Sensitive
- Internet-facing
- Unsupported
- Unknown
- Vendor-managed

## Day 3: Review Identity and Access

Perform a focused access review.

**Check:**

- Who has administrator access?

- Who can access finance systems?

- Who can access sensitive customer or employee data?

- Which shared accounts exist?

- Which service accounts exist?

- Which vendors have access?

- Which former staff still appear in systems?

- Which accounts do not have MFA?

Remove unnecessary access and record exceptions.

Apply least privilege wherever practical.

## Day 4: Strengthen Endpoints, Email, and Remote Access

**Confirm that company devices have:**

- Endpoint protection
- Automatic security updates
- Screen locking
- Disk encryption where appropriate
- Controlled administrator rights
- Supported operating systems

Then review email and remote access.

**Check:**

- Spam and phishing protection
- Mailbox forwarding rules
- Legacy authentication
- Remote access tools
- VPN configuration
- Public RDP or SSH
- Unauthorized remote support software

Focus on reducing the easiest ways attackers can enter or persist.

## Day 5: Improve Backups, Logging, and Detection

Perform a deeper backup review.

**Confirm:**

- What is backed up
- How frequently
- Where backups are stored
- Who can delete them
- How long they are retained
- When restoration was last tested
- Who receives backup failure alerts

**Then define minimum monitoring for:**

- Critical account sign-ins
- Admin changes
- Endpoint security alerts
- Email security alerts
- Backup failures
- Remote access activity
- Public-facing systems

Alerts must go somewhere somebody actually reviews.

## Day 6: Create a Basic Incident Response and Recovery Plan

**Define:**

- Who leads an incident
- Who can disable accounts
- Who can isolate devices
- Who contacts leadership
- Who contacts the MSP
- Who contacts insurance or legal counsel
- Who can communicate externally
- Which systems must be recovered first

**Create a basic response checklist covering:**

- Triage
- Evidence preservation
- Containment
- Communication
- Escalation
- Eradication
- Recovery

Also create a recovery priority list for the most important business systems.

The plan does not need to be perfect.

It needs to be usable.

## Day 7: Train Employees and Review Remaining Risk

Provide a short cybersecurity briefing to all employees.

**Cover:**

- Phishing
- Fake login pages
- Unexpected MFA prompts
- Payment fraud
- Password safety
- Safe file sharing
- Lost devices
- Reporting mistakes immediately

**Give additional guidance to high-risk teams such as:**

- Finance
- HR
- Executives
- IT
- Procurement
- Managers

Then conduct a leadership review.

**Review:**

- What was completed
- What remains missing
- Highest current risks
- Unsupported systems
- Backup gaps
- Access gaps
- Monitoring gaps
- Vendor risks
- Actions requiring budget
- Actions requiring external support

Create a 30- to 90-day improvement plan from the remaining gaps.

## 7-Day Outputs

**By the end of seven days, the company should have:**

A cybersecurity owner and leadership contact
A basic asset inventory
A basic applications and services inventory
A users and privileged access list
A vendor and dependency list
MFA on high-risk accounts
Reduced unnecessary administrator access
Former employee and unnecessary vendor access removed
Basic endpoint protection confirmed
Critical systems patched or remediation assigned
Internet exposure reviewed
Backup coverage documented
At least one restore test completed where practical
Critical logging and alerts identified
Incident reporting path established
Basic incident response plan
Emergency contact list
Recovery priority list
Employee security briefing completed
High-risk teams given additional guidance
A prioritized list of remaining cybersecurity improvements

## What Good Looks Like After 7 Days

The company should not expect to be fully secure after seven days.

It should, however, be able to say:

“We know our most important systems, accounts, vendors, and risks. Our critical accounts use MFA, administrator access has been reviewed, backups have been checked, obvious exposure has been reduced, employees know how to report problems, and we have a basic plan for responding and recovering.”

## What Comes Next

After the seven-day rush period, move into the full cybersecurity playbook.

**Use:**

- Assess to understand and prioritize risk.
- Identify to complete inventories and ownership.
- Protect to strengthen controls.
- Detect to improve visibility.
- Respond to build incident readiness.
- Recover to improve resilience.
- Review to turn findings into corrective actions.
- Educate to strengthen employee behavior and decision-making.

Use the companion workbook to assign owners, due dates, evidence, and verification for all remaining work.

## Practical Rule

Do not try to fix everything first.

Fix the controls that reduce the greatest amount of risk in the shortest amount of time.

**In 24 hours:**

Protect accounts, access, backups, exposure, and reporting.

**In seven days:**

Build enough visibility, protection, detection, response, and recovery capability to begin managing cybersecurity properly.



