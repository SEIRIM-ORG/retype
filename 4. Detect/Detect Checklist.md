---
icon: shield-check
order: -10
---

Use this checklist to confirm that the company can notice suspicious activity, control failures, and possible incidents early enough to act.

The goal of Detect is not to monitor everything. The goal is to make sure the company is watching the most important systems, receiving the right alerts, reviewing reports, and escalating serious issues into the Respond section.

## Detection Ownership and Coverage Checklist

☐ Assign a detection owner.

☐ Assign a backup detection owner.

☐ Confirm whether detection is handled internally, by IT, by an MSP, by a vendor, or by a combination of these.

☐ Identify the systems that must be covered by detection.

☐ Include email, identity, Microsoft 365 or Google Workspace, endpoint protection, servers, firewalls, VPN, backups, cloud storage, SaaS tools, websites, domain registrar, DNS provider, accounting, payroll, CRM, and remote support tools.

☐ Define where alerts go, such as a security mailbox, ticket queue, MSP dashboard, SIEM, or monitoring platform.

☐ Avoid sending important alerts only to one person’s inbox.

☐ Define which alerts need immediate escalation.

☐ Create a detection coverage register.

☐ Review detection coverage when new systems, vendors, websites, cloud platforms, or remote access tools are added.

## Logging, Alerts, and Visibility Checklist

☐ Assign an owner for logging and alerts.

☐ Enable key logs for important systems.

☐ Include sign-in logs, admin activity logs, email security logs, endpoint alerts, firewall logs, VPN logs, backup logs, SaaS audit logs, cloud audit logs, website logs, DNS logs, and domain registrar activity where available.

☐ Confirm that critical alerts go to a monitored destination.

☐ Create priority levels for alerts.

☐ Define critical alerts, high-priority alerts, normal alerts, and informational alerts.

☐ Monitor for suspicious logins, MFA failures, MFA resets, new admin accounts, privilege changes, mailbox forwarding rules, malware detections, disabled security tools, public file sharing, large downloads, VPN anomalies, backup failures, and DNS changes.

☐ Set log retention expectations.

☐ Protect the logging platform with MFA, limited admin access, and restricted deletion rights.

☐ Test important alerts.

☐ Create a log and alert register.

☐ Keep evidence of log settings, alert settings, test results, reports, and exceptions.

## Main Attack Path Monitoring Checklist

☐ Identify the main attack paths most relevant to the company.

☐ Include identity compromise, email compromise, endpoint malware, cloud and SaaS misuse, remote access abuse, website compromise, data exposure, backup tampering, admin misuse, and vendor access abuse.

☐ Monitor identity activity for suspicious sign-ins, impossible travel, failed login spikes, MFA reset abuse, new admin roles, inactive accounts becoming active, and former employee login attempts.

☐ Monitor email for phishing, malware, spoofing, suspicious inbox rules, mailbox forwarding, executive impersonation, unusual sending behavior, and business email compromise signs.

☐ Monitor endpoints and servers for malware, ransomware behavior, suspicious scripts, unauthorized remote tools, disabled protection tools, unusual command-line activity, and devices that stop reporting.

☐ Monitor cloud and SaaS platforms for public sharing, guest access changes, mass downloads, data exports, OAuth apps, API keys, integrations, and admin changes.

☐ Monitor remote access and network entry points for unusual VPN activity, public RDP or SSH, firewall changes, new port forwards, exposed services, and vendor access.

☐ Monitor websites and CMS platforms for admin login activity, plugin risk, file changes, vulnerable components, public exposure, and suspicious uploads.

☐ Monitor backups and security controls for failures, deletion activity, disabled protection, stopped agents, disabled logging, failed patches, and storage capacity problems.

☐ Create a main attack path monitoring register.

☐ Review attack path monitoring at least quarterly.

## External Exposure and Control Failure Checklist

☐ Define what should never be public.

☐ Include admin panels, databases, backup consoles, network management pages, RDP, SSH, internal dashboards, staging sites, test sites, printer interfaces, camera systems, internal APIs, and sensitive file locations.

☐ Create an external exposure watchlist.

☐ Include domains, subdomains, public IPs, websites, APIs, VPN portals, remote access portals, DNS records, SSL/TLS certificates, hosting accounts, cloud storage, and externally shared SaaS folders.

☐ Run regular external exposure checks on company-owned systems.

☐ Review open ports, exposed services, public admin panels, exposed databases, old websites, staging sites, weak TLS settings, risky DNS records, and public cloud storage.

☐ Monitor critical control failures.

☐ Include backup failures, endpoint protection failures, devices that stop reporting, MFA disabled, audit logging disabled, firewall logging disabled, admin accounts added, public sharing enabled, DNS changes, domain changes, and SSL/TLS certificate expiry.

☐ Send exposure and control failure alerts to a monitored destination.

☐ Assign owners to findings.

☐ Fix findings and verify that the exposure or failure has been resolved.

☐ Create an exposure and control failure register.

## Employee Reporting, Triage, and Handoff Checklist

☐ Define what employees should report.

☐ Include suspicious emails, unexpected attachments, strange links, fake login pages, unexpected MFA prompts, password reset emails, payment change requests, lost devices, unusual computer behavior, missing files, public sharing mistakes, and suspicious customer or vendor messages.

☐ Create simple reporting channels.

☐ Include a security email address, phishing report button, ticketing system, chat channel, phone path, manager escalation path, or web form.

☐ Give employees clear instructions for what to do if they clicked, opened, replied, entered a password, approved MFA, sent money, shared data, or lost a device.

☐ Define what information employees should include in a report.

☐ Assign a triage owner.

☐ Define triage levels for low, medium, high, and critical reports.

☐ Escalate serious events into the Respond section.

☐ Include confirmed malware, ransomware signs, compromised email, unauthorized admin access, suspicious MFA approval, password entered into a fake page, fraudulent payment, public data exposure, former employee access, vendor abuse, backup tampering, and domain or DNS compromise.

☐ Record the report, triage level, action taken, evidence, outcome, and handoff decision.

☐ Acknowledge reports where appropriate so employees continue reporting quickly.

☐ Test the reporting path at least quarterly.

## Final Detect Section Outputs

☐ Detection owner assigned.

☐ Backup detection owner assigned.

☐ Detection coverage register created.

☐ Important systems included in monitoring coverage.

☐ Alert destinations defined.

☐ Key logs enabled.

☐ Critical alerts identified.

☐ Log retention expectations defined.

☐ Important alert paths tested.

☐ Main attack paths identified.

☐ Attack path monitoring register created.

☐ External exposure watchlist created.

☐ Control failure monitoring defined.

☐ Exposure and control failure register created.

☐ Employee reporting channels created.

☐ Triage process defined.

☐ Handoff criteria to Respond defined.

☐ Evidence stored.

☐ Review schedule created.

☐ Priority unresolved gaps carried forward into Respond, Recover, Review, or future improvement plans.