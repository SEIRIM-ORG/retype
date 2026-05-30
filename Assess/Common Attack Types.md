---
order: 80
icon: triangle-right
---

## Intro

When you consider your security preparedness, it is useful to look through the lens of the kinds of attacks your company is most likely to experience and need to prepare for.

As we start the cybersecurity risk assessment, the most important attack types to consider are:

- Phishing and social engineering  
- Business email compromise and invoice fraud  
- Stolen credentials and password attacks  
- Ransomware and extortion  
- Unpatched system exploitation  
- Malware and infostealers  
- Cloud and SaaS account compromise  
- Third-party and supply chain compromise  
- DDoS and service disruption  
- Insider threat and human error

As a warm up for the cybersecurity assessments ask “Are we ready for when these kinds of attacks hit our business, and what would happen if they did? How will we react?” 


## 1. Phishing and Social Engineering

Phishing remains one of the most common ways attackers get inside organizations. It works because it targets people, not just technology. Employees may be tricked into clicking malicious links, opening infected attachments, entering passwords into fake login pages, scanning QR codes, or approving requests that appear to come from executives, vendors, or trusted partners.

The FBI reported that phishing and spoofing were the top cybercrime category by complaint volume in its 2024 Internet Crime Report. ([Federal Bureau of Investigation](https://www.fbi.gov/news/press-releases/fbi-releases-annual-internet-crime-report)) CISA also specifically warns small and medium-sized businesses to train employees to recognize phishing because attackers use it to steal sensitive information or deliver malicious attachments. ([CISA](https://www.cisa.gov/audiences/small-and-medium-businesses/secure-your-business))

Assessment question: **Can employees quickly recognize and report suspicious emails, fake login pages, QR-code scams, voice phishing, and impersonation attempts?**

## 2. Business Email Compromise and Invoice Fraud

Business email compromise, or BEC, is one of the most dangerous threats for SMEs because it directly targets money movement. Attackers may compromise or impersonate an executive, supplier, customer, or finance employee, then request a wire transfer, payroll change, invoice payment, or bank-account update.

This is not just an IT issue. It is a finance-control issue. The FBI’s 2025 IC3 report says business email compromise remained one of the largest categories of reported losses, behind investment-related fraud. ([Internet Crime Complaint Center](https://www.ic3.gov/AnnualReport/Reports/2025_IC3Report.pdf)) 

Assessment question: **Do we require out-of-band verification before changing supplier bank details, approving unusual payments, or acting on urgent executive requests?**

## 3. Stolen Credentials and Password Attacks

Many attackers no longer need to “hack” their way in. They simply sign in using stolen or guessed credentials. Password reuse, weak passwords, missing MFA, exposed credentials from previous breaches, and infostealer malware all make this easier.

Microsoft’s 2025 reporting states that more than 97% of identity attacks were password attacks, and that identity-based attacks increased by 32% in the first half of 2025. ([The Official Microsoft Blog](https://blogs.microsoft.com/on-the-issues/2025/10/16/mddr-2025/)) Mandiant’s M-Trends 2025 report also found that stolen credentials became the second most common initial infection vector, representing 16% of intrusions observed in 2024. ([Google Services](https://services.google.com/fh/files/misc/m-trends-2025-en.pdf))

Assessment question: **Do all critical systems use MFA, strong password management, access reviews, and rapid account removal when employees leave?**

## 4. Ransomware and Extortion

Ransomware is no longer just about encrypting files. Many ransomware groups now steal data first, then threaten to leak it if the company does not pay. This creates operational, legal, reputational, and customer-trust consequences.

ENISA’s 2025 threat landscape ranks ransomware among the top threats and identifies it as one of the most impactful cyber threats. ([ENISA](https://www.enisa.europa.eu/topics/cyber-threats/threat-landscape)) Microsoft’s 2025 Digital Defense Report also highlights ransomware and data theft as widespread threats, with financially motivated attacks driving a large share of cyber activity. ([Source](https://news.microsoft.com/source/emea/features/microsoft-digital-defense-report-2025-extortion-and-ransomware-drive-over-half-of-cyberattacks/))

Assessment question: **Could we restore critical operations from clean backups without paying a ransom, and have we actually tested that recovery process?**

## 5. Exploitation of Unpatched Systems

Attackers actively scan the internet for exposed and outdated systems. Unpatched VPNs, firewalls, remote access tools, servers, websites, and business applications can become entry points.

Mandiant’s M-Trends 2026 reporting says exploits remained the most common initial infection vector for the sixth consecutive year, accounting for 32% of intrusions. ([Google Cloud](https://cloud.google.com/blog/topics/threat-intelligence/m-trends-2026)) M-Trends 2025 also found that exploits were the most common initial infection vector in 2024, ahead of stolen credentials and phishing. ([Google Services](https://services.google.com/fh/files/misc/m-trends-2025-en.pdf))

Assessment question: **Do we know which systems are exposed to the internet, and do we patch critical vulnerabilities fast enough?**

## 6. Malware and Infostealers

Malware includes tools that steal passwords, spy on activity, encrypt files, or give attackers remote access. Infostealers are especially dangerous because they quietly collect saved passwords, browser cookies, session tokens, and other credentials that can later be used to access business systems.

Mandiant reported a rise in infostealer use and linked that trend to stolen credentials becoming a major initial infection vector. ([Google Cloud](https://cloud.google.com/blog/topics/threat-intelligence/m-trends-2025)) CrowdStrike’s 2026 Global Threat Report also notes that many modern attacks are “malware-free,” meaning companies cannot rely only on traditional antivirus thinking; attackers increasingly use legitimate tools, valid credentials, and hands-on-keyboard activity. ([CrowdStrike](https://www.crowdstrike.com/en-us/global-threat-report/))

Assessment question: **Do we have endpoint protection, browser credential controls, password managers, and monitoring for suspicious sign-ins?**

## 7. Cloud and SaaS Account Compromise

Many SMEs now run on Microsoft 365, Google Workspace, accounting platforms, CRMs, cloud storage, and project management tools. If attackers compromise these accounts, they may access email, files, invoices, customer data, or admin settings without touching the company’s physical network.

Mandiant’s 2026 reporting found that, in cloud-related compromises, voice phishing, third-party compromise, stolen credentials, email phishing, insider threat, and exploits were all observed initial vectors; it also identified data theft in 59% of cloud compromises. ([Industrial Cyber](https://industrialcyber.co/reports/m-trends-2026-reveals-threat-landscape-shaped-by-faster-coordinated-and-industrialized-cyberattacks/))

Assessment question: **Are SaaS admin accounts protected with MFA, logging, least privilege, external-sharing controls, and regular access reviews?**

## 8. Third-Party and Supply Chain Compromise

A company can have decent internal security and still be compromised through a vendor, IT provider, software supplier, contractor, or SaaS platform. This is a major issue for SMEs because they often outsource IT, payroll, accounting, marketing, development, and cloud administration.

IBM’s 2025 Cost of a Data Breach reporting identified supply chain compromise as one of the most prevalent and costly initial attack vectors, behind phishing in prevalence and among the highest in cost. ENISA’s 2025 threat landscape also highlights collaboration among threat groups and exploitation of vulnerabilities across digital infrastructure. ([ENISA](https://www.enisa.europa.eu/news/etl-2025-eu-consistently-targeted-by-diverse-yet-convergent-threat-groups))

Assessment question: **Which vendors have access to our systems or data, and what security requirements do we impose on them?**

## 9. DDoS and Service Disruption

Distributed denial-of-service attacks flood websites, applications, or online services with traffic to make them unavailable. For SMEs that depend on e-commerce, online booking, customer portals, logistics platforms, or cloud-hosted services, availability attacks can become revenue-impacting events.

ENISA’s 2025 Threat Landscape identifies DDoS attacks as the most prevalent threat in the EU reporting period, with ransomware also ranked at the top. ([ENISA](https://www.enisa.europa.eu/sites/default/files/2026-01/ENISA%20Threat%20Landscape%202025_v1.2.pdf))

Assessment question: **Which online services are revenue-critical, and do we have protection or fallback plans if they become unavailable?**

## 10. Insider Threat and Human Error

Not every incident is caused by an external attacker. Employees, contractors, or administrators may accidentally expose data, misuse access, send files to the wrong person, approve fraudulent requests, or intentionally steal information.

IBM’s 2025 breach research described malicious insider threats as among the costliest attack vectors. But for SMEs, the more common issue may be ordinary human error: weak access controls, unmanaged file sharing, poor offboarding, or accidental disclosure.

Assessment question: **Do employees and contractors only have the access they need, and do we remove that access immediately when their role changes or ends?**

