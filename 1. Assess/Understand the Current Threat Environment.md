---
icon: triangle-right
order: 70
---


## Key Step - Awareness of Current Trends

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

For an SME cybersecurity assessment, we would prioritize the risks in this order:

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
    


## Practical Tasks for the Company

The company should perform the following tasks in this section.

## Task 1: Assign Ownership for Threat Awareness

The company should assign a specific person or role to monitor the current threat environment. This may be an internal IT lead, security lead, operations manager, MSP contact, or executive sponsor.

The owner is not responsible for solving every issue in this section. Their job is to make sure the company is not blind to major threat developments that may affect its systems, vendors, employees, or industry.

**The company should document:**

- Threat awareness owner  
- Backup owner  
- MSP or external security contact  
- Executive sponsor  
- Review frequency

## Task 2: Create a Trusted Source List

The company should define which sources it will use to understand current cybersecurity threats. This prevents the organization from relying on random social media posts, vendor fear marketing, or outdated advice.

**Useful sources may include:**

- CISA Known Exploited Vulnerabilities Catalog  
- CISA advisories and alerts  
- Vendor security advisories for systems the company uses  
- Microsoft security advisories  
- Google Workspace security updates  
- Firewall, VPN, backup, endpoint, and SaaS vendor notices  
- Cyber insurance advisories  
- MSP security bulletins  
- Industry-specific security groups or ISACs where applicable  
- Major annual threat reports from reputable cybersecurity firms

The output should be a short list of approved threat intelligence sources.

## Task 3: Create a Regularly Updated Threat Environment Snapshot

The company should produce a short summary of the threat environment on a regular basis (monthly or quarterly depending on available staff time). This should be no more than one or two pages.

**The snapshot should answer:**

- What major threats are currently active?

- Which technologies are being targeted?

- Are there newly exploited vulnerabilities affecting common business systems?

- Are attackers targeting cloud, SaaS, identity, VPNs, firewalls, or backup systems?

- Are there active scams or fraud tactics relevant to the company?

- Are there current ransomware or extortion trends the company should know about?

- Does any recent news affect the company’s industry, vendors, or technology stack?

The output should be a monthly threat environment summary.

## Task 4: Maintain a Technology Watchlist

The company should maintain a simple watchlist of technologies that require active security awareness.

This is not the full asset inventory that occurs in the Identify phase but just the initial precursor draft list focusing on technologies that are commonly targeted or especially important to the business.

**Examples:**

- Microsoft 365 or Google Workspace  
- VPN or remote access platform  
- Firewall and router products  
- Endpoint protection platform  
- Backup platform  
- Accounting system  
- Payroll system  
- CRM  
- Website CMS  
- Cloud storage  
- Password manager  
- Remote monitoring and management tools  
- Developer tools and code repositories  
- Major SaaS platforms containing sensitive data

The output should be a short technology watchlist used for monitoring relevant threat news.

## Task 5: Track Threats by Business Relevance

The company should not try to follow every global cybersecurity headline. Instead, it should tag current threats by whether they are relevant to the company.

**Use simple categories:**

**Relevant now:** affects a system, vendor, process, or industry the company uses.

**Possibly relevant:** may affect the company, but more information is needed.

**Not currently relevant:** important generally, but no clear connection to the company.

This is not the formal risk score. That happens later. The purpose here is to filter the noise so leadership and IT can focus attention.

The output should be a relevance-filtered list of current threats.

## Task 6: Identify Threat Triggers That Require Internal Review

The company should define which types of threat news require immediate internal attention.

**Examples of triggers:**

- A CISA KEV entry affects a product the company uses.

- A firewall, VPN, remote access, or SaaS platform used by the company has an actively exploited vulnerability.

- A vendor announces a breach involving customer data, credentials, or integrations.

- A ransomware group is actively exploiting a technology the company uses.

- A cyber insurer or MSP issues an urgent advisory.

- A major SaaS provider used by the company reports suspicious token, OAuth, or account activity.

- A known scam targets the company’s industry, finance process, or customer base.

The output should be a list of threat triggers and who must be notified when they occur.

## Task 7: Review Current Threats with the MSP or IT Provider

If the company uses an MSP or outsourced IT provider, it should ask for a short threat review on a regular basis.

**The company should ask:**

- Are any current exploited vulnerabilities relevant to our environment?

- Have any of our vendors or tools issued urgent advisories?

- Are our internet-facing systems affected by current attack campaigns?

- Have you seen increased phishing, ransomware, SaaS compromise, or fraud attempts among similar clients?

- Are there any immediate issues we should carry into the formal risk assessment?

The output should be a short MSP or IT-provider threat note.


## Task 8: Brief Leadership on the Current Threat Environment

Leadership should receive a short, plain-language briefing on the current threat environment.

The briefing should include:

- Top current cybersecurity trends relevant to SMEs

- Threats most relevant to the company’s systems and workflows

- Known urgent issues affecting company technologies, if any

- Major assumptions or unknowns that need follow-up

- Items that should be carried forward into the risk assessment

The output should be a short executive threat briefing.

## Expected Outputs from This Section

**At the end of this section, the company should have:**

- A named owner for monitoring the threat environment.

- A trusted source list for cybersecurity threat information.

- A monthly or quarterly threat environment snapshot.

- A technology watchlist for threat monitoring.

- A relevance-filtered list of current threats.

- A list of trigger events requiring internal review.

- Notes from the MSP or IT provider, where applicable.

- A plain-language executive briefing.

- A list of unknowns to carry into later Assess activities.


## Sources for Cybersecurity Threat Intelligence

Select from the following governmental, open source, and commercial platforms to remain aware of the current threat environment:

Below is a practical source list I would include in the **Understand the Current Threat Environment** section. The company should not try to monitor everything. The strongest model is to maintain a short trusted source list, assign an owner, and review it monthly or when an urgent advisory affects company technology.

## Minimum Source Stack for Most SMEs

These are the sources we recommend looking to for SMEs:

|Source|Link|Use It For|
|---|---|---|
|CISA Known Exploited Vulnerabilities Catalog|[CISA KEV Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog)|Confirmed exploited vulnerabilities. This should be checked against the company’s technology watchlist.|
|CISA Cybersecurity Advisories|[CISA Cybersecurity Advisories](https://www.cisa.gov/news-events/cybersecurity-advisories)|High-impact alerts, active threat campaigns, mitigations, and joint advisories.|
|NIST National Vulnerability Database|[NVD](https://nvd.nist.gov/)|CVE details, severity data, affected products, and vulnerability references.|
|CVE Program|[CVE.org](https://www.cve.org/)|Canonical CVE identifiers and vulnerability records.|
|FIRST EPSS|[Exploit Prediction Scoring System](https://www.first.org/epss/)|Prioritizing vulnerabilities by likelihood of exploitation, not just severity score.|
|MITRE ATT&CK|[MITRE ATT&CK](https://attack.mitre.org/)|Understanding attacker tactics, techniques, and procedures. Useful for detection and tabletop planning.|
|FBI Internet Crime Complaint Center|[IC3 Annual Reports](https://www.ic3.gov/AnnualReport/Reports)|Business email compromise, fraud, ransomware, phishing, and reported loss trends.|
|FBI Cyber|[FBI Cyber](https://www.fbi.gov/investigate/cyber)|U.S. cybercrime and threat guidance, especially for reporting and law enforcement context.|

CISA’s KEV catalog is useful because it focuses on vulnerabilities known to be exploited in the wild, while CISA advisories provide timely information on high-impact threats and mitigations. NIST NVD and CVE.org provide vulnerability reference data, while EPSS helps prioritize which vulnerabilities are more likely to be exploited. MITRE ATT&CK is useful for translating threat reporting into attacker behavior. ([CISA](https://www.cisa.gov/known-exploited-vulnerabilities-catalog "Known Exploited Vulnerabilities Catalog"))

## Government and National Cybersecurity Authorities

These are high-trust sources. Use the ones most relevant to the company’s geography, customers, and regulatory environment.

| Source                             | Link                                                                                                   | Use It For                                                                            |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- |
| CISA                               | [CISA](https://www.cisa.gov/)                                                                          | U.S. cyber alerts, guidance, KEV, ransomware resources, and vulnerability advisories. |
| UK National Cyber Security Centre  | [NCSC Reports and Advisories](https://www.ncsc.gov.uk/section/keep-up-to-date/reports-advisories)      | Practical cyber advisories, threat reporting, and executive-friendly guidance.        |
| NCSC Early Warning                 | [NCSC Early Warning](https://www.ncsc.gov.uk/section/active-cyber-defence/early-warning)               | Free early warning service for eligible UK organizations.                             |
| Australian Cyber Security Centre   | [ACSC Alerts and Advisories](https://www.cyber.gov.au/about-us/view-all-content/alerts-and-advisories) | Alerts, advisories, and practical threat guidance for Australian organizations.       |
| Canadian Centre for Cyber Security | [Canadian Cyber Centre Alerts](https://www.cyber.gc.ca/en/alerts-advisories)                           | Canadian cyber alerts, advisories, and threat guidance.                               |
| ENISA                              | [ENISA Threat Landscape](https://www.enisa.europa.eu/topics/cyber-threats/threat-landscape)            | European threat landscape reporting and sector-level cyber risk context.              |

NCSC, ACSC, the Canadian Cyber Centre, and ENISA are useful cross-checks against U.S.-centric CISA reporting, especially if the SME operates internationally or serves customers in those regions. ([National Cyber Security Centre](https://www.ncsc.gov.uk/section/keep-up-to-date/reports-advisories "Reports & advisories"))

## Vendor Security Advisory Sources

This is where many SMEs fail. The company should not just monitor general cybersecurity news. It must monitor the vendors it actually uses.

|Vendor / Platform|Link|Use It For|
|---|---|---|
|Microsoft Security Response Center|[MSRC Security Update Guide](https://msrc.microsoft.com/update-guide)|Windows, Microsoft 365, Exchange, Azure, SharePoint, Defender, and other Microsoft security updates.|
|Microsoft Digital Defense Report|[Microsoft Digital Defense Report](https://www.microsoft.com/en-us/security/security-insider/threat-landscape/microsoft-digital-defense-report-2025)|Annual Microsoft threat landscape and identity/security trends.|
|Google Cloud Security Bulletins|[Google Cloud Security Bulletins](https://cloud.google.com/support/bulletins)|Google Cloud product vulnerabilities and security bulletins.|
|Google Workspace Updates|[Google Workspace Updates Blog](https://workspaceupdates.googleblog.com/)|Google Workspace product, admin, and security-relevant updates.|
|Apple Security Releases|[Apple Security Releases](https://support.apple.com/en-us/100100)|macOS, iOS, iPadOS, Safari, and Apple platform security updates.|
|Cisco Security Advisories|[Cisco Security Advisories](https://sec.cloudapps.cisco.com/security/center/publicationListing.x)|Cisco network, firewall, VPN, collaboration, and infrastructure vulnerabilities.|
|Fortinet PSIRT|[Fortinet PSIRT Advisories](https://www.fortiguard.com/psirt)|Fortinet firewall, VPN, FortiGate, FortiOS, and Fortinet product vulnerabilities.|
|Palo Alto Networks Security Advisories|[Palo Alto Security Advisories](https://security.paloaltonetworks.com/)|PAN-OS, GlobalProtect, Prisma, Cortex, and Palo Alto product advisories.|
|GitHub Advisory Database|[GitHub Advisory Database](https://github.com/advisories)|Open-source package vulnerabilities affecting npm, pip, Maven, Go, NuGet, RubyGems, and other ecosystems.|
|OpenSSF|[OpenSSF](https://openssf.org/)|Open-source software supply-chain security guidance and tools.|

If the company uses Microsoft 365, Google Workspace, Fortinet, Cisco, Palo Alto, WordPress, GitHub, Atlassian, VMware, cloud platforms, or any major SaaS product, the company should subscribe to that vendor’s security advisory feed. Vendor advisories are often the fastest source for product-specific remediation details. Google Cloud, GitHub, Fortinet, Cisco, and Palo Alto all maintain dedicated advisory or bulletin pages for this purpose. ([Google Cloud](https://cloud.google.com/support/bulletins "Security Bulletins  |  Cloud Customer Care  |  Google Cloud Documentation"))

## Threat Research and Annual Reports

These sources help leadership understand the broader environment. They should not replace urgent advisories, but they are useful for quarterly or annual threat reviews.

| Source                                    | Link                                                                                        | Use It For                                                                                                                     |
| ----------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Mandiant M-Trends                         | [Mandiant M-Trends](https://cloud.google.com/security/resources/m-trends)                   | Frontline incident response trends, initial access vectors, ransomware, cloud compromise, dwell time, and attacker techniques. |
| Google Threat Intelligence Blog           | [Google Threat Intelligence](https://cloud.google.com/blog/topics/threat-intelligence)      | Current attacker campaigns, vulnerability exploitation, malware, cloud threats, and AI-related threat research.                |
| Unit 42 Research                          | [Unit 42](https://unit42.paloaltonetworks.com/)                                             | Incident response findings, ransomware, cloud threats, attacker behavior, and practical defensive recommendations.             |
| CrowdStrike Global Threat Report          | [CrowdStrike Global Threat Report](https://www.crowdstrike.com/en-us/global-threat-report/) | Adversary trends, malware-free attacks, identity abuse, nation-state activity, and eCrime trends.                              |
| Verizon Data Breach Investigations Report | [Verizon DBIR](https://www.verizon.com/business/resources/reports/dbir/)                    | Breach patterns, attack vectors, human factors, ransomware, vulnerability exploitation, and industry trends.                   |
| Microsoft Security Insider                | [Microsoft Security Insider](https://www.microsoft.com/en-us/security/security-insider/)    | Microsoft threat intelligence, identity trends, ransomware, fraud, and security guidance.                                      |
| Google Project Zero                       | [Google Project Zero](https://projectzero.google/)                                          | Zero-day research, root-cause analysis, and vulnerability exploitation trends.                                                 |

Mandiant, Unit 42, CrowdStrike, Microsoft, Google Threat Intelligence, and Verizon are useful because they translate large volumes of real incident data into executive-level trends. For an SME, these should feed the monthly or quarterly threat environment snapshot, not become a daily reading burden.

## Free and Practical Open Threat Intelligence Sources

These are more technical. They are useful for IT, MSPs, security providers, and more mature SMEs.

|Source|Link|Use It For|
|---|---|---|
|SANS Internet Storm Center|[SANS ISC](https://isc.sans.edu/)|Daily handler diaries, attack trends, internet scanning activity, and practical technical observations.|
|SANS ISC Threat Feeds|[SANS ISC Threat Feeds](https://isc.sans.edu/data/threatfeed.html)|Actionable threat feed data for defenders.|
|Shadowserver Foundation|[Shadowserver](https://www.shadowserver.org/)|Internet-scale threat reporting, exposed services, botnets, malware, and vulnerable systems.|
|abuse.ch|[abuse.ch](https://abuse.ch/)|Malware, botnet, malicious URL, SSL, and threat feed projects.|
|Feodo Tracker|[Feodo Tracker](https://feodotracker.abuse.ch/)|Botnet command-and-control tracking and blocklists.|
|OpenPhish|[OpenPhish](https://openphish.com/)|Active phishing threat intelligence.|
|AlienVault Open Threat Exchange|[AlienVault OTX](https://otx.alienvault.com/)|Community-generated threat indicators and threat intelligence pulses.|
|VirusTotal Blog|[VirusTotal Blog](https://blog.virustotal.com/)|Malware, phishing, file, URL, and detection research.|
|Google Threat Intelligence Documentation|[Google Threat Intelligence Docs](https://gtidocs.virustotal.com/)|Guidance for using Google Threat Intelligence and VirusTotal tooling.|

A small company should not blindly dump every feed into tools without tuning, because that creates noise. These sources are best used by the MSP, security provider, or internal IT owner to confirm whether specific URLs, IPs, hashes, domains, or campaigns are relevant to the company. SANS ISC, Shadowserver, abuse.ch, OpenPhish, AlienVault OTX, and VirusTotal are all useful practical sources for technical threat data and campaign research. ([SANS Internet Storm Center](https://isc.sans.edu/ "SANS.edu Internet Storm Center - SANS Internet Storm Center"))

## Sector-Specific Intelligence Sources

If the SME operates in a regulated or high-risk sector, it should consider joining or monitoring a sector-specific information sharing group.

|Source|Link|Use It For|
|---|---|---|
|National Council of ISACs|[National Council of ISACs](https://www.nationalisacs.org/)|Finding the relevant sector ISAC for the company’s industry.|
|FS-ISAC|[FS-ISAC](https://www.fsisac.com/)|Financial services threat intelligence and cyber resilience information sharing.|
|Health-ISAC|[Health-ISAC](https://health-isac.org/)|Healthcare sector cyber and physical security threat intelligence.|
|Health-ISAC Threat Intelligence|[Health-ISAC Threat Intelligence](https://health-isac.org/category/h-isac-blog/threat-intelligence-h-isac-blog/)|Healthcare-focused threat updates and analysis.|

ISACs are valuable when the company’s risks are sector-specific, such as finance, healthcare, energy, retail, manufacturing, transportation, or education. The National Council of ISACs describes ISACs as member-driven organizations that deliver threat and mitigation information to asset owners and operators. ([natlcouncilofisacs](https://www.nationalisacs.org/ "National Council of ISACs"))

## Recommended Review Cadence

For most SMEs, use this rhythm.

Daily or near-real-time: CISA KEV, vendor advisories for critical systems, MSP alerts, Microsoft or Google admin alerts.

Weekly: CISA advisories, NCSC/ACSC/Cyber Centre advisories if relevant, SANS ISC, vendor security updates.

Monthly: Mandiant, Unit 42, CrowdStrike, Microsoft, Google Threat Intelligence, Verizon DBIR updates or major research posts.

Quarterly: Executive threat environment briefing, technology watchlist review, source list review, and open questions to carry into the risk assessment.

## Practical Minimum for a Small Company

A very small SME does not need 40 feeds. Start with this core set:

[CISA KEV Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog)  
[CISA Cybersecurity Advisories](https://www.cisa.gov/news-events/cybersecurity-advisories)  
[NVD](https://nvd.nist.gov/)  
[FIRST EPSS](https://www.first.org/epss/)  
[MITRE ATT&CK](https://attack.mitre.org/)  
[MSRC Security Update Guide](https://msrc.microsoft.com/update-guide)  
[Google Workspace Updates](https://workspaceupdates.googleblog.com/) or the equivalent source for the company’s main productivity suite  
The security advisory pages for the company’s firewall, VPN, backup, endpoint protection, and major SaaS vendors  
[FBI IC3 Annual Reports](https://www.ic3.gov/AnnualReport/Reports)  
[Mandiant M-Trends](https://cloud.google.com/security/resources/m-trends)  
[SANS Internet Storm Center](https://isc.sans.edu/)

The blunt rule: a company should only monitor sources it can act on. A threat feed that nobody reviews, understands, or connects to company technology is theater.

### Cybersecurity News

News sources are a separate category from the formal threat-intelligence sources. They are useful for **situational awareness**, but they should not replace CISA, vendor advisories, NVD, or direct security bulletins.

| Cybersecurity News Source            | Link                                                            | Best Use in This Section                                                                                                                                                             |
| ------------------------------------ | --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BleepingComputer                     | [BleepingComputer](https://www.bleepingcomputer.com/)           | Fast practical coverage of breaches, ransomware, malware, exploited vulnerabilities, Windows/Microsoft issues, and active cybercrime campaigns. Useful for weekly threat awareness.  |
| The Hacker News                      | [The Hacker News](https://thehackernews.com/)                   | Broad daily cybersecurity news, vulnerability coverage, threat actor updates, cloud/security product issues, and attack campaign summaries. Useful for quick scanning.               |
| Dark Reading                         | [Dark Reading](https://www.darkreading.com/)                    | Enterprise security news, cyber risk, vulnerability trends, threat intelligence, application security, and security operations analysis. Good for executive and IT/security readers. |
| The Register — Security              | [The Register Security](https://www.theregister.com/security/)  | Sharp technology and security reporting, including breaches, cybercrime, software vulnerabilities, vendor failures, patching, and regulatory issues.                                 |
| SecurityWeek                         | [SecurityWeek](https://www.securityweek.com/)                   | Cybersecurity news and analysis for security professionals, including vulnerabilities, threat actors, ransomware, cyber policy, funding, and enterprise security trends.             |
| KrebsOnSecurity                      | [KrebsOnSecurity](https://krebsonsecurity.com/)                 | Investigative security journalism, cybercrime ecosystems, fraud, identity abuse, payment crime, botnets, and breach reporting. Strong for understanding attacker economics.          |
| The Record from Recorded Future News | [The Record](https://therecord.media/)                          | Cyber policy, ransomware, nation-state activity, cybercrime, law enforcement actions, critical infrastructure attacks, and geopolitical cyber developments.                          |
| CSO Online                           | [CSO Online](https://www.csoonline.com/)                        | Security leadership, risk management, incident response, resilience, cyber governance, and enterprise security decision-making. Useful for management-facing context.                |
| Infosecurity Magazine                | [Infosecurity Magazine](https://www.infosecurity-magazine.com/) | Security news, trends, research summaries, executive commentary, and industry developments. Useful for periodic threat-environment scanning.                                         |
| SC Media                             | [SC Media](https://www.scworld.com/)                            | Cybersecurity news, analysis, research, webinars, and practitioner-oriented updates. Useful for security operations, risk, and sector-specific stories.                              |

They are helpful because they provide ongoing coverage of breach activity, ransomware, cybercrime, exploited vulnerabilities, security operations, and executive-level cyber risk.

Use these sites to stay aware of what is happening, but use **official advisories and vendor bulletins** to decide whether a specific system needs action. News tells you what is happening; advisories tell you what to fix.