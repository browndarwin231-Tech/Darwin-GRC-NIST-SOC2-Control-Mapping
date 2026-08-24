# GRC Gap Assessment

## Executive Summary

This assessment reviews the cybersecurity and compliance posture of the fictional organization CloudNova Technologies.

The assessment focuses on security controls aligned with the NIST Cybersecurity Framework and SOC 2-related control areas.

The review identified several gaps involving identity and access management, third-party risk management, incident response testing, backup validation, and privileged account reviews.

The highest-priority risks involve former employee access, untested incident response procedures, third-party vendor risk, and excessive privileged access.

---

## Assessment Scope

The assessment reviewed the following areas:

- Identity and Access Management
- Privileged Access
- Security Monitoring
- Incident Response
- Third-Party Risk Management
- Security Awareness
- Backup and Recovery
- Network Security

---

## Finding 1: Terminated User Access

### Current State

Employee accounts are not always disabled immediately after termination.

### Risk

Former employees may retain access to company systems or sensitive information.

### Risk Level

**High**

### Framework Mapping

- NIST CSF: PR.AA
- SOC 2 Area: Logical Access

### Gap

The organization does not have a consistently enforced process for immediately disabling terminated-user accounts.

### Recommendation

Integrate account deactivation into the employee offboarding process.

Access should be removed immediately when employment ends.

Quarterly access reviews should also be performed to identify inactive or unnecessary accounts.

---

## Finding 2: Privileged Account Reviews

### Current State

Administrator accounts exist but are not reviewed regularly.

### Risk

Users may retain elevated permissions they no longer require.

Excessive privileged access could increase the impact of account compromise or insider misuse.

### Risk Level

**High**

### Framework Mapping

- NIST CSF: PR.AA
- SOC 2 Area: Logical Access

### Gap

There is no formal recurring privileged-access review process.

### Recommendation

Conduct quarterly privileged-access reviews.

Remove unnecessary permissions and document management approval for privileged access.

---

## Finding 3: Third-Party Vendor Risk

### Current State

The organization uses third-party vendors but does not maintain a formal vendor risk assessment process.

### Risk

A compromised or insecure vendor could expose company systems or sensitive data.

### Risk Level

**High**

### Framework Mapping

- NIST CSF: ID.RA
- SOC 2 Area: Vendor Management

### Gap

Vendors are not consistently evaluated for cybersecurity and compliance risk.

### Recommendation

Implement a third-party risk management process that includes:

- Vendor security questionnaires
- Vendor risk classifications
- Security documentation review
- Contract and security requirement review
- Recurring reassessments

---

## Finding 4: Incident Response Testing

### Current State

CloudNova Technologies maintains an incident response plan.

However, the organization has not performed formal tabletop exercises.

### Risk

Employees may not know how to respond effectively during a real security incident.

This may increase incident containment and recovery time.

### Risk Level

**High**

### Framework Mapping

- NIST CSF: RS.MA
- SOC 2 Area: Incident Management

### Gap

The incident response plan exists but has not been tested.

### Recommendation

Conduct an incident response tabletop exercise at least annually.

Document:

- Participants
- Scenario
- Response actions
- Lessons learned
- Identified weaknesses
- Corrective actions

---

## Finding 5: Backup Restoration Testing

### Current State

The organization performs backups but does not consistently test restoration.

### Risk

Backups may be unavailable or unusable during a ransomware incident, system failure, or disaster.

### Risk Level

**Medium**

### Framework Mapping

- NIST CSF: RC.RP
- SOC 2 Area: Availability

### Gap

There is no consistent documented backup restoration testing schedule.

### Recommendation

Perform quarterly backup restoration tests.

Document the recovery results and investigate any unsuccessful restoration attempts.

---

## Finding 6: Security Monitoring Review

### Current State

Security logs are collected centrally.

### Risk

Important threats may go undetected if logging coverage and detection rules are not reviewed regularly.

### Risk Level

**Medium**

### Framework Mapping

- NIST CSF: DE.CM
- SOC 2 Area: System Monitoring

### Gap

The organization has centralized logging but lacks documented recurring reviews of detection coverage.

### Recommendation

Review log sources and security detection coverage regularly.

Confirm that critical systems are sending logs and that appropriate alerts exist for high-risk activity.

---

## Finding 7: Security Awareness Effectiveness

### Current State

Employees receive security awareness training.

### Risk

Employees may remain vulnerable to phishing or social-engineering attacks if training effectiveness is not measured.

### Risk Level

**High**

### Framework Mapping

- NIST CSF: PR.AT
- SOC 2 Area: Personnel Security

### Gap

Training exists, but its effectiveness is not consistently measured.

### Recommendation

Conduct recurring phishing simulations.

Track:

- Training completion
- Phishing failure rates
- Repeat failures
- Improvement over time

---

## Overall Risk Summary

| Finding | Risk Level | Priority |
|---|---|---|
| Terminated User Access | High | Immediate |
| Privileged Account Reviews | High | Immediate |
| Third-Party Vendor Risk | High | High |
| Incident Response Testing | High | High |
| Backup Restoration Testing | Medium | Medium |
| Security Monitoring Review | Medium | Medium |
| Security Awareness Effectiveness | High | High |

---

## Conclusion

CloudNova Technologies has several foundational security controls in place, including MFA, centralized logging, security awareness training, firewalls, and backups.

However, the assessment identified weaknesses in access governance, vendor risk management, incident response testing, backup validation, and security-control monitoring.

The organization should prioritize remediation of high-risk findings first and establish recurring review processes to maintain compliance and reduce cybersecurity risk.
