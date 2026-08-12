

### Purpose

Use this checklist when deploying or reviewing endpoints, servers, cloud systems, SaaS platforms, network devices, and other important technology.

The objective is to reduce unnecessary features, weak defaults, excessive access, and insecure configurations.

### Identity and Access

- [ ]  Default accounts reviewed.
- [ ]  Default passwords changed.
- [ ]  MFA enabled where required.
- [ ]  Administrator access limited.
- [ ]  Separate administrator accounts used where practical.
- [ ]  Unnecessary accounts removed or disabled.
- [ ]  Service accounts documented.
- [ ]  Vendor access restricted.
- [ ]  Least privilege applied.

### System Configuration

- [ ]  Operating system supported.
- [ ]  Security updates current.
- [ ]  Unnecessary services disabled.
- [ ]  Unused ports or protocols disabled.
- [ ]  Unnecessary software removed.
- [ ]  Host firewall enabled where appropriate.
- [ ]  Secure time synchronization configured.
- [ ]  Configuration owner identified.

### Endpoint Security

- [ ]  Endpoint protection enabled.
- [ ]  Disk encryption enabled where appropriate.
- [ ]  Screen locking configured.
- [ ]  Local administrator access restricted.
- [ ]  Device inventory updated.
- [ ]  Security logging enabled.
- [ ]  Remote access restricted.

### Network and Remote Access

- [ ]  Administrative interfaces are not unnecessarily internet-facing.
- [ ]  RDP or SSH exposure reviewed.
- [ ]  Firewall rules reviewed.
- [ ]  VPN or zero-trust controls used where appropriate.
- [ ]  Default network device credentials changed.
- [ ]  Old or unused firewall rules removed.
- [ ]  Remote support tools approved and controlled.

### Cloud and SaaS

- [ ]  MFA enabled for administrators.
- [ ]  Administrator roles reviewed.
- [ ]  External sharing reviewed.
- [ ]  Public links restricted.
- [ ]  Audit logging enabled where available.
- [ ]  OAuth and third-party integrations reviewed.
- [ ]  Legacy authentication disabled where possible.
- [ ]  Data retention and recovery settings reviewed.
- [ ]  Unused accounts and applications removed.

### Email

- [ ]  MFA enabled.
- [ ]  Administrator accounts protected.
- [ ]  External forwarding reviewed.
- [ ]  Mailbox forwarding rules monitored where practical.
- [ ]  Spam and phishing protection enabled.
- [ ]  SPF configured.
- [ ]  DKIM configured where applicable.
- [ ]  DMARC configured and reviewed.
- [ ]  Legacy authentication restricted where possible.

### Websites and Internet-Facing Systems

- [ ]  Software and plugins supported.
- [ ]  Updates applied.
- [ ]  Administrator access protected with MFA where possible.
- [ ]  Unnecessary admin interfaces restricted.
- [ ]  TLS configuration reviewed.
- [ ]  Security headers reviewed.
- [ ]  Backups available.
- [ ]  Logging enabled.
- [ ]  Default credentials removed.

### Backups

- [ ]  Required systems included in backup.
- [ ]  Backup failures generate alerts.
- [ ]  Backup access restricted.
- [ ]  Backup administrators use MFA where possible.
- [ ]  Backup retention configured.
- [ ]  Protection against deletion or ransomware considered.
- [ ]  Restore testing performed.

### Logging and Monitoring

- [ ]  Important authentication logs enabled.
- [ ]  Administrator activity logged where practical.
- [ ]  Endpoint alerts monitored.
- [ ]  Backup failure alerts monitored.
- [ ]  Security alerts go to an accountable owner.
- [ ]  Log retention appropriate to the system.
- [ ]  Time settings support accurate event correlation.

### Verification

System: ____________________

System owner: ____________________

Reviewed by: ____________________

Review date: ____________________

Significant gaps: ____________________

Improvement owner: ____________________

Due date: ____________________

Evidence location: ____________________

Next review date: ____________________

### Practical Rule

Secure configuration means removing what is not needed, protecting what remains, and verifying that important safeguards are actually enabled.