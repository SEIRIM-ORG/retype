

## Purpose

Use this checklist before declaring a restored system, service, or business process recovered.

A system is not recovered simply because it powers on or users can log in. Technical operation, security, data, monitoring, backups, access, and business functionality should all be checked.

## Recovery Information

System or service: ____________________

Incident: ____________________

Recovery owner: ____________________

Business owner: ____________________

Restore date: ____________________

Validation date: ____________________

## Restore Source

- [ ]  Restore source identified.
- [ ]  Restore point considered trustworthy.
- [ ]  Backup integrity checked where practical.
- [ ]  Restore source predates known malicious activity where required.
- [ ]  Recovery source documented.

## Technical Validation

- [ ]  System starts correctly.
- [ ]  Required services are running.
- [ ]  Application operates normally.
- [ ]  Required dependencies are available.
- [ ]  Database connections work.
- [ ]  Network connectivity is correct.
- [ ]  DNS functions correctly where applicable.
- [ ]  Integrations work.
- [ ]  Performance is acceptable.
- [ ]  Errors or warnings reviewed.

## Data Validation

- [ ]  Required data is present.
- [ ]  Data appears complete.
- [ ]  Recent transactions reviewed.
- [ ]  File integrity checked where practical.
- [ ]  Database integrity checked where appropriate.
- [ ]  Business owner confirms required information is available.
- [ ]  Missing data is documented.

## Access Validation

- [ ]  Required users can access the system.
- [ ]  Unnecessary users do not have access.
- [ ]  Administrator access reviewed.
- [ ]  MFA enabled where required.
- [ ]  Compromised credentials have been changed.
- [ ]  Suspicious sessions revoked.
- [ ]  Vendor access reviewed.
- [ ]  Temporary recovery accounts reviewed.

## Security Validation

- [ ]  Vulnerability or weakness that contributed to the incident has been addressed.
- [ ]  Required patches applied.
- [ ]  Secure configuration restored.
- [ ]  Endpoint protection active.
- [ ]  Firewall protection active.
- [ ]  Unnecessary exposure removed.
- [ ]  Malicious persistence checked where relevant.
- [ ]  Security tools functioning.

## Logging and Monitoring

- [ ]  Authentication logging active.
- [ ]  Administrative activity logging active where required.
- [ ]  Security alerts active.
- [ ]  Logs reach the expected monitoring system.
- [ ]  Incident indicators monitored where appropriate.
- [ ]  Enhanced monitoring enabled temporarily if needed.

## Backup Validation

- [ ]  Normal backup schedule resumed.
- [ ]  Backup failures will generate alerts.
- [ ]  New backup created after recovery where appropriate.
- [ ]  Backup access reviewed.
- [ ]  Next restore test scheduled.

## Business Validation

- [ ]  Business owner tests the restored process.
- [ ]  Key transactions work.
- [ ]  Customer-facing functionality works.
- [ ]  Required reports work.
- [ ]  Required integrations work.
- [ ]  Temporary workaround records reconciled.
- [ ]  Users informed that the system is available.
- [ ]  Known limitations communicated.

## Residual Risk

Are any known risks still open?

- Yes / No

If yes:

Risk: ____________________

Owner: ____________________

Temporary control: ____________________

Due date: ____________________

Leadership acceptance required: Yes / No

## Approval for Normal Use

Technical owner approval: ____________________

Security / IT approval: ____________________

Business owner approval: ____________________

Return-to-service date/time: ____________________

Evidence location: ____________________

## Practical Rule

Recovery is complete only when the technology works, the business works, the security controls work, and the remaining risks are understood.