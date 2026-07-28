# SPL Queries – SOC-002: Suspicious Email Investigation

## Overview

This document contains example Splunk searches that could be used to investigate suspicious email activity in an enterprise environment.

**Note:** This investigation focused on manual email header analysis because the dataset did not contain enterprise email logs. The searches below demonstrate how similar investigations could be performed if email logs were indexed into Splunk.

---

## Query 1 – Search by Sender

```spl
index=email sender="Mantra Falcon"
```

**Purpose**

Locate all emails sent by the identified sender.

---

## Query 2 – Search by Subject

```spl
index=email subject="Sr. AI Engineer opening"
```

**Purpose**

Find emails with the same subject line.

---

## Query 3 – Search by Recipient

```spl
index=email recipient="xmarksthespot@gmail.com"
```

**Purpose**

Identify messages delivered to the intended recipient.

---

## Query 4 – Search by Sender Domain

```spl
index=email "*terrigenisis.com*"
```

**Purpose**

Locate emails associated with the sender's domain.

---

## Query 5 – Search by Keywords

```spl
index=email ("AI Engineer" OR sponsorship OR visa)
```

**Purpose**

Identify emails containing similar wording or recruitment-related content.

---

## Query 6 – Search for Authentication Results

```spl
index=email (SPF OR DKIM OR DMARC)
```

**Purpose**

Locate emails containing authentication results for SPF, DKIM, or DMARC.

---

## Query 7 – Search for Similar Messages

```spl
index=email "Mantra Falcon" OR "Sr. AI Engineer opening"
```

**Purpose**

Determine whether similar emails have been received elsewhere in the organization.

---

# Investigation Summary

The suspicious email investigation involved:

- Reviewing email headers
- Validating SPF, DKIM, and DMARC
- Inspecting sender information
- Examining email content
- Identifying potential phishing indicators
- Documenting findings

The available evidence indicated that the email successfully passed SPF, DKIM, and DMARC authentication checks. No clear evidence of email spoofing was identified during the investigation.

---

# Skills Demonstrated

- Splunk Search Language (SPL)
- Email Header Analysis
- Email Authentication (SPF, DKIM, DMARC)
- Threat Investigation
- Indicator of Compromise (IOC) Analysis
- Security Documentation
