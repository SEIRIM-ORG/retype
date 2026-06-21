---
order: 40
icon: triangle-right
---


### Goals

Employees are often the first people to notice that something is wrong.

A suspicious email, fake invoice request, unexpected MFA prompt, strange login page, unusual device behavior, missing files, strange browser pop-up, or suspicious customer message may be reported before any tool raises an alert.

The company needs a simple way for employees to report concerns quickly.

The goal is not to punish mistakes. The goal is to find out early.

If someone clicked a link, opened an attachment, entered a password, approved an MFA prompt, sent money, shared a file, or replied to a suspicious request, the company needs to know immediately.

## Step 1: Define What Employees Should Report

Employees should know what counts as reportable.

**They should report:**

- Suspicious emails
- Unexpected attachments
- Strange links or login pages
- Requests to change bank details
- Urgent payment or gift card requests
- Messages pretending to be from executives
- Unexpected MFA prompts
- Password reset emails they did not request
- New login alerts they do not recognize
- Lost or stolen devices
- Unusual computer behavior
- Pop-ups or browser redirects
- Files missing, renamed, or encrypted
- Shared files that appear public by mistake
- Customer reports of strange emails from the company
- Vendor messages that seem unusual
- Any mistake involving company data, passwords, payments, or sensitive files

The rule should be simple: if it feels wrong, report it.

## Step 2: Create Simple Reporting Channels

Employees should not need to guess where to report something.

**Use one or more clear channels:**

- A dedicated security email address, such as security @ company.com
- A phishing report button in Outlook or Gmail
- A helpdesk or ticketing system
- A Teams, Slack, Mattermost, or internal chat channel for urgent security reports
- A phone number for urgent issues
- A manager escalation path for employees who are unsure
- A web form for non-urgent reports

The reporting path should be easy to remember and visible in training, onboarding, intranet pages, posters, and security reminders.

Do not make employees search through a policy document during a possible incident.

## Step 3: Tell Employees What to Do Immediately

For common situations, give short instructions.

- If the employee received a suspicious email, they should not click links, open attachments, reply, forward it casually, or download files. They should use the report button or send it to the approved security mailbox.

- If the employee clicked a suspicious link, they should report it immediately and say they clicked.

- If the employee entered a password, they should report it immediately and say which account was involved.

- If the employee approved an unexpected MFA prompt, they should report it immediately.

- If the employee opened a suspicious attachment, they should report it and stop using the device until IT or the MSP gives instructions.

- If the employee sent money, changed bank details, shared data, or sent files to the wrong person, they should report it immediately.

This wording matters. Employees should not hide mistakes because they are embarrassed.

## Step 4: Collect the Right Information

The first report does not need to be perfect. It needs enough information for triage.

**Ask employees to include:**

- Who reported it
- When it happened
- What system or account was involved
- What message, file, link, device, or request looked suspicious
- Whether they clicked, replied, downloaded, opened, approved, logged in, sent money, or shared data
- Whether anyone else received the same message
- Screenshots where safe
- The original suspicious email where possible, using the approved report method
- For suspected payment fraud, collect the invoice, bank detail change request, sender address, payment amount, and any approval trail.
- For lost devices, collect the device type, assigned user, last known location, and whether the device contained or accessed company data.

Do not ask employees to investigate on their own. Their job is to report.

## Step 5: Assign Triage Ownership

Every report must go to someone responsible for reviewing it.

This may be the IT lead, MSP, security owner, helpdesk, outsourced SOC, or assigned operations manager.

**Define:**

- Who reviews reports during business hours
- Who handles urgent reports after hours
- Who covers when the main owner is unavailable
- How quickly reports must be reviewed
- Where reports are recorded
- Who can escalate into the Respond section

A report that lands in an unmonitored inbox is not a detection process.

## Step 6: Triage the Report

The triage owner should review the report and decide how serious it is.

**Use simple categories:**

- **Low:** suspicious but no clear action taken and no sensitive system involved.

- **Medium:** user clicked a link, opened an attachment, or interacted with something suspicious, but there is no confirmed compromise yet.

- **High:** password entered, MFA approved, suspicious login detected, sensitive data shared, malware alert triggered, or finance/HR/customer data involved.

- **Critical:** ransomware signs, confirmed account compromise, unauthorized admin access, fraudulent payment, public exposure of sensitive data, backup deletion, active malware, or broad business impact.

The triage owner should record the category, reason, immediate action, and whether escalation is required.

## Step 7: Decide When to Hand Off to Respond

Detect ends when the company decides that a suspicious event needs incident response.

**Escalate into the Respond section when there are signs of:**

- Confirmed malware
- Ransomware behavior
- Compromised email account
- Unauthorized admin access
- Suspicious MFA approval
- Password entered into a fake page
- Fraudulent payment or bank detail change
- Sensitive data sent to the wrong person
- Public exposure of confidential data
- Lost device containing company data
- Former employee access
- Vendor account abuse
- Backup deletion or tampering
- Domain, DNS, website, or cloud account compromise

At handoff, the triage owner should provide the report, timeline, affected account or system, known actions taken, evidence collected, and recommended urgency.

Do not keep serious events stuck in triage.

## Step 8: Record the Outcome and Close the Loop

Every report should have an outcome.

**Possible outcomes include:**

- False alarm
- Blocked phishing attempt
- User education needed
- Password reset completed
- MFA reset completed
- Device checked
- Mailbox reviewed
- Malware removed
- Data exposure confirmed
- Fraud attempt stopped
- Escalated to Respond
- Escalated to legal, insurer, customer, or leadership

The employee should receive a short acknowledgement where appropriate. This encourages future reporting.

The company should also track patterns. If several employees report the same phishing email, the company may need to search for similar messages, block the sender, warn the company, or adjust email filtering.

## Step 9: Test the Reporting Path

Test the reporting process at least quarterly.

**Check that:**

- The report button works.
- The security mailbox is monitored.
- Tickets are created correctly.
- Urgent reports reach the right person.
- After-hours escalation works.
- The MSP knows what to do.
- Employees know where to report.
- Reported emails keep enough technical detail for investigation.
- The handoff to Respond is clear.

A reporting process that has never been tested is not reliable.

## Simple Triage Guide

#### Low concern:

Suspicious email reported, no click, no reply, no attachment opened, no sensitive data involved.

#### Medium concern:

User clicked a link, opened a suspicious file, replied to a suspicious message, or received repeated targeted messages.

#### High concern:

User entered credentials, approved MFA, shared sensitive data, saw suspicious login activity, or a high-risk mailbox or finance process was involved.

#### Critical concern:

Confirmed compromise, malware, ransomware signs, fraudulent payment, public exposure of sensitive data, unauthorized admin access, backup tampering, or active attacker behavior.

## Recommended Open Source and Affordable Tools

|Tool or Solution|Link|Type|Best Use|
|---|---|---|---|
|Microsoft Outlook Report Button|[Microsoft Outlook Report Button](https://learn.microsoft.com/en-us/defender-office-365/submissions-outlook-report-messages)|Included depending on Microsoft 365 configuration|Let users report phishing, junk, and suspicious email directly from Outlook|
|Google Workspace Alert Center|[Google Workspace Alert Center](https://workspace.google.com/products/admin/alert-center/)|Included depending on Google Workspace edition|View security alerts, including phishing, malware, and suspicious account activity|
|Google Workspace Alert Center Help|[Google Alert Center Help](https://knowledge.workspace.google.com/admin/security/about-the-alert-center)|Free resource|Configure and use Google Workspace alert review|
|osTicket|[osTicket](https://osticket.com/)|Open-source|Simple ticketing intake for employee reports and IT/security requests|
|Zammad|[Zammad](https://zammad.org/)|Open-source|Helpdesk and ticketing system for structured reporting and triage|
|Request Tracker|[Request Tracker](https://bestpractical.com/request-tracker)|Open-source with commercial support|Ticketing and workflow management for IT/security requests|
|GLPI|[GLPI](https://glpi-project.org/)|Open-source|IT service management, asset tracking, and ticket handling|
|Jira Service Management|[Jira Service Management](https://www.atlassian.com/software/jira/service-management)|Free tier and commercial|Service desk, incident intake, approval workflows, escalation tracking|
|Freshdesk|[Freshdesk](https://www.freshworks.com/freshdesk/)|Free tier and commercial|Lightweight support inbox and ticketing for small teams|
|TheHive|[TheHive](https://strangebee.com/thehive/)|Commercial with community/project history|Security case management and incident triage for security teams|
|Cortex|[Cortex](https://strangebee.com/cortex/)|Open-source companion tool|Analyze observables such as IPs, domains, hashes, URLs, and email indicators|
|Shuffle|[Shuffle](https://shuffler.io/)|Open-source and commercial|Security automation and SOAR workflows for ticket enrichment and notifications|
|n8n|[n8n](https://n8n.io/)|Source-available and commercial|Workflow automation for routing reports, alerts, tickets, and notifications|
|Node-RED|[Node-RED](https://nodered.org/)|Open-source|Lightweight workflow automation for technical teams|
|Mattermost|[Mattermost](https://mattermost.com/)|Open-source and commercial|Internal chat and urgent security reporting channel|
|Zulip|[Zulip](https://zulip.com/)|Open-source and hosted options|Organized internal chat for security reports and operational threads|
|Rocket.Chat|[Rocket.Chat](https://www.rocket.chat/)|Open-source and commercial|Internal team communication and incident channels|
|Gotify|[Gotify](https://gotify.net/)|Open-source|Self-hosted push notifications for urgent internal alerts|
|ntfy|[ntfy](https://ntfy.sh/)|Open-source and hosted options|Simple push notifications for alerts and escalation|
|Uptime Kuma|[Uptime Kuma](https://uptime.kuma.pet/)|Open-source|Simple monitoring and notification routing for services and websites|
|Healthchecks.io|[Healthchecks.io](https://healthchecks.io/)|Open-source and hosted plans|Monitoring recurring jobs such as backups and scheduled scripts|
|Canarytokens|[Canarytokens](https://canarytokens.org/)|Free|Tripwire-style alerts for suspicious file, link, credential, or system access|
|Phishing Initiative|[Phishing Initiative](https://phishing-initiative.org/)|Free service|Submit and check suspected phishing URLs|
|VirusTotal|[VirusTotal](https://www.virustotal.com/)|Free and commercial|Check suspicious files, URLs, domains, and hashes carefully|
|urlscan.io|[urlscan.io](https://urlscan.io/)|Free and commercial|Analyze suspicious URLs and webpages safely|
|MISP|[MISP](https://www.misp-project.org/)|Open-source|Threat intelligence sharing and indicator tracking for more mature teams|

## Practical Tool Stack for SMEs

#### Very small company:

Use a dedicated security mailbox, Microsoft Outlook Report Button or Gmail reporting, Freshdesk or Jira Service Management free tier, Uptime Kuma or Healthchecks.io, and a simple spreadsheet report register.

#### Microsoft-based SME:

Use the Outlook Report Button, Microsoft Defender for Office 365 submissions, Microsoft 365 alert policies, Jira Service Management or Freshdesk, Teams escalation channel, and a monitored security mailbox.

#### Google Workspace SME:

Use Gmail reporting, Google Workspace Alert Center, Google Admin alerts, Google Forms or a ticketing system for non-email reports, and a monitored security mailbox.

#### Cost-conscious open-source setup:

Use Zammad or osTicket for intake, Mattermost or Zulip for urgent internal reporting, Gotify or ntfy for escalation notifications, Shuffle or n8n for routing, and TheHive or GLPI for structured cases.

#### More mature security team:

Use TheHive for case management, Cortex for observable analysis, Shuffle for automation, MISP for indicator tracking, VirusTotal and urlscan.io for enrichment, and SIEM alerts routed into the case workflow.

## Employee Report Register Template

**The company should maintain a simple report register with these fields:**

- Report ID
- Date and time reported
- Reporter
- Department
- Report type
- System or account involved
- Short description
- User action taken
- Initial triage level
- Triage owner
- Immediate action
- Escalated to Respond
- Final outcome
- Evidence location
- Date closed
- Follow-up needed

## Expected Outputs from This Section

**At the end of this section, the company should have:**

- A clear list of what employees should report.
- One or more simple reporting channels.
- Short instructions for employees after suspicious activity.
- A standard intake format.
- A named triage owner.
- A simple triage method.
- Clear rules for handoff into Respond.
- A report register.
- A process for closing the loop with employees.
- A tested reporting path.

## Practical Rule

Make reporting easy and fast.

Do not punish honest mistakes.

A company should leave this section able to say:

“Employees know what to report, where to report it, what to say, and what to do after reporting. The company knows who reviews reports, how they are triaged, and when they become incident response matters.”

That is employee reporting, triage, and handoff to Respond.

---

