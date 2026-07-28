# SOC-002: Suspicious Email Investigation

## Executive Summary

A suspicious email was investigated to determine whether it represented a phishing attempt or a legitimate communication.

The investigation included analysis of the email headers, sender information, authentication results, and message content. Evidence was collected and documented throughout the investigation.

---

## Investigation Objective

Determine:

- Sender legitimacy
- SPF authentication
- DKIM authentication
- DMARC alignment
- Indicators of phishing
- Recommended response

---

## Investigation Steps

### Step 1 – Examine Email Headers

Reviewed the raw email headers.

Evidence:
- Screenshots/Evidence-01-Email-Headers.png
- Email-Headers.txt

---

### Step 2 – Verify Email Authentication

Checked:

- SPF
- DKIM
- DMARC

Evidence:

Screenshots/Evidence-02-Authentication-Results.png

---

### Step 3 – Inspect Email Content

Reviewed:

- Subject
- Sender
- URLs
- Attachments
- Social engineering indicators

Evidence:

Screenshots/Evidence-03-Email-Body.png

---

### Step 4 – Document Findings

Collected all evidence and determined the final assessment.

Evidence:

Screenshots/Evidence-04-Investigation-Summary.png

---

# Findings

Example findings:

- Sender address reviewed.
- Authentication results analyzed.
- No malicious attachment observed.
- Message content inspected for phishing techniques.

---

# Indicators of Compromise (IOCs)

| Indicator | Value |
|------------|-------|
| Sender | (example@example.com) |
| Subject | Suspicious Email |
| SPF | Pass/Fail |
| DKIM | Pass/Fail |
| DMARC | Pass/Fail |

---

# Conclusion

Based on the available evidence, the email was analyzed using standard SOC investigation procedures.

The investigation demonstrates the ability to:

- Analyze email headers
- Interpret SPF, DKIM and DMARC
- Review message content
- Document evidence
- Produce an investigation report

---

# MITRE ATT&CK

| Technique | Description |
|-----------|-------------|
| T1566 | Phishing |

---

# Skills Demonstrated

- Email Analysis
- Header Analysis
- Threat Hunting
- IOC Identification
- Documentation
- Security Investigation
