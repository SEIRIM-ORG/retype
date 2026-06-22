---
icon: shield-check
order: -10
---


Use this checklist to confirm that the company can take controlled action when suspicious activity becomes a possible or confirmed cybersecurity incident.

The goal of Respond is to reduce damage, preserve evidence, contain the incident, coordinate communication, remove the cause, and prepare for safe recovery.

## Incident Response Ownership and Activation Checklist

☐ Assign an incident response lead.

☐ Assign a backup incident response lead.

☐ Identify the executive decision-maker for major business decisions.

☐ Identify the internal IT, MSP, or external technical response contact.

☐ Identify legal, compliance, cyber insurance, communications, HR, finance, and business process contacts where relevant.

☐ Create an incident response contact list with phone numbers, email addresses, vendor contacts, insurance contacts, and after-hours methods.

☐ Store the response contact list somewhere accessible even if email or cloud storage is unavailable.

☐ Define which events activate the incident response process.

☐ Include ransomware signs, confirmed malware, compromised email, unauthorized admin access, suspicious MFA approval, public data exposure, payment fraud, backup tampering, vendor account abuse, lost device with sensitive data, and domain, DNS, website, or cloud compromise.

☐ Define who is authorized to activate the response process.

☐ Record each activation decision with date, time, trigger, affected systems, initial severity, people notified, and immediate actions.

## Initial Triage, Evidence, and Incident Classification Checklist

☐ Open an incident record.

☐ Assign an incident owner.

☐ Record who reported the issue, when it was reported, how it was detected, and what system, account, device, vendor, or process may be affected.

☐ Preserve the first evidence before deleting, rebuilding, wiping, or changing systems.

☐ Preserve suspicious emails, headers, screenshots, URLs, files, alerts, logs, user statements, tickets, vendor reports, payment requests, and system records where available.

☐ Identify the initial affected scope.

☐ Check whether one user, many users, one device, many devices, one mailbox, one SaaS platform, one vendor, one file share, one website, or the wider company may be involved.

☐ Check whether the incident appears active.

☐ Look for active suspicious sessions, new mailbox rules, ongoing file changes, malware alerts, VPN sessions, public links, backup deletion activity, website changes, or continued data downloads.

☐ Collect the most important technical facts.

☐ Include usernames, device names, IP addresses, source locations, login times, domains, URLs, email senders, attachment names, file names, alert names, system names, and business process impact.

☐ Classify the incident as low, medium, high, or critical.

☐ Update severity if new facts show greater risk or wider impact.

☐ Decide the next action.

☐ Create a short situation summary for leadership, IT, MSP, legal, insurance, or external responders if needed.

## Containment and Immediate Risk Reduction Checklist

☐ Confirm who is authorized to approve containment actions.

☐ Record the current facts before making major changes.

☐ Decide whether the incident is active and whether urgent containment is required.

☐ Revoke suspicious sessions.

☐ Disable or restrict compromised accounts.

☐ Reset passwords where appropriate.

☐ Review and reset MFA methods where needed.

☐ Remove suspicious mailbox forwarding, inbox rules, delegated access, and OAuth app approvals.

☐ Isolate affected devices or servers where needed.

☐ Stop ransomware-like activity, mass file changes, or malware spread.

☐ Disable public links or exposed data access.

☐ Close unsafe remote access paths, such as public RDP, public SSH, exposed databases, broad VPN access, or exposed admin panels.

☐ Suspend suspicious vendor, MSP, contractor, or remote support access.

☐ Protect backup systems from deletion, encryption, tampering, or unsafe restoration.

☐ Block known malicious senders, domains, URLs, IP addresses, file hashes, or command-and-control destinations where useful.

☐ Pause risky business processes where needed, including payments, bank-detail changes, payroll changes, customer data sharing, or vendor approvals.

☐ Contact MSPs, SaaS vendors, hosting providers, cloud providers, backup providers, domain registrars, DNS providers, or incident response support where needed.

☐ Verify that containment worked.

☐ Confirm attacker access has been interrupted, affected systems are contained, related activity has been checked, monitoring still works, and business impact is understood.

☐ Record every major containment action, approval, result, and follow-up.

## Communication, Escalation, and External Support Checklist

☐ Assign a communication owner.

☐ Notify leadership early when the incident may affect operations, finance, customer data, employee data, legal obligations, reputation, or recovery capability.

☐ Give leadership a short factual update with what happened, what may be affected, whether the incident appears active, what actions were taken, what decisions are needed, and when the next update will be provided.

☐ Give employees clear instructions if they need to avoid affected systems, report related activity, stop using email, avoid suspicious messages, or follow alternate procedures.

☐ Use safe communication channels if email, chat, identity, or admin systems may be compromised.

☐ Escalate to technical support when the company cannot safely contain or investigate the issue alone.

☐ Contact cyber insurance, legal, or compliance support when data theft, personal information, payment fraud, ransomware, business interruption, customer obligations, regulatory obligations, or legal exposure may be involved.

☐ Control external communication to customers, vendors, regulators, law enforcement, media, or the public.

☐ Avoid speculation, blame, unsupported reassurance, or unapproved customer-facing statements.

☐ Record internal updates, leadership decisions, vendor contacts, insurance notices, legal guidance, customer communications, and external support actions.

## Eradication, Stabilization, and Safe Handoff to Recover Checklist

☐ Confirm the known affected scope before cleanup.

☐ Remove attacker access.

☐ Secure compromised accounts, revoke sessions, reset passwords, review MFA, remove unauthorized roles, disable suspicious vendor access, and rotate exposed tokens or keys.

☐ Remove malicious artifacts and persistence.

☐ Check for malware files, scripts, scheduled tasks, startup items, malicious services, web shells, suspicious users, mailbox rules, forwarding, OAuth apps, API tokens, SSH keys, firewall rules, remote tools, and cloud automation.

☐ Patch or mitigate the weakness that allowed the incident.

☐ Fix exposed services, vulnerable software, unsafe firewall rules, public sharing, weak remote access, website vulnerabilities, cloud misconfigurations, or missing MFA.

☐ Clean affected email, cloud, SaaS, and collaboration platforms.

☐ Review forwarding, inbox rules, delegated access, suspicious sent mail, OAuth apps, API keys, guest users, public links, admin roles, data exports, and audit log settings.

☐ Decide whether affected devices or servers should be cleaned, rebuilt, replaced, or kept isolated.

☐ Rebuild from trusted media when compromise is serious, persistence is unclear, admin access was abused, ransomware was present, or the system cannot be trusted.

☐ Validate backups before recovery.

☐ Confirm restore points exist, backup integrity is acceptable, backup storage was not tampered with, and selected restore points are likely clean.

☐ Rotate exposed credentials, secrets, and keys.

☐ Include user passwords, admin passwords, service accounts, API keys, SSH keys, cloud keys, application secrets, database credentials, backup credentials, and vendor portal credentials where needed.

☐ Verify eradication through hunting and rescanning.

☐ Search for known indicators across endpoints, servers, logs, email, cloud, SaaS, VPN, websites, backups, and admin systems.

☐ Stabilize core security controls.

☐ Confirm MFA, logging, alerts, endpoint protection, backups, firewall rules, VPN controls, email security, SaaS sharing controls, cloud audit logs, website protection, patching, and admin restrictions are working.

☐ Stabilize affected business processes.

☐ Review finance, HR, customer data, vendor access, payroll, service delivery, and operational workarounds where relevant.

☐ Monitor closely after eradication for recurring suspicious activity.

☐ Decide whether the environment is safe enough for recovery.

☐ Prepare the handoff package for the Recover section.

☐ Record residual risks, exceptions, temporary controls, owners, due dates, and leadership approvals.

## Final Respond Section Outputs

☐ Incident response lead assigned.

☐ Backup response lead assigned.

☐ Response team identified.

☐ Response contact list completed and stored safely.

☐ Activation triggers defined.

☐ Incident record opened when needed.

☐ Evidence preserved.

☐ Initial scope identified.

☐ Incident severity classified.

☐ Situation summary created.

☐ Containment actions completed.

☐ Containment verified.

☐ Communication owner assigned.

☐ Leadership notification process used.

☐ Employee instructions issued where needed.

☐ MSP, vendor, legal, insurance, or external support contacted where needed.

☐ Communications and decisions recorded.

☐ Attacker access removed.

☐ Malicious artifacts and persistence removed.

☐ Exploited weaknesses patched or mitigated.

☐ Affected email, cloud, SaaS, websites, devices, servers, and accounts cleaned or secured.

☐ Credentials, secrets, and keys rotated where needed.

☐ Backups verified before recovery.

☐ Core security controls stabilized.

☐ Business process controls stabilized.

☐ Post-eradication monitoring started.

☐ Residual risks documented.

☐ Recover handoff package completed.

☐ Leadership approval recorded before moving into Recover.

## Objective

Respond is controlled action under pressure.

The company should leave this section able to say:

“We know who leads the response, how incidents are triaged, what evidence must be preserved, how damage is contained, who must be contacted, how the cause is removed, and when it is safe to move into recovery.”

---

