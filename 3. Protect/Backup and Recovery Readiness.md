---
icon: triangle-right
order: 80
---
### Goals

Backups are the company’s last line of defense when systems fail, data is deleted, ransomware spreads, or a cloud account is compromised.

The goal of this section is to make sure the company has backups that are complete, protected, monitored, and tested.

A backup that has never been restored is only an assumption. A backup that attackers can delete is not safe. A backup that no one monitors may already be failing.

This section covers the backup regime and recovery readiness. The actual live recovery process occurs separately in the Recover section.

## Step 1: Assign a Backup Owner

Give backup ownership to a named person or provider.

Record the backup owner, technical owner, executive sponsor, MSP contact if applicable, and review schedule.

The backup owner is responsible for making sure backups exist, jobs are monitored, failures are investigated, restore tests happen, and evidence is stored.


## Step 2: Define What Must Be Backed Up

Create a clear list of what the company needs to protect.

Include business-critical data, systems, applications, SaaS platforms, configuration files, identity records, websites, databases, file storage, endpoints, and cloud workloads.

**At minimum, review these areas:**

|Backup Area|Examples|
|---|---|
|User files|Shared drives, OneDrive, Google Drive, local work folders|
|Email and collaboration|Exchange, Gmail, Teams, SharePoint, Google Workspace|
|Business systems|Accounting, CRM, HR, payroll, inventory, ticketing|
|Servers|File servers, application servers, database servers|
|Cloud systems|Cloud VMs, storage buckets, hosted databases|
|Websites|Website files, CMS files, plugins, themes, databases|
|Identity and access|Directory exports, admin records, MFA recovery records|
|Network and security configs|Firewalls, routers, switches, VPNs, Wi-Fi controllers|
|Backups of backups|Backup catalogs, backup server configs, encryption keys|
|Documentation|Asset lists, vendor contacts, emergency procedures|

If the company cannot name what is backed up, it does not have a controlled backup program.

## Step 3: Set Backup Priorities

Not all systems need the same backup frequency.

Mark each system or data set by business importance.

**Use simple categories:**

|Priority|Meaning|
|---|---|
|Critical|Business cannot operate without it|
|High|Major disruption if unavailable|
|Medium|Important, but short downtime is tolerable|
|Low|Useful, but not urgent for recovery|

For each item, record the maximum acceptable data loss and maximum acceptable downtime.

**Use plain language:**

| Term                           | Meaning                                      |
| ------------------------------ | -------------------------------------------- |
| Recovery Point Objective (RPO) | How much data the company can afford to lose |
| Recovery Time Objective (RTO)  | How quickly the company needs it restored    |

**Examples:**

- **Accounting system:** lose no more than one business day of data, restore within 24 hours.

- **Email:** lose no more than four hours of data, restore access within one business day.

- **Website:** restore within 24 hours, recover from last clean backup.

Targets are usually shorter in time when the data is more critical, or higher in volume occurring at a more rapid rate. Data that only changes once a month doesn't need to be backed up daily, for example.

## Step 4: Build the Backup Schedule

Create a backup schedule based on business need.

**Suggested starting point:**

|System Type|Suggested Backup Frequency|
|---|---|
|Critical databases|Daily or more often|
|Accounting and payroll data|Daily|
|File storage|Daily|
|Email and collaboration data|Daily|
|Website files and database|Daily or before major changes|
|Endpoint work folders|Daily or continuous|
|Server images|Daily or weekly depending on need|
|Network device configurations|After every major change and at least monthly|
|SaaS exports|Daily, weekly, or according to business impact|
|Security and IAM documentation|After every major change|

Avoid relying only on ad hoc manual exports. Manual backups are often forgotten.

## Step 5: Use a 3-2-1-1-0 Backup Structure

Use a modern version of the 3-2-1 backup model.

The company should aim for:

|Rule|Meaning|
|---|---|
|3|Keep at least three copies of important data|
|2|Store copies on at least two different types of storage|
|1|Keep at least one copy offsite|
|1|Keep at least one copy offline or immutable|
|0|Aim for zero restore errors through testing|

This is the practical target.

A backup stored on the same network, using the same admin account, with no restore test, is weak.

## Step 6: Protect Backups from Ransomware

Backups must be harder to destroy than production systems.

**Apply these controls:**

|Control|Requirement|
|---|---|
|Separate credentials|Backup admin accounts must not be the same as daily IT admin accounts|
|MFA|Backup consoles and cloud storage accounts must use MFA|
|Encryption|Backups must be encrypted in storage and during transfer where supported|
|Immutable storage|Critical backups should use immutability or object lock where possible|
|Offline copy|Keep at least one backup copy disconnected from the normal network|
|Restricted access|Only approved backup administrators should access backup systems|
|Separate storage|Do not store all backups only on production file shares|
|Protected keys|Encryption keys and recovery codes must be stored safely|
|No domain dependency where possible|Backup recovery should not fully depend on a compromised domain|
|Logging|Backup login, deletion, and job activity should be logged where possible|

Attackers often look for backup systems first. Treat backup infrastructure as a high-value target.

## Step 7: Cover SaaS Platforms

Do not assume SaaS platforms are automatically backed up in a way that matches business needs.

Microsoft 365, Google Workspace, CRM, accounting software, project management tools, HR platforms, cloud storage, and ticketing systems may have retention features, but retention is not always the same as full backup and recovery.

**For each major SaaS platform, record:**

|SaaS Backup Field|Record|
|---|---|
|Platform|Microsoft 365, Google Workspace, CRM, accounting, etc.|
|Data stored|Email, files, contacts, records, tickets, invoices|
|Native recovery options|Trash, version history, retention, export|
|Backup tool|Native, third-party, export, or none|
|Backup frequency|Daily, weekly, continuous, or manual|
|Restore method|How data is restored|
|Owner|Person responsible|
|Gap|What is not protected|

This step matters because many SMEs discover too late that deleted SaaS data cannot be recovered the way they expected.

## Step 8: Back Up Configuration and Documentation

Backups should not only cover files.

The company should also back up the information needed to rebuild systems.

**Include:**

- Firewall configurations
- Router and switch configurations
- VPN settings
- Wi-Fi settings
- DNS records
- Domain registrar information
- Website configuration
- Cloud infrastructure configuration
- Server build notes
- Application license records
- Admin contact list
- Vendor support contacts
- Backup software configuration
- Encryption key recovery process
- Incident contact sheet

If the company loses the system and the configuration, recovery becomes much slower.

## Step 9: Protect Backup Credentials and Encryption Keys

Backup credentials and encryption keys must be protected carefully.

**Ensure:**

- Store them in an approved password manager or secrets vault.
- Limit access to backup administrators.
- Require MFA.
- Keep emergency access documented.
- Keep recovery codes separate from the systems they protect.
- Do not store backup encryption keys only on the backup server.
- Do not store recovery instructions only in the system that may be down.

If keys are lost, encrypted backups may become useless.

## Step 10: Monitor Backup Jobs

Every backup job should be monitored.

Record backup success, failure, warnings, missed jobs, storage capacity, and unusual deletion activity.

The backup owner should receive alerts when backup jobs fail.

**At minimum, review:**

|Monitoring Item|Requirement|
|---|---|
|Backup success|Confirm jobs completed|
|Backup failure|Investigate immediately|
|Storage capacity|Prevent silent failures due to full storage|
|Last successful backup|Track by system|
|Missed backups|Identify systems not backed up|
|Deletion events|Alert on unusual backup deletion|
|Encryption status|Confirm backups remain encrypted|
|Offsite copy status|Confirm offsite copy completed|
|Immutable copy status|Confirm protected copy exists|

A backup system that fails silently is not a backup system. It is a future incident.

## Step 11: Test Restores

Restore testing is mandatory.

A restore test proves that backup data can actually be used.

**Test different recovery types:**

|Restore Type|Example|
|---|---|
|Single file restore|Recover one deleted file|
|Folder restore|Recover a shared folder|
|Email restore|Recover a mailbox item|
|SaaS restore|Restore cloud files or records|
|Database restore|Recover a test copy of a database|
|Server restore|Restore a server or VM|
|Website restore|Restore website files and database|
|Bare-metal or full-system restore|Rebuild a complete machine where needed|

**Recommended schedule:**

|System Type|Restore Test Frequency|
|---|---|
|Critical systems|Quarterly|
|Important systems|Twice per year|
|Lower-risk systems|Annually|
|After backup changes|Test immediately|
|After major system changes|Test immediately|

The test should be documented. If no one records it, it did not happen.

## Step 12: Check for Clean Recovery

Do not restore infected systems blindly.

Before restoring after a security incident, the company must confirm that the restore point is clean enough to use.

**Record:**

- Which restore point was selected
- Why that restore point was selected
- Whether malware scanning was performed
- Whether account compromise was considered
- Whether vulnerable systems were patched before reconnecting
- Whether passwords or keys needed rotation
- Whether restored systems were monitored after restoration

This does not replace the upcoming **#5 Recover** section. It simply makes sure the backup program supports safe recovery.

## Step 13: Document the Backup Runbook

Create a simple backup runbook.

**The runbook should explain:**

- What is backed up
- Where backups are stored
- Who owns the backups
- Who receives alerts
- How often backups run
- How long backups are retained
- How restore tests are performed
- How backup failures are handled
- How emergency access works
- Where encryption keys are stored
- How to contact backup vendors or MSPs
- What to do if ransomware is suspected

Keep a copy outside the normal production environment. If the file server is down, the company still needs the runbook.

## Step 14: Keep Backup Evidence

Store evidence that the backup program is working.

**Useful evidence includes:**

- Backup job reports
- Backup failure logs
- Storage capacity reports
- Restore test records
- Screenshots of backup settings
- Screenshots of immutability settings
- Encryption settings
- MFA settings for backup admin accounts
- Backup access reviews
- Offsite backup confirmation
- Vendor support contracts
- Backup runbook
- Backup exception approvals

This evidence helps with audits, cyber insurance, customer reviews, and incident response.

## Step 15: Review the Backup Program Regularly

Review the backup program on a fixed schedule.

**At least quarterly, check:**

- New systems added since last review
- Systems removed since last review
- Backup job failures
- Restore test results
- Storage capacity
- Backup access list
- Backup retention settings
- SaaS backup gaps
- Unsupported systems
- Backup cost changes
- Backup vendor issues
- Open backup risks

**Every major business or technology change should trigger a backup review.**

**Examples:**

- New SaaS platform
- New website
- New database
- New office
- New cloud environment
- New accounting system
- New file storage location
- New MSP
- Major employee role change
- Major data migration

Do not wait for the annual review to discover that new systems were never added to backups.

## Backup Register Template

The Backup Register is the organizational repository positioned as the central knowledge of the backups system.

|Field|What to Record|
|---|---|
|System or Data Set|Name of system, application, database, file share, SaaS platform, or device|
|Business Owner|Department or person responsible|
|Technical Owner|IT, MSP, vendor, or administrator|
|Criticality|Critical, High, Medium, or Low|
|Backup Method|Image, file, database, export, SaaS backup, snapshot|
|Backup Frequency|Daily, hourly, weekly, continuous, or manual|
|Backup Location|Local, cloud, offsite, NAS, object storage, tape, other|
|Offline or Immutable Copy|Yes, No, or Planned|
|Encryption|Yes, No, or Unknown|
|Retention Period|How long backups are kept|
|Last Successful Backup|Date and time|
|Last Restore Test|Date tested|
|Restore Owner|Person responsible for restore|
|Known Gaps|Missing coverage, failed jobs, no test, weak access, no offsite copy|
|Next Action|Required fix|
|Review Date|Next scheduled review|

## Recommended Open Source and Affordable Tools

|Tool|Link|Type|Best Use|
|---|---|---|---|
|BorgBackup|[BorgBackup](https://www.borgbackup.org/)|Open-source|Encrypted, compressed, deduplicated backups for Linux, macOS, BSD, and technical teams|
|restic|[restic](https://restic.net/)|Open-source|Encrypted backups to local, self-hosted, and cloud storage targets|
|Kopia|[Kopia](https://kopia.io/)|Open-source|Encrypted and deduplicated backups with GUI and CLI options|
|Duplicati|[Duplicati](https://duplicati.com/)|Open-source and low-cost|Encrypted backups to many cloud and remote storage providers|
|UrBackup|[UrBackup](https://www.urbackup.org/)|Open-source|Client/server file and image backups for small networks|
|Proxmox Backup Server|[Proxmox Backup Server](https://proxmox.com/en/products/proxmox-backup-server/overview)|Open-source with paid support options|VM, container, and physical host backups, especially for Proxmox environments|
|Bareos|[Bareos](https://www.bareos.com/)|Open-source with paid support options|Network backup for servers and more complex environments|
|Bacula Community|[Bacula Community](https://www.bacula.org/)|Open-source|Enterprise-style network backup for technical teams|
|BackupPC|[BackupPC](https://backuppc.github.io/backuppc/)|Open-source|Disk-based backups for Linux/Unix/Windows PCs and servers|
|rsnapshot|[rsnapshot](https://rsnapshot.org/)|Open-source|Filesystem snapshot backups using rsync and hard links|
|rclone|[rclone](https://rclone.org/)|Open-source|Moving backup data to cloud storage targets; not a full backup plan by itself|
|Syncthing|[Syncthing](https://syncthing.net/)|Open-source|File synchronization between devices; useful for sync, not a replacement for real backups|
|Veeam Backup & Replication Community Edition|[Veeam Community Edition](https://www.veeam.com/products/free/backup-recovery.html)|Free for limited workloads|Backup for small VMware, Hyper-V, Proxmox, Windows, Linux, NAS, and physical workloads|
|Veeam Backup for Microsoft 365|[Veeam Microsoft 365 Backup](https://www.veeam.com/products/saas/backup-microsoft-office-365.html)|Commercial, low-cost options|Microsoft 365 backup for Exchange, SharePoint, OneDrive, and Teams|
|Synology Active Backup for Business|[Synology Active Backup](https://www.synology.com/en-global/dsm/feature/active_backup_business)|Included with supported Synology NAS|Backup for PCs, servers, VMs, and business workloads|
|Synology Hyper Backup|[Synology Hyper Backup](https://www.synology.com/en-global/dsm/feature/hyper_backup)|Included with Synology NAS|NAS backup to local, remote, and cloud destinations|
|Backblaze B2|[Backblaze B2](https://www.backblaze.com/cloud-storage)|Low-cost cloud storage|Offsite backup storage target|
|Wasabi|[Wasabi](https://wasabi.com/)|Low-cost cloud storage|Object storage backup target|
|Amazon S3 Glacier|[Amazon S3 Glacier](https://aws.amazon.com/s3/storage-classes/glacier/)|Low-cost archive storage|Long-term archive and offsite backup storage|
|Microsoft Azure Backup|[Azure Backup](https://azure.microsoft.com/products/backup)|Commercial cloud backup|Microsoft cloud backup for servers, VMs, and workloads|
|Google Cloud Backup and DR|[Google Cloud Backup and DR](https://cloud.google.com/backup-disaster-recovery)|Commercial cloud backup|Google Cloud backup and disaster recovery workloads|
|Windows File History|[Windows File History](https://support.microsoft.com/windows/back-up-and-restore-with-file-history)|Built into Windows|Basic file backup for very small environments|
|macOS Time Machine|[Time Machine](https://support.apple.com/mac-back-up-your-files)|Built into macOS|Basic Mac backup for small environments|

## Practical Tool Guidance for SMEs

### Very small company:

- Microsoft 365 or Google Workspace native recovery features
- A third-party backup for cloud email and files where needed
- Bitwarden or another password manager for backup credentials
- External drive or NAS backup
- Offsite cloud storage
- Documented restore tests

### Small technical company:

- restic, BorgBackup, Kopia, or Duplicati
- Backblaze B2, Wasabi, or S3-compatible storage
- Gitleaks or secret scanning for code repositories
- Separate storage credentials
- Quarterly restore tests

### Small company with servers:

- Veeam Community Edition
- UrBackup
- Proxmox Backup Server
- Synology Active Backup
- NAS plus offsite object storage
- Documented server restore procedure

### Self-hosted or Linux-heavy company:

- BorgBackup
- restic
- Kopia
- Bareos
- Bacula Community
- Proxmox Backup Server
- rclone for offsite transfer

### Company using Microsoft 365 heavily:

- Microsoft 365 retention features where appropriate
- Third-party Microsoft 365 backup
- Veeam Backup for Microsoft 365
- Backup of SharePoint, OneDrive, Exchange, Teams, and Entra-related records where available

### Company using Google Workspace heavily:

- Google Vault or native retention where appropriate
- Third-party Google Workspace backup where business need requires it
- Regular export process for critical records
- Google Admin audit review

## Further Steps

### Backup Failure Handling

Backup failures must be treated as operational issues.

**When a backup fails:**

- Record the failed job.
- Identify the affected system.
- Check the error message.
- Confirm whether the next backup succeeded.
- Fix the cause.
- Run a manual backup if needed.
- Record the resolution.
- Escalate if a critical system remains unprotected.

A failed backup for a critical system should not sit unnoticed for weeks.

### Backup Exception Handling

Some systems may be difficult to back up.

**Do not ignore them. Record the exception.**

|Exception Field|Record|
|---|---|
|System|Name of system|
|Missing backup|What is not protected|
|Reason|Technical, vendor, cost, legacy, unknown|
|Business impact|What happens if it is lost|
|Temporary control|Export, manual copy, vendor recovery, screenshot, documentation|
|Owner|Person responsible|
|Review date|When exception must be revisited|

An exception without an expiration date becomes a permanent weakness.

## Expected Outputs from This Section

At the end of this section, the company should have:

- A named backup owner.
- A list of systems and data that must be backed up.
- Backup priorities for critical systems.
- Backup frequency and retention targets.
- At least one offsite backup copy for critical data.
- At least one offline or immutable backup copy for critical data where practical.
- MFA and access control for backup systems.
- Encrypted backups where supported.
- A SaaS backup review.
- Backup of important configurations and documentation.
- Backup job monitoring.
- A restore testing schedule.
- Documented restore test evidence.
- A backup runbook.
- A backup register.
- A backup exception list.
- A quarterly backup review process.


## Objectives

Do not trust a backup because it exists. Trust it only after it has restored cleanly.

The company should leave this section able to say:

“We know what is backed up, where it is stored, who owns it, how often it runs, how long it is retained, whether attackers can delete it, and when it was last restored successfully.”

That is backup readiness.

---

