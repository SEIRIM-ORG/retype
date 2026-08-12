


## Purpose

This policy defines how the company protects important systems and data through backups and how those backups should support recovery after accidental deletion, system failure, ransomware, cyber incidents, or other disruption.

The goal is not simply to create backups. The company should be able to restore important information and systems within a timeframe that supports business needs.

## Scope

**This policy applies to important:**

- Business data
- File storage
- Servers
- Databases
- Cloud workloads
- SaaS platforms
- Websites
- Business applications
- Configuration information
- Critical system documentation
- Other information required to restore business operations

## Backup Ownership

Each important backup process should have an owner.

**The owner is responsible for confirming:**

- The required system or data is included
- Backups run successfully
- Failures are investigated
- Retention is appropriate
- Backup access is protected
- Restore testing occurs
- Backup owner: ____________________
- Backup owner backup/contact: ____________________

## What Must Be Backed Up

The company should identify which systems and information are required for business recovery.

**Priority should be given to:**

- Critical business data
- Customer and employee records
- Financial records
- Operational systems
- Important databases
- Business file storage
- Website and application data
- Configuration files
- Security and infrastructure configuration where necessary

The company should not assume SaaS or cloud providers automatically provide the level of backup and recovery the business requires.

## Backup Frequency

Backup frequency should reflect how much data the company can reasonably afford to lose.

More frequently changing or business-critical information should normally be backed up more frequently than low-value or rarely changing information.

**Backup frequency: __________________**

## Retention

The company should define how long backups are retained.

**Retention should consider:**

- Business requirements
- Recovery needs
- Accidental deletion
- Ransomware that may remain unnoticed
- Legal or contractual requirements
- Storage cost
- Retention periods should be documented

## Protection From Ransomware and Deletion

Where practical, at least one backup copy should be protected from normal user or administrator compromise.

**Protection may include:**

- Immutable storage
- Offline copies
- Separate backup credentials
- Separate administrative accounts
- Restricted deletion permissions
- Different storage environments
- MFA on backup administration

An attacker who compromises the normal environment should not automatically be able to destroy every backup.

## Monitoring

Backup failures should generate alerts.

Alerts should be sent somewhere that is actively monitored.

**Backup owners should investigate:**

- Failed jobs
- Partial jobs
- Storage capacity problems
- Unexpected retention changes
- Disabled protection
- Unusual deletion
- Missed schedules

## Restore Testing

Backups should be tested through actual restoration.

**Testing should confirm:**

- The backup exists
- The data can be restored
- The restored information is usable
- The recovery procedure is understood
- Important dependencies are available
- Recovery time is acceptable

Critical systems should be tested more frequently than low-risk systems.

## Access Control

Access to backup systems should be limited.

**Where practical:**

- Use named administrator accounts
- Require MFA
- Separate backup administration from ordinary user accounts
- Restrict deletion rights
- Review administrator access
- Log important backup changes

## Backup Documentation

**Record:**

- System or data protected
- Backup owner
- Backup method
- Frequency
- Retention
- Backup location
- Protection method
- Last successful backup
- Last restore test
- Recovery dependencies
- Known gaps

## Recovery

Recovery should follow documented business priorities.

Before using backups after a cybersecurity incident, the company should consider whether the restore point is trustworthy and whether the vulnerability or attacker access that caused the incident has been removed.

## Exceptions

Backup gaps should be documented.

**Where a required backup cannot be implemented:**

- Record the reason
- Record the risk
- Assign an owner
- Apply temporary controls
- Set a remediation or review date

## Review

**Review this policy at least annually and after:**

- Serious incidents
- Major system changes
- Backup failures
- Recovery failures
- New critical systems
- Significant business changes

## Practical Rule

A backup is only useful if the company can restore from it.