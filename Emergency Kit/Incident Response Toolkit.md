---
icon: triangle-right
order: 10
---
## Appendix: Open Source Leaning Incident Response Toolkit

This appendix gathers useful free, open-source, publicly available, and affordable tools that can support incident response, evidence collection, investigation, containment, recovery, documentation, and training.

The company does not need every tool listed here. Tool selection should match the company’s size, technical ability, systems, risk level, and available support.

During a serious incident, tools should be used carefully. Avoid installing new tools directly onto compromised systems unless a qualified technical responder approves the approach. In many cases, the safest first step is to preserve evidence, contain the obvious damage, and escalate to qualified support.

## 1. Incident Tracking, Case Management, and Action Tracking

|Tool|Link|Type|Best Use|
|---|---|---|---|
|TheHive|[TheHive](https://strangebee.com/thehive/)|Commercial / security case management|Incident case management, triage, collaboration, investigation records, reporting|
|Zammad|[Zammad](https://zammad.org/)|Open-source / commercial|Security tickets, employee reports, incident follow-up, support workflow|
|osTicket|[osTicket](https://osticket.com/)|Open-source / commercial|Simple helpdesk-style incident intake and action tracking|
|GLPI|[GLPI](https://glpi-project.org/)|Open-source / commercial|IT service desk, assets, tickets, incident records, follow-up tasks|
|Jira Service Management|[Jira Service Management](https://www.atlassian.com/software/jira/service-management)|Commercial / free tier|Incident workflows, approvals, tasks, and improvement tracking|
|OpenProject|[OpenProject](https://www.openproject.org/)|Open-source / commercial|Improvement project tracking and leadership-visible remediation work|
|Kanboard|[Kanboard](https://kanboard.org/)|Open-source|Lightweight task board for incident and improvement actions|

## 2. Secure Documentation and Evidence Storage

|Tool|Link|Type|Best Use|
|---|---|---|---|
|CryptPad|[CryptPad](https://cryptpad.org/)|Open-source / free options|Secure notes, incident timelines, collaborative documentation|
|Nextcloud|[Nextcloud](https://nextcloud.com/)|Open-source / commercial|Controlled storage for evidence, reports, screenshots, and response records|
|BookStack|[BookStack](https://www.bookstackapp.com/)|Open-source|Internal incident response handbook, procedures, and evidence references|
|Wiki.js|[Wiki.js](https://js.wiki/)|Open-source|Internal knowledge base for procedures, contacts, and playbooks|
|Google Drive|[Google Drive](https://www.google.com/drive/)|Free / Workspace|Evidence storage and controlled sharing for Google-based SMEs|
|SharePoint|[SharePoint](https://www.microsoft.com/microsoft-365/sharepoint/collaboration)|Microsoft 365|Evidence storage and controlled sharing for Microsoft-based SMEs|

## 3. Endpoint Investigation and Response

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Velociraptor|[Velociraptor](https://docs.velociraptor.app/)|Open-source|Endpoint visibility, forensic collection, hunting, remote investigation|
|osquery|[osquery](https://www.osquery.io/)|Open-source|Querying endpoint state, installed software, processes, users, and system details|
|Fleet|[Fleet](https://fleetdm.com/)|Open-source / commercial|Managing osquery at scale across endpoints|
|Sysmon|[Sysmon](https://learn.microsoft.com/sysinternals/downloads/sysmon)|Free Microsoft tool|Detailed Windows endpoint logging for process, network, and file activity|
|Wazuh Agent|[Wazuh](https://wazuh.com/)|Open-source|Endpoint monitoring, detection, vulnerability visibility, file integrity monitoring|
|Microsoft Defender for Business|[Microsoft Defender for Business](https://www.microsoft.com/security/business/endpoint-security/microsoft-defender-business)|Affordable commercial|Endpoint protection and response for Microsoft-based SMEs|

## 4. Logging, SIEM, and Detection

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Wazuh|[Wazuh](https://wazuh.com/)|Open-source|SIEM, XDR, endpoint monitoring, alerting, compliance visibility|
|Security Onion|[Security Onion](https://securityonionsolutions.com/software/)|Free / open platform|Threat hunting, network security monitoring, log management|
|Graylog Open|[Graylog Open](https://graylog.org/products/source-available/)|Source-available / commercial|Centralized log management and search|
|OpenSearch|[OpenSearch](https://opensearch.org/)|Open-source|Log storage, search, dashboards, and security analytics|
|Grafana Loki|[Grafana Loki](https://grafana.com/oss/loki/)|Open-source / commercial|Log aggregation and dashboarding|
|Sigma|[Sigma](https://sigmahq.io/)|Open-source rule format|Detection rule writing and translation across SIEM platforms|
|ElastAlert 2|[ElastAlert 2](https://github.com/jertel/elastalert2)|Open-source|Alerting from Elasticsearch or OpenSearch-style data|
|Microsoft Sentinel|[Microsoft Sentinel](https://azure.microsoft.com/products/microsoft-sentinel)|Commercial / cloud-native|Cloud SIEM and security analytics for Microsoft-heavy environments|

## 5. Network Monitoring and Containment

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Suricata|[Suricata](https://suricata.io/)|Open-source|Network intrusion detection and prevention|
|Zeek|[Zeek](https://zeek.org/)|Open-source|Network visibility, protocol analysis, and security monitoring|
|Nmap|[Nmap](https://nmap.org/)|Open-source|Network discovery, exposed services, and validation checks|
|OPNsense|[OPNsense](https://opnsense.org/)|Open-source / commercial support|Firewalling, segmentation, VPN, emergency network controls|
|pfSense CE|[pfSense Community Edition](https://www.pfsense.org/)|Free community edition|Firewalling, routing, VPN, and network containment|
|CrowdSec|[CrowdSec](https://www.crowdsec.net/)|Open-source / commercial|Community-powered intrusion prevention and abusive IP blocking|
|Fail2ban|[Fail2ban](https://github.com/fail2ban/fail2ban)|Open-source|Brute-force protection for exposed services|
|Wireshark|[Wireshark](https://www.wireshark.org/)|Open-source|Packet capture review and network troubleshooting|
|tcpdump|[tcpdump](https://www.tcpdump.org/)|Open-source|Command-line packet capture and network evidence collection|

## 6. Digital Forensics and Timeline Analysis

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Autopsy|[Autopsy](https://www.autopsy.com/)|Open-source|Disk forensics, file recovery, and investigation of affected devices|
|The Sleuth Kit|[The Sleuth Kit](https://www.sleuthkit.org/)|Open-source|Low-level disk and file system forensic analysis|
|Volatility 3|[Volatility 3](https://volatilityfoundation.org/)|Open-source|Memory forensics and volatile evidence analysis|
|Timesketch|[Timesketch](https://timesketch.org/)|Open-source|Collaborative forensic timeline analysis|
|Plaso|[Plaso](https://plaso.readthedocs.io/)|Open-source|Log and artifact timeline creation|
|Hayabusa|[Hayabusa](https://github.com/Yamato-Security/hayabusa)|Open-source|Windows event log threat hunting and timeline analysis|
|Chainsaw|[Chainsaw](https://github.com/WithSecureLabs/chainsaw)|Open-source|Windows event log searching, Sigma matching, and forensic review|
|DFIR ORC|[DFIR ORC](https://dfir-orc.github.io/)|Open-source|Forensic collection on Windows systems|
|KAPE|[KAPE](https://www.kroll.com/en/services/cyber-risk/incident-response-litigation-support/kape)|Free / commercial support|Targeted forensic artifact collection and processing|

## 7. Malware, Indicators, and Suspicious Link Review

|Tool|Link|Type|Best Use|
|---|---|---|---|
|CyberChef|[CyberChef](https://gchq.github.io/CyberChef/)|Open-source|Decoding, deobfuscation, data transformation, artifact review|
|VirusTotal|[VirusTotal](https://www.virustotal.com/)|Free / commercial|Checking suspicious files, hashes, domains, URLs, and IPs|
|urlscan.io|[urlscan.io](https://urlscan.io/)|Free / commercial|Reviewing suspicious URLs and phishing pages|
|MISP|[MISP](https://www.misp-project.org/)|Open-source|Threat intelligence sharing and indicator management|
|YARA|[YARA](https://virustotal.github.io/yara/)|Open-source|Malware pattern matching and file classification|
|MalwareBazaar|[MalwareBazaar](https://bazaar.abuse.ch/)|Free public resource|Malware sample and hash intelligence|
|AbuseIPDB|[AbuseIPDB](https://www.abuseipdb.com/)|Free / commercial|IP reputation and abuse reporting|
|GreyNoise Community|[GreyNoise Community](https://viz.greynoise.io/)|Free / commercial|Internet noise and IP context|

## 8. Email, Phishing, and Business Email Compromise Support

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Microsoft Report Message / Report Phishing|[Microsoft Report Messages](https://learn.microsoft.com/defender-office-365/submissions-outlook-report-messages)|Microsoft 365|Employee phishing reporting in Outlook|
|Gmail Report Phishing|[Gmail Report Phishing](https://support.google.com/mail/answer/8253)|Gmail / Google Workspace|Employee phishing reporting in Gmail|
|MXToolbox|[MXToolbox](https://mxtoolbox.com/)|Free / commercial|Mail server, DNS, SPF, DKIM, DMARC, and blacklist checks|
|DMARCian|[DMARCian](https://dmarcian.com/)|Commercial / free tools|DMARC reporting, email authentication monitoring|
|EasyDMARC|[EasyDMARC](https://easydmarc.com/)|Commercial / free tools|DMARC, SPF, DKIM, and email security monitoring|
|Gophish|[Gophish](https://getgophish.com/)|Open-source|Phishing simulations and reporting practice|
|CanIPhish|[CanIPhish](https://caniphish.com/)|Free tier / commercial|Phishing simulation and awareness campaigns|
|Google Phishing Quiz|[Google Phishing Quiz](https://phishingquiz.withgoogle.com/)|Free exercise|Phishing recognition practice|

## 9. Cloud, SaaS, and Configuration Review

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Prowler|[Prowler](https://prowler.com/)|Open-source / commercial|Cloud security posture checks, especially AWS and multi-cloud use cases|
|ScoutSuite|[ScoutSuite](https://github.com/nccgroup/ScoutSuite)|Open-source|Cloud security auditing across major cloud providers|
|Steampipe|[Steampipe](https://steampipe.io/)|Open-source / commercial|Querying cloud, SaaS, and infrastructure configuration data|
|Trivy|[Trivy](https://trivy.dev/)|Open-source|Vulnerability, container, IaC, dependency, and secret scanning|
|Checkov|[Checkov](https://www.checkov.io/)|Open-source / commercial|Infrastructure-as-code and cloud configuration scanning|
|Gitleaks|[Gitleaks](https://gitleaks.io/)|Open-source|Secret scanning in repositories and files|
|TruffleHog|[TruffleHog](https://trufflesecurity.com/trufflehog)|Open-source / commercial|Secret scanning across repositories, files, and systems|
|Microsoft Purview Audit|[Microsoft Purview Audit](https://learn.microsoft.com/purview/audit-solutions-overview)|Microsoft 365|Audit logging and investigation support in Microsoft environments|
|Google Workspace Admin Audit Logs|[Google Workspace Audit Logs](https://support.google.com/a/answer/4579696)|Google Workspace|Admin, login, Drive, and user activity review|

## 10. Vulnerability, Exposure, and Website Checks

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Greenbone Community Edition|[Greenbone Community Edition](https://greenbone.github.io/docs/latest/)|Open-source|Vulnerability scanning|
|Nuclei|[Nuclei](https://nuclei.projectdiscovery.io/)|Open-source|Template-based vulnerability and exposure scanning|
|WPScan|[WPScan](https://wpscan.com/)|Free / commercial|WordPress vulnerability checks|
|Security Headers|[Security Headers](https://securityheaders.com/)|Free public tool|HTTP security header checks|
|SSL Labs Server Test|[SSL Labs Server Test](https://www.ssllabs.com/ssltest/)|Free public tool|TLS and certificate configuration review|
|Internet.nl|[Internet.nl](https://internet.nl/)|Free public tool|Website, email, TLS, DNSSEC, and IPv6 checks|
|Shodan|[Shodan](https://www.shodan.io/)|Free / commercial|Internet-facing asset and exposure discovery|
|Censys|[Censys](https://censys.com/)|Free / commercial|Internet exposure and certificate search|
|Hardenize|[Hardenize](https://www.hardenize.com/)|Free / commercial|Website, email, and TLS configuration review|
|SecurityTrails|[SecurityTrails](https://securitytrails.com/)|Free / commercial|DNS, domain, and internet asset discovery|

## 11. Backup, Recovery, and Restore Validation

|Tool|Link|Type|Best Use|
|---|---|---|---|
|restic|[restic](https://restic.net/)|Open-source|Encrypted backups and restore testing|
|BorgBackup|[BorgBackup](https://www.borgbackup.org/)|Open-source|Deduplicated encrypted backups|
|Kopia|[Kopia](https://kopia.io/)|Open-source|Fast encrypted backups and snapshots|
|Proxmox Backup Server|[Proxmox Backup Server](https://www.proxmox.com/en/proxmox-backup-server)|Open-source / commercial support|VM, container, and server backup support|
|Veeam Community Edition|[Veeam Community Edition](https://www.veeam.com/products/free/backup-recovery.html)|Free edition / commercial|Backup and recovery for small environments and labs|
|UrBackup|[UrBackup](https://www.urbackup.org/)|Open-source|Client-server backup for files and images|
|Duplicati|[Duplicati](https://duplicati.com/)|Open-source|Encrypted backups to local and cloud storage|
|Rclone|[Rclone](https://rclone.org/)|Open-source|File synchronization and backup movement across cloud/storage providers|

## 12. Monitoring, Status, and Notifications

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Uptime Kuma|[Uptime Kuma](https://uptime.kuma.pet/)|Open-source|Service uptime monitoring and status checks|
|Healthchecks.io|[Healthchecks.io](https://healthchecks.io/)|Open-source / hosted service|Backup job, cron job, and scheduled task monitoring|
|Zabbix|[Zabbix](https://www.zabbix.com/)|Open-source / commercial support|Infrastructure, server, service, and network monitoring|
|LibreNMS|[LibreNMS](https://www.librenms.org/)|Open-source|Network monitoring and device visibility|
|Prometheus|[Prometheus](https://prometheus.io/)|Open-source|Metrics collection and alerting|
|Grafana|[Grafana](https://grafana.com/oss/grafana/)|Open-source / commercial|Dashboards for monitoring and reporting|
|ntfy|[ntfy](https://ntfy.sh/)|Open-source / hosted|Lightweight push notifications|
|Gotify|[Gotify](https://gotify.net/)|Open-source|Self-hosted push notifications|

## 13. Secure Remote Access and Emergency Access Control

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Cloudflare Zero Trust|[Cloudflare Zero Trust](https://www.cloudflare.com/zero-trust/)|Free tier / commercial|Secure access, application access control, emergency access tightening|
|Tailscale|[Tailscale](https://tailscale.com/)|Free tier / commercial|Simple mesh VPN and private access control|
|NetBird|[NetBird](https://netbird.io/)|Open-source / commercial|WireGuard-based secure access and device connectivity|
|WireGuard|[WireGuard](https://www.wireguard.com/)|Open-source|Lightweight VPN technology|
|OpenVPN Community Edition|[OpenVPN Community Edition](https://openvpn.net/community/)|Open-source|VPN access for remote connectivity|

## 14. Internal Communication and Emergency Coordination

|Tool|Link|Type|Best Use|
|---|---|---|---|
|Mattermost|[Mattermost](https://mattermost.com/)|Open-source / commercial|Internal incident coordination and security channels|
|Zulip|[Zulip](https://zulip.com/)|Open-source / commercial|Structured chat for security reporting and incident discussions|
|Rocket.Chat|[Rocket.Chat](https://www.rocket.chat/)|Open-source / commercial|Internal chat and emergency communication|
|Jitsi Meet|[Jitsi Meet](https://jitsi.org/jitsi-meet/)|Open-source|Emergency video calls and incident meetings|
|Signal|[Signal](https://signal.org/)|Free public app|Out-of-band emergency communication where appropriate|
|Statusfy|[Statusfy](https://statusfy.co/)|Open-source|Status pages for service disruption communication|
|Cachet|[Cachet](https://cachethq.io/)|Open-source|Status page and incident status communication|

## 15. Training, Awareness, and Simulations

| Tool or Resource                     | Link                                                                                                                         | Type                       | Best Use                                   |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------- | ------------------------------------------ |
| CISA Secure Our World                | [CISA Secure Our World](https://www.cisa.gov/secure-our-world)                                                               | Free public resource       | Employee awareness materials               |
| FTC Cybersecurity for Small Business | [FTC Cybersecurity for Small Business](https://www.ftc.gov/business-guidance/small-businesses/cybersecurity)                 | Free public resource       | Small-business cybersecurity education     |
| NCSC Top Tips for Staff              | [NCSC Top Tips for Staff](https://www.ncsc.gov.uk/information/top-tips-for-staff)                                            | Free public training       | Basic staff cybersecurity training         |
| SANS OUCH!                           | [SANS OUCH!](https://www.sans.org/newsletters/ouch)                                                                          | Free newsletter            | Monthly awareness reminders                |
| NCSC Exercise in a Box               | [NCSC Exercise in a Box](https://www.ncsc.gov.uk/section/exercise-in-a-box/overview)                                         | Free exercise resource     | Tabletop and micro exercises               |
| CISA Tabletop Exercise Package       | [CISA Tabletop Exercise Package](https://www.cisa.gov/resources-tools/training/cisa-tabletop-exercise-package-documentation) | Free exercise resource     | Tabletop exercise planning                 |
| H5P                                  | [H5P](https://h5p.org/)                                                                                                      | Open-source / free options | Interactive quizzes and training scenarios |
| TalentLMS                            | [TalentLMS](https://www.talentlms.com/)                                                                                      | Affordable commercial      | Small-team training delivery and tracking  |
| Google Forms                         | [Google Forms](https://www.google.com/forms/about/)                                                                          | Free / Workspace           | Training confirmations and quizzes         |
| Microsoft Forms                      | [Microsoft Forms](https://www.microsoft.com/microsoft-365/online-surveys-polls-quizzes)                                      | Microsoft 365              | Training confirmations and quizzes         |

## Suggested Minimal Toolkit for SMEs

A smaller company does not need everything in this appendix.

**A practical starting toolkit may include:**

- **Ticketing or tracking:** Zammad, osTicket, GLPI, Jira Service Management, or a controlled spreadsheet.

- **Documentation and evidence:** Nextcloud, SharePoint, Google Drive, BookStack, Wiki.js, or CryptPad.

- **Endpoint visibility:** Wazuh, Microsoft Defender for Business, osquery, Fleet, or Velociraptor with qualified support.

- **Logging and detection:** Wazuh, Security Onion, Graylog, OpenSearch, or Microsoft Sentinel.

- **Network checks:** Nmap, Security Headers, SSL Labs, Internet.nl, Shodan, and Censys.

- **Phishing and suspicious link review:** Microsoft or Gmail report tools, Gophish, VirusTotal, urlscan.io, and MXToolbox.

- **Backups and recovery:** restic, BorgBackup, Kopia, Proxmox Backup Server, Veeam Community Edition, or an existing managed backup platform.

- **Monitoring and alerts:** Uptime Kuma, Healthchecks.io, Zabbix, Grafana, ntfy, or Gotify.

- **Training and exercises:** CISA Secure Our World, NCSC Exercise in a Box, SANS OUCH!, Moodle, H5P, Google Forms, or Microsoft Forms.

## Tool Selection Guidance

Use the tools the company can actually maintain.

A simple, well-maintained setup is better than a complex toolkit nobody watches.

**Before adopting a tool, ask:**

- Who owns it?
- Who knows how to use it?
- Where will alerts go?
- How will evidence be stored?
- How often will it be reviewed?
- Will it help during an incident?
- What risk does it reduce?
- Does it create new maintenance work?
- Is support available if needed?
