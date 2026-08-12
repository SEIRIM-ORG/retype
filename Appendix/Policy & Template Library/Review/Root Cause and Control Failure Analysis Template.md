

## Purpose

Use this template to determine why an incident occurred and which cybersecurity, technical, business, or human controls failed or were missing.

The objective is to identify the conditions that allowed the incident to happen, not simply the final action that triggered it.

**For example:**

“An employee clicked a phishing link” is usually not a complete root cause.

The deeper questions may include:

- Why did the message reach the employee?
- Why could the stolen password be used?
- Why did the account have broad access?
- Why was suspicious activity not detected?
- Why could the attacker remain active?

## Incident Information

Incident ID: ____________________

Incident: ____________________

Analysis owner: ____________________

Analysis date: ____________________

Participants: ____________________

## 1. Confirm the Incident Sequence

Summarize the sequence that led to the incident:

1. ---
    
2. ---
    
3. ---
    
4. ---
    
5. ---
    

## 2. Initial Entry Point

**How did the incident begin?**

- Phishing
- Stolen credentials
- Exploited vulnerability
- Misconfiguration
- Vendor compromise
- Insider misuse
- Malware
- Lost device
- Exposed service
- Human error
- Unknown
- Other: ____________________

Evidence supporting this conclusion:

---

Confidence:

- Confirmed / Likely / Possible / Unknown

## 3. Immediate Cause

What directly allowed the incident to succeed?

---

Examples:

- User entered credentials into a phishing site.
- Internet-facing server was unpatched.
- Vendor account had excessive access.
- Public sharing was enabled.
- Administrator credential was stolen.
- Employee bank details were changed without verification.

## 4. Ask Why Repeatedly

### Why 1

Why was the immediate cause possible?

---

### Why 2

Why did that condition exist?

---

### Why 3

Why was it not prevented or corrected?

---

### Why 4

Why was it not detected earlier?

---

### Why 5

What underlying process, ownership, technical, or management issue allowed the weakness to remain?

---

Not every incident requires exactly five levels. Continue until the analysis reaches conditions the company can meaningfully improve.

## 5. Preventive Control Failures

**Which controls should have prevented or reduced the incident?**

- [ ]  MFA.
- [ ]  Access control.
- [ ]  Secure configuration.
- [ ]  Patching.
- [ ]  Email security.
- [ ]  Endpoint protection.
- [ ]  Network restriction.
- [ ]  Vendor control.
- [ ]  Payment verification.
- [ ]  Data handling controls.
- [ ]  Employee training.
- [ ]  Separation of duties.
- [ ]  Other: ____________________

**For each failed control:**

Expected control: ____________________

What actually existed: ____________________

Why it failed or was missing: ____________________

## 6. Detective Control Failures

**Consider:**

- [ ]  Logging missing.
- [ ]  Alert missing.
- [ ]  Alert not monitored.
- [ ]  Alert ignored.
- [ ]  Insufficient log retention.
- [ ]  Suspicious activity not recognized.
- [ ]  Employee reporting delayed.
- [ ]  External notification provided first indication.

Details:

---

## 7. Response Control Failures

**Consider:**

- [ ]  Incident owner unclear.
- [ ]  Escalation delayed.
- [ ]  Contact information unavailable.
- [ ]  Evidence lost.
- [ ]  Containment incomplete.
- [ ]  Compromised sessions remained active.
- [ ]  Vendor response delayed.
- [ ]  Decision authority unclear.
- [ ]  Communications inconsistent.

Details:

---

## 8. Recovery Control Failures

**Consider:**

- [ ]  Backups unavailable.
- [ ]  Backup compromised.
- [ ]  Restore not previously tested.
- [ ]  Recovery priorities unclear.
- [ ]  Dependencies unknown.
- [ ]  Restore introduced previous weakness.
- [ ]  Business validation incomplete.
- [ ]  Recovery took longer than expected.

Details:

---

## 9. Business and Human Process Failures

**Consider:**

- [ ]  Responsibility unclear.
- [ ]  Excessive access.
- [ ]  Weak onboarding.
- [ ]  Weak offboarding.
- [ ]  Shared accounts.
- [ ]  Approval process bypassed.
- [ ]  Vendor responsibilities unclear.
- [ ]  Staff not trained.
- [ ]  Procedure existed but was not followed.
- [ ]  Procedure did not reflect actual operations.
- [ ]  Security exception became permanent.

Details:

---

## 10. Root Cause Statement

Primary root cause:

---

Contributing factors:

---

What evidence supports this conclusion?

---

**Confidence:**

- Confirmed / Likely / Partial / Unknown

## 11. Required Improvements

**For each root cause or material contributing factor:**

Required action: ____________________

Control being improved: ____________________

Owner: ____________________

Priority: ____________________

Due date: ____________________

Verification method: ____________________

Evidence required: ____________________

## Practical Rule

Do not stop at the last human mistake or technical failure.

Find the conditions that allowed the mistake or failure to become an incident.