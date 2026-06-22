---
icon: north-star
order: 100
---


The Detect section of the playbook helps prepare how the company notices suspicious activity before it becomes a larger incident.

Protection controls reduce risk, but they do not stop everything. A phishing email may get through. A password may be stolen. A laptop may become infected. A cloud folder may be shared publicly. A firewall rule may expose a system by mistake. A vendor account may be abused. A backup job may fail quietly.

The company needs a way to see these warning signs.

Detect is not only about security tools. It is about knowing which systems need visibility, which alerts matter, who receives them, who reviews them, and when suspicious activity should be escalated.

For SMEs, the goal is not to build a large security operations center. The goal is to make sure important warning signs are not missed.

## 1. Detection Ownership and Coverage

This subsection defines who is responsible for detection and which systems are included.

The company should name the person, team, MSP, or vendor responsible for receiving, reviewing, and escalating security alerts. It should also define who covers this responsibility when the main owner is unavailable.

Detection coverage should include the systems most likely to show early signs of trouble: email, identity platforms, Microsoft 365 or Google Workspace, endpoints, servers, firewalls, VPN, backup systems, cloud storage, SaaS platforms, websites, domain registrar, DNS provider, accounting, payroll, CRM, and other business-critical tools.

The practical question is:

“Who is watching the important systems, and what are they responsible for noticing?”

## 2. Logging, Alerts, and Security Visibility

This subsection defines which logs and alerts the company needs.

If logs are not enabled, the company may not know what happened during an incident. It may not be able to see who logged in, what changed, which files were accessed, whether data was exported, or how an attacker moved through the environment.

Important logs may include sign-in logs, admin activity logs, email security logs, endpoint alerts, firewall logs, VPN logs, cloud audit logs, SaaS audit logs, website logs, backup logs, DNS logs, and remote access logs.

The company should also define which events must generate alerts. Important alerts may include suspicious logins, repeated failed logins, MFA failures, new admin accounts, privilege changes, mailbox forwarding rules, malware detections, ransomware-like activity, disabled security tools, public file sharing, unusual data downloads, VPN logins from unusual locations, backup failures, and domain or DNS changes.

The practical question is:

“If something suspicious happens, will we see it, and will someone be notified?”

## 3. Monitoring the Main Attack Paths

This subsection defines what the company should watch across the systems attackers usually target first.

Identity monitoring should look for suspicious sign-ins, impossible travel, repeated failed logins, MFA reset abuse, new admin roles, inactive accounts becoming active, and unusual vendor access.

Email monitoring should look for phishing, malware, spoofing, executive impersonation, suspicious inbox rules, hidden forwarding, unusual sending behavior, and signs of business email compromise.

Endpoint and server monitoring should look for malware, ransomware behavior, disabled security tools, suspicious scripts, unauthorized remote tools, unusual command-line activity, privilege escalation, and unknown software.

Cloud and SaaS monitoring should look for public file sharing, mass downloads, new integrations, suspicious OAuth apps, API key misuse, admin changes, data exports, and guest access changes.

Network monitoring should look for unusual VPN activity, exposed services, suspicious DNS activity, unexpected outbound traffic, firewall changes, and signs of internal scanning.

The practical question is:

“What activity would show that an account, device, system, cloud platform, or network path may be compromised?”

## 4. External Exposure and Control Failure Detection

This subsection defines how the company notices when something becomes exposed, disabled, broken, or misconfigured.

Many incidents begin because a control failed quietly. MFA was disabled. A backup job stopped. Endpoint protection stopped reporting. A firewall rule was added. A public link was created. A domain record was changed. A website plugin became vulnerable. A cloud storage bucket became public. A device stopped checking in.

The company should regularly check for control failures and accidental exposure.

This should include public IP reviews, domain and subdomain reviews, external port checks, public cloud storage checks, SSL/TLS checks, security header checks, backup failure checks, endpoint protection health checks, patch visibility checks, SaaS sharing reviews, and admin console reviews.

The practical question is:

“Would we notice if an important protection stopped working or something sensitive became public?”

## 5. Employee Reporting, Triage, and Handoff to Respond

Employees are part of detection.

A person may notice a suspicious email, strange login prompt, unexpected MFA notification, fake invoice request, unusual device behavior, missing files, strange browser pop-up, suspicious customer message, or unauthorized bank detail change before any tool does.

The company should make reporting simple. Employees should know what to report, where to report it, what information to include, and what to do if they clicked something, approved something, entered a password, or sent data to the wrong place.

Reports and alerts should then go through a simple triage process.

Not every alert is an incident. But serious warning signs need a clear path into the Respond section.

Examples that should usually be escalated include confirmed malware, ransomware signs, unauthorized admin access, suspicious MFA reset, compromised mailbox, external data sharing, unusual financial request, public exposure of sensitive data, suspicious vendor access, backup deletion activity, or confirmed access by a former employee.

The practical question is:

“When something suspicious appears, who reviews it, how fast do they review it, and when does it become an incident response matter?”

## Table of Contents

1. Detection Ownership and Coverage
    
2. Logging, Alerts, and Security Visibility
    
3. Monitoring the Main Attack Paths
    
4. External Exposure and Control Failure Detection
    
5. Employee Reporting, Triage, and Handoff to Respond
    

## Expected Outputs from the Detect Section

At the end of the Detect section, the company should have a:

- Named detection owner.
- List of systems covered by monitoring.
- List of important logs that must be enabled.
- List of alerts that must be reviewed.
- Defined destination for alerts and suspicious reports.
- Simple employee reporting path.
- Process for reviewing suspicious activity.
- List of control failures that must be noticed.
- Triage method for deciding what needs escalation.
- Clear handoff point from Detect into Respond.


## Objectives

Detection only works when someone is responsible for seeing the signal and acting on it.

A company should leave this section able to say:

“We know what we are watching, where alerts go, who reviews them, what counts as suspicious, and when to escalate.”

That is detection.

---

