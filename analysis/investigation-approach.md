# Investigation Approach

## Overview

Following confirmation of an employee email compromise, the primary objective of the investigation is to determine how the attacker progressed beyond the initial point of access and whether organizational data was accessed or exfiltrated.

The investigation should follow a structured evidence-driven approach.

---

## Phase 1 — Initial Access Investigation

### Objective

Determine how the employee account was compromised.

### Activities

- Review email security alerts
- Analyze authentication logs
- Validate source IP addresses
- Review VPN authentication
- Identify suspicious login behavior

### Evidence Sources

- Email gateway logs
- Identity provider logs
- Authentication logs
- VPN logs
- MFA events

---

## Phase 2 — Account Activity Investigation

### Objective

Determine what resources were accessed after compromise.

### Activities

- Review mailbox activity
- Analyze cloud storage access
- Examine file downloads
- Identify permission changes
- Estimate scope of account access

### Evidence Sources

- Mailbox audit logs
- SharePoint or OneDrive logs
- File access logs
- Cloud audit logs
- User activity reports

---

## Phase 3 — Lateral Movement Investigation

### Objective

Determine whether attackers expanded access within the environment.

### Activities

- Review remote authentication
- Analyze privilege escalation
- Investigate administrative activity
- Examine endpoint telemetry
- Identify additional compromised systems

### Evidence Sources

- Active Directory logs
- Windows Security Events
- EDR telemetry
- RDP and SMB logs
- Network authentication logs

---

## Phase 4 — Data Exfiltration Investigation

### Objective

Confirm whether sensitive information left the organization.

### Activities

- Review large file downloads
- Analyze outbound network traffic
- Identify external destinations
- Estimate data volume
- Determine affected information

### Evidence Sources

- Firewall logs
- Proxy logs
- DLP alerts
- Network flow records
- Cloud audit logs

---

## Investigation Outcome

The investigation should reconstruct the complete attacker lifecycle by correlating evidence from email, identity, endpoint, cloud, and network environments. Conclusions should be supported by validated forensic evidence rather than assumptions.
