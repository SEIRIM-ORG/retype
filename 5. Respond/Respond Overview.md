---
icon: north-star
order: 100
---

The Respond section defines what the company does after suspicious activity has been confirmed or is serious enough to treat as a possible incident.

Detect is about noticing warning signs. Respond is about taking controlled action.

A response should not depend on panic, guesswork, or one technical person making every decision under pressure. The company should already know who leads the response, who makes business decisions, who contacts vendors, who preserves evidence, who communicates internally, and when outside help is needed.

For SMEs, the goal is not to create a complicated incident command structure. The goal is to move quickly, avoid making the situation worse, contain the damage, preserve useful evidence, and prepare the business for recovery.

### What This Section Covers

The Respond section includes the following main stages:

## 1. Incident Response Ownership and Activation

This subsection defines who leads the response and when the response process begins.

The company should identify an incident response lead, backup lead, executive decision-maker, IT or MSP contact, legal or compliance contact, cyber insurance contact, communications owner, and key business process owners.

It should also define what triggers activation of the response process.

Examples include confirmed malware, ransomware signs, compromised email, unauthorized admin access, suspicious MFA approval, public exposure of sensitive data, fraudulent payment, backup tampering, lost device with company data, domain or DNS compromise, and vendor account abuse.

The practical question is:

“Who takes charge when a possible incident is serious enough to require action?”

## 2. Initial Triage, Evidence, and Incident Classification

This subsection defines how the company confirms what happened without losing evidence or making the incident worse.

The first actions should be controlled. The company should record what was reported, when it was reported, who is affected, which systems or accounts may be involved, what actions have already been taken, and what evidence exists.

Evidence may include emails, screenshots, logs, alert records, device names, user names, IP addresses, file names, URLs, timestamps, tickets, phone notes, and vendor reports.

The incident should then be classified by severity.

A minor suspicious email is not the same as a compromised administrator account. A single malware alert is not the same as ransomware spreading across the network. Classification helps the company decide how urgently to act, who must be involved, and whether outside support is needed.

The practical question is:

“What do we know, what do we not know, what evidence must be preserved, and how serious is this?”

## 3. Containment and Immediate Risk Reduction

This subsection defines the first actions taken to stop the incident from spreading or causing more damage.

Containment may involve disabling a compromised account, resetting passwords, revoking sessions, isolating a device, blocking a sender, removing a malicious inbox rule, disabling external sharing, disconnecting a server, blocking a firewall rule, suspending vendor access, preserving backups, or taking a website offline temporarily.

The company should avoid destructive or rushed actions unless necessary. For example, wiping a device too early may destroy useful evidence. Turning systems off without understanding dependencies may disrupt the business. Restoring from backup before containing the cause may reintroduce the same problem.

Containment should be fast, but controlled.

The practical question is:

“What can we safely do now to stop further damage?”

## 4. Communication, Escalation, and External Support

This subsection defines who must be informed and when.

During an incident, poor communication can make the problem worse. Leadership may not know the business impact. Employees may keep using affected systems. Customers may hear inconsistent information. Vendors may delay support. Insurance reporting deadlines may be missed.

The company should define internal communication paths, leadership updates, employee instructions, vendor notifications, MSP escalation, legal review, insurer notification, law enforcement considerations, and customer or regulatory notification triggers.

Not every incident requires external disclosure. But the company should know who decides, and that decision should not be improvised during the event.

The practical question is:

“Who needs to know, who decides what is said, and who must be contacted for support or obligations?”

## 5. Eradication, Stabilization, and Safe Handoff to Recover

This subsection defines how the company removes the cause of the incident and prepares for recovery.

Eradication means removing the attacker’s access, malicious files, unsafe rules, exposed links, compromised credentials, vulnerable software, unauthorized tools, risky integrations, or misconfigurations that allowed the incident to happen.

Stabilization means confirming the environment is safe enough to begin recovery work.

This may include checking affected accounts, reviewing logs, removing persistence, patching exploited systems, validating endpoint protection, confirming backup integrity, verifying admin access, checking vendor access, reviewing file sharing, and confirming that the incident is no longer active.

Only after containment and stabilization should the company move fully into Recover.

The practical question is:

“Have we removed the cause, stopped the active risk, and confirmed it is safe to restore normal operations?”

## Respond Section Table of Contents

1. Incident Response Ownership and Activation
    
2. Initial Triage, Evidence, and Incident Classification
    
3. Containment and Immediate Risk Reduction
    
4. Communication, Escalation, and External Support
    
5. Eradication, Stabilization, and Safe Handoff to Recover
    

## Expected Outputs from the Respond Section

**At the end of the Respond section, the company should have:**

- A named incident response lead.
- A backup response lead.
- A list of internal and external response contacts.
- Clear incident activation triggers.
- A simple incident severity classification method.
- An evidence collection checklist.
- A containment action guide.
- A communication and escalation plan.
- Cyber insurance, legal, vendor, and MSP contact paths.
- A method for tracking incident actions and decisions.
- A process for confirming the incident has been contained.
- A clear handoff point from Respond into Recover.

## Objectives

Respond is about controlled action under pressure.

A company should leave this section able to say:

“We know who leads, what triggers response, what evidence to preserve, how to contain damage, who to contact, and when recovery can safely begin.”

That is incident response readiness.

---

