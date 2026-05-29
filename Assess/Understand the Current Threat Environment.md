

icon: rocket



## First Step - Understand Common Attack Types

Before your company can measure its cybersecurity risk, it's best to understand what you are actually defending against. Most cyber incidents do not begin with highly sophisticated “zero-day” attacks. They usually start with common, repeatable weaknesses: a stolen password, a phishing email, an unpatched system, a compromised vendor, or an employee tricked into approving a fraudulent request.

Here at SEIRIM we are continually studying the research from the top large cybersecurity defense providers, network and cloud providers, major tech companies and more as they have the large volumes of data that help uncover what the current trends are in attacks impacting organizations and hence the risks and threats we need to be aware of.

For example Verizon’s 2025 Data Breach Investigations Report analyzed more than 22,000 security incidents and over 12,000 confirmed breaches, showing that companies continue to face recurring risks from credential abuse, vulnerability exploitation, ransomware, and human-driven attacks. ([Verizon](https://www.verizon.com/business/resources/reports/2025-dbir-data-breach-investigations-report.pdf)) 

Microsoft’s 2025 Digital Defense Report also emphasizes that attackers frequently target identity systems, with more than 97% of identity attacks involving password attacks and identity-based attacks rising in the first half of 2025. ([Microsoft](https://www.microsoft.com/en-us/corporate-responsibility/cybersecurity/microsoft-digital-defense-report-2025/))

Overall, the data and trends we find that seem the most balanced among all research we review comes from Mandiant (now part of Google) Based on Mandiant’s _M-Trends 2026 Report_, the top cybersecurity risks for an SME are not exotic “advanced hacker” scenarios. They are practical failure points: exposed systems, weak identity controls, SaaS sprawl, poor monitoring, fragile backups, and employees being manipulated.

Based on trends the top risks to a SME are ranked:

## 1. Exploitation of public-facing systems

This is the top risk from the Mandiant data. Exploits were the most common initial infection vector for the sixth straight year, making up 32% of identified initial infection vectors in 2025. For SMEs, this means exposed VPNs, firewalls, websites, remote access tools, SharePoint servers, outdated SaaS integrations, and business applications are major entry points.

Takeaway: Learn all of your systems that are exposed to the internet, plus all systems that can be accessed by staff to get to know your attack surface.

Assessment questions:

Do we know every internet-facing system we own?

Are VPNs, firewalls, websites, and remote access tools patched quickly?

Do we scan externally exposed assets at least monthly?

## 2. Voice phishing and live social engineering

Mandiant found that voice phishing became the second-most common initial infection vector in 2025, at 11%. This is worse than ordinary phishing because a live person can pressure, adapt, and manipulate the employee in real time. Mandiant specifically notes that interactive attacks are more resilient against automated technical controls.

For SMEs, the highest-risk targets are help desk staff, finance teams, executives, HR, and anyone who can reset passwords, approve payments, or change MFA settings.

Assessment questions:

Can our help desk verify users before resetting passwords or MFA?

Do finance staff verify payment changes through a second channel?

Are employees trained for phone, SMS, WhatsApp, LinkedIn, and QR-code scams, not just email phishing?

## 3. Cloud and SaaS compromise

SMEs often run on Microsoft 365, Google Workspace, CRMs, accounting platforms, cloud drives, HR platforms, and project management tools. Mandiant found that in cloud-related compromises, the top initial vectors were voice phishing at 23%, third-party compromise at 17%, stolen credentials at 16%, email phishing at 15%, insider threat at 14%, and exploits at 6%. Mandiant also found evidence of data theft in 59% of cloud compromises.

This is a major SME risk because cloud compromise can bypass the office network completely. An attacker may not need malware if they can log into email, cloud storage, or admin portals.

Assessment questions:

Do all SaaS admin accounts have MFA?

Do we review external file-sharing permissions?

Do we monitor suspicious logins, mailbox forwarding rules, OAuth apps, and bulk downloads?

## 4. Stolen credentials and weak identity controls

Stolen credentials are a major initial infection vector which can come from infostealers, exposed databases, source-code repositories, dark web forums, or breach leaks. These are cases where the first visible attacker action is simply logging in with valid credentials.

For SMEs, this is brutal because many companies still rely on passwords, shared admin accounts, weak offboarding, reused credentials, and no meaningful access reviews.

Assessment questions:

Is MFA enabled on email, cloud storage, accounting, VPN, admin accounts, and remote access?

Are shared accounts banned?

Are accounts removed immediately when employees, contractors, or vendors leave?

## 5. Ransomware and recovery denial

Ransomware is no longer just a data encryption problem. Modern ransomware groups increasingly target the company’s ability to recover by attacking backups, identity services, and virtualization management planes. Ransomware operators have shifted toward deliberate recovery denial.

For SMEs, this question is not only “Do we have backups?” The real question is: “Can attackers delete, encrypt, or corrupt those backups?”

Assessment questions:

Are backups immutable, offline, or otherwise protected from admin-account compromise?

Have we tested restoration from backups?

Could we recover if our identity system, backup console, and file server were all compromised?

## 6. Third-party and SaaS supply chain compromise

Third-party compromise is defined as attackers using access to one organization’s accounts or infrastructure to reach additional targets. It also notes that third-party compromise includes SaaS platform compromises.

This matters heavily for for your SME as you are likely outsourcing a lot of infrastructure: IT support, payroll, accounting, cloud administration, website development, marketing platforms, CRM management, and payment processing as examples. One weak vendor can become the doorway into the business or itself a point of failure

Assessment questions:

Which vendors have access to our systems or data?

Do vendors use MFA?

Can vendor access be limited, logged, and removed quickly?

## 7. Edge and network device compromise

Mandiant highlights increased attacker focus on edge and core network devices such as VPNs, routers, firewalls, and security appliances. These devices often cannot run normal enterprise security tooling, have long uptime, delayed patching, weak telemetry, and may be excluded from vulnerability management.

For SMEs, this is a hidden risk. Many companies assume the firewall or VPN is protecting them, when in reality that device may itself be exposed, outdated, and poorly monitored.

Assessment questions:

Are firewalls, VPNs, routers, and security appliances included in the asset inventory?

Are their logs collected?

Are they patched and reviewed, or just left running for years?

## 8. Prior compromise and fast attacker hand-offs

Mandiant identifies “prior compromise” as an important infection vector: one actor gains access, then another actor uses that access later. In ransomware cases, prior compromise was the most common initial infection vector at 30%.

This is dangerous for SMEs because a “small” malware infection or suspicious browser download may not stay small. Access can be sold or handed off to a ransomware operator quickly.

Assessment questions:

Do we treat malware infections as serious incidents?

Do we reset credentials after endpoint compromise?

Do we investigate whether one infected machine gave attackers broader access?

## 9. Data theft and extortion

Mandiant identified evidence of data theft in 40% of investigations in 2025. It also notes that stolen data often included credentials, reconnaissance data, customer records, contact details, order information, and other information useful for persistence, lateral movement, privilege escalation, or future voice phishing.

For SMEs, data theft can be more damaging than downtime because it triggers customer trust issues, legal exposure, cyber insurance claims, and potential extortion.

Assessment questions:

Where is sensitive customer, employee, and financial data stored?

Who can export it?

Would we know if someone downloaded a large volume of files?

## 10. Poor detection and logging

Mandiant reported a global median dwell time of 14 days in 2025, up from 11 days in 2024. That means many attackers remain inside environments for days or longer before discovery.

For SMEs, the problem is usually worse because logging is thin, alerts are unmanaged, SaaS logs are ignored, and the MSP may only respond after something visibly breaks.

Assessment questions:

Who receives security alerts?

Are Microsoft 365, Google Workspace, firewall, endpoint, and backup alerts monitored?

Do we have logs that would let us reconstruct what happened after an incident?


## Practical SME Risk Ranking

For an SME cybersecurity assessment, I would prioritize the risks in this order:

1. Internet-facing system exploitation
    
2. Weak identity and stolen credentials
    
3. Cloud/SaaS compromise
    
4. Voice phishing and social engineering
    
5. Ransomware and recovery denial
    
6. Third-party/vendor compromise
    
7. Edge device compromise
    
8. Data theft and extortion
    
9. Prior compromise and malware hand-off
    
10. Poor logging, monitoring, and incident visibility
    

The blunt version for executives: the company is probably not going to be defeated by one magical hacker. It is more likely to be hit through an exposed system, a stolen password, a manipulated employee, a compromised SaaS account, or a backup strategy that fails under pressure. That is what the risk assessment should address first.

