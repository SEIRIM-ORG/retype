---
icon: shield-check
order: -10
---


Use this checklist to confirm that the company can restore systems, data, access, and business operations safely after an incident.

The goal of Recover is to restore normal operations without restoring the weakness, compromise, unsafe access, or failed control that caused the incident.

## Recovery Ownership, Priorities, and Readiness Checklist

☐ Assign a recovery lead.

☐ Assign a backup recovery lead.

☐ Identify the executive decision-maker for recovery approval.

☐ Identify technical owners, business process owners, backup owners, SaaS or cloud administrators, MSP contacts, vendor contacts, and legal or insurance contacts where needed.

☐ Confirm that containment and stabilization are complete enough for recovery to begin.

☐ Confirm that active attacker access has been interrupted.

☐ Confirm that compromised accounts are secured.

☐ Confirm that affected systems are isolated, cleaned, rebuilt, or ready for restoration.

☐ Confirm that known persistence has been removed or controlled.

☐ Confirm that exploited weaknesses are patched or mitigated.

☐ Confirm that backups are protected and restore points have been reviewed.

☐ Prioritize recovery by business impact and dependencies.

☐ Create a recovery priority list with system, owner, dependency, restore source, readiness status, expected recovery time, and validation owner.

☐ Record approval to begin recovery.

## Restore Systems, Data, and Access Safely Checklist

☐ Restore systems in approved priority order.

☐ Use trusted restore sources, such as clean backups, approved system images, trusted installation media, vendor restore points, or rebuilt cloud resources.

☐ Avoid restoring backups, images, or configurations that may contain the same compromise.

☐ Restore to a controlled environment first where practical.

☐ Rebuild high-risk systems instead of trusting them when compromise is serious or persistence is unclear.

☐ Restore only the data needed for business operations.

☐ Check restored data for completeness, corruption, encryption, malware, exposed secrets, and unsafe permissions.

☐ Restore user access in stages.

☐ Confirm password resets, MFA review, session revocation, and permission review before restoring access for affected accounts.

☐ Apply security controls before reconnecting systems to normal use.

☐ Confirm MFA, endpoint protection, logging, alerts, patching, firewall rules, backups, encryption, admin restrictions, and secure configuration are active.

☐ Restore integrations, APIs, service accounts, vendor access, and third-party apps carefully.

☐ Rotate keys, tokens, service credentials, SSH keys, API keys, and vendor credentials where needed.

☐ Confirm backups resume after each restored system returns to operation.

☐ Monitor restored systems closely for recurring suspicious activity.

☐ Record each restoration action, approval, restore source, validation result, issue found, and remaining risk.

## Validate Restored Systems and Business Operations Checklist

☐ Confirm each restored system is reachable and functioning.

☐ Confirm required services, applications, databases, DNS, certificates, integrations, storage, scheduled tasks, and logs are working.

☐ Validate restored data.

☐ Confirm important files, records, databases, customer data, finance data, HR records, order history, website content, and application data are present and usable.

☐ Review access and permissions.

☐ Confirm users, administrators, vendors, guests, service accounts, groups, and shared accounts have only required access.

☐ Review public links, external sharing, guest access, admin roles, delegated access, OAuth apps, API keys, and group membership.

☐ Confirm security controls are active.

☐ Check MFA, endpoint protection, EDR or antivirus, logging, alerting, patching, firewall rules, VPN restrictions, encryption, SaaS sharing controls, cloud audit logs, website protections, and admin restrictions.

☐ Confirm backups and monitoring resumed.

☐ Test key business processes with business owners.

☐ Confirm users can log in, required data is present, transactions can be processed, reports can be generated, customers can be served, payments or approvals work, and operations can continue safely.

☐ Monitor restored systems for recurrence.

☐ Record validation results for each restored system or process.

☐ Document residual risks and approval for normal or limited use.

## Communication and Business Continuity During Recovery Checklist

☐ Assign a recovery communication owner.

☐ Identify who needs recovery updates.

☐ Include leadership, IT or MSP, department managers, employees, customer service, finance, HR, sales, operations, vendors, customers, partners, legal, compliance, and insurance contacts where relevant.

☐ Use clear system status categories.

☐ Mark systems as unavailable, restoring, available for testing, available for limited use, available for normal use, or restricted until further notice.

☐ Give employees clear instructions on which systems to use, which systems to avoid, what temporary procedures apply, and what suspicious activity to report.

☐ Manage temporary workarounds.

☐ Assign an owner, start time, expected end time, security rules, approval requirements, and recordkeeping method for each workaround.

☐ Avoid unsafe workarounds such as personal email, unmanaged file sharing, shared passwords, uncontrolled spreadsheets, or unapproved messaging apps unless formally approved as an emergency exception.

☐ Control customer, vendor, and partner communication.

☐ Use approved talking points where external communication is needed.

☐ Avoid speculation, blame, unsupported reassurance, or claims that have not been verified.

☐ Record major recovery communication and business continuity decisions.

☐ Confirm when temporary workarounds can end.

☐ Communicate recovery completion or remaining limits.

## Recovery Documentation and Handoff to Review Checklist

☐ Confirm what was restored.

☐ Record systems, data, devices, accounts, SaaS platforms, cloud services, websites, integrations, vendor access, backups, and business processes restored.

☐ Document how recovery was completed.

☐ Include backup restores, rebuilds, account re-enablement, credential rotation, SaaS configuration changes, file permission corrections, website restoration, cloud changes, vendor access changes, and business process workarounds.

☐ Attach validation evidence.

☐ Include screenshots, logs, tickets, backup restore reports, endpoint protection reports, monitoring dashboards, access review notes, vulnerability scan results, cloud audit records, website test results, user acceptance notes, and business owner sign-off.

☐ Document remaining risks and open issues.

☐ Record owner, reason open, temporary control, business impact, due date, approval, and review date for each remaining issue.

☐ Confirm temporary workarounds are closed, extended, replaced, or formally approved as exceptions.

☐ Prepare a recovery closure summary.

☐ Include what happened, what was affected, what was restored, what was rebuilt, what controls were verified, what business processes were validated, what remains unresolved, and what must be reviewed next.

☐ Get technical owner sign-off.

☐ Get business owner sign-off.

☐ Get leadership approval that recovery is complete, conditionally complete, or still in progress.

☐ Store recovery records safely in a controlled location.

☐ Set follow-up dates for unresolved recovery actions.

☐ Prepare the handoff package for the Review section.

## Final Recover Section Outputs

☐ Recovery lead assigned.

☐ Backup recovery lead assigned.

☐ Recovery roles confirmed.

☐ Recovery priorities defined.

☐ Recovery readiness confirmed.

☐ Approval to begin recovery recorded.

☐ Systems restored in priority order.

☐ Trusted restore sources used.

☐ High-risk systems rebuilt where needed.

☐ Data restored and checked.

☐ Access restored in stages.

☐ Security controls applied before normal use.

☐ Integrations and vendor access reviewed.

☐ Credentials, secrets, and keys rotated where needed.

☐ Backups confirmed after restoration.

☐ Restored systems monitored closely.

☐ Technical validation completed.

☐ Business process validation completed.

☐ Recovery communications controlled.

☐ Temporary workarounds documented.

☐ Temporary workarounds closed or approved as exceptions.

☐ Restoration actions documented.

☐ Validation evidence attached.

☐ Residual risks documented.

☐ Technical owner sign-off recorded.

☐ Business owner sign-off recorded.

☐ Leadership approval recorded.

☐ Recovery records stored safely.

☐ Follow-up actions assigned.

☐ Handoff package prepared for the Review section.

## Objective

Recovery is not complete when systems turn back on.

The company should leave this section able to say:

“We restored systems safely, validated that they work, confirmed security controls are active, documented remaining risks, obtained approval, and handed the incident to Review for improvement.”

---

