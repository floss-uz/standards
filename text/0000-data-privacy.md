- Standartization Name: Data Privacy and Personal Data Governance

- Start Date: 2025-10-30

- RFC PR: N/A

- STD Issue: N/A

- Severity: MUST

# Summary

This RFC establishes the mandatory data governance framework for FLOSS
Uzbekistan and its member communities. It mandates principles of **Data
Minimization, Purpose Limitation, Geographic Storage,** and robust **Subject
Rights** (access, rectification, deletion) to ensure the privacy of all
community members and adhere to best practices in data protection.

# Motivation

As FLOSS Uzbekistan and its member communities mature, it becomes essential
to establish trust and legal clarity regarding the handling of member
data. Adopting a strong, transparent privacy policy not only protects our
community members but also positions the organization as a leader in ethical
data stewardship within the Uzbek IT ecosystem. This standard minimizes legal
risk and builds confidence among contributors, users, and potential partners.

# I. Principles of Data Minimization and Collection

## A. Definition of Personal Data

**Personal data** is any information relating to an identified or identifiable
natural person. In the community context, this includes, but not limited
to these:

- **Direct Identifiers:** Full Name, Email Address, Phone Number,
Telegram/Matrix/GitHub ID.

- **Indirect Identifiers:** IP Address logs, Geolocation data, and private
correspondence.

## B. Data Minimization and Consent

- **Purpose Limitation:** Every instance of personal data collection **MUST**
be publicly stated and fully justified by a specific, documented community
function. No extra data gathering is permitted.

- **Explicit Consent:** Any collection of data beyond what is strictly
necessary for basic function (e.g., username for core project contribution)
**MUST** require explicit, affirmative **opt-in** consent. Consent must be
easily revocable.

- **Data Aggregation Policy:** Data used for community health analysis (e.g.,
message counts, contribution velocity) **MUST** be immediately **anonymized
and aggregated**. Only anonymized data may be retained beyond the general
retention period.

# II. Storage, Retention, and Security

## A. Data Localization

- **Geographic Storage:** All personal data collected by FLOSS Uzbekistan
or its member communities **MUST** be stored exclusively on servers located
**within the geographical borders of Uzbekistan**. Data **MUST NOT** leave
the country.

## B. Retention and Deletion

- **Retention Limit:** Personal data **MUST** be stored no longer than **two
(2) years** after the individual's last recorded active engagement with the
community (or the documented purpose has been fulfilled).

- **Security Measures:** All systems storing personal data **MUST** employ
modern security measures, including **encryption at rest** (when stored)
and **encryption in transit** (via HTTPS/TLS).

- **Access Control:** Access to personal data **MUST** be strictly limited
on a **"need-to-know" basis** to designated roles (e.g., Community Chair,
CoC Response Team).

## C. Data Sharing (MUST)

- **Third-Party Prohibition:** Personal data collected by FLOSS Uzbekistan
is **NEVER** shared, sold, or transferred to any third party (commercial
entities, external organizations, etc.) under any circumstance, unless
legally mandated by Uzbek law.

# III. Data Subject Rights and Enforcement

## A. The Right to Access and Portability (MUST)

- **Data Download:** The community **MUST** provide an **easy process**
for members to download a copy of all their personal data (Portability)
held by the organization in a common, structured format (e.g., JSON or CSV).

- **Right to Rectification:** Members **MUST** have an easy process (preferably
a self-service option) to correct or update their personal data.

## B. The Right to Erasure (MUST)

- **Easy Deletion:** The community **MUST** establish a clear, auditable
process for the deletion of personal data upon request (the Right to Be
Forgotten).

- **Timeframe:** All deletion requests **MUST** be processed and completed
within **30 calendar days** of receipt.

- **Confirmation:** The designated contact **MUST** confirm the completion
of deletion to the requesting member.

## C. Breach Protocol and Enforcement (MUST)

- **Data Breach Protocol:** The Community Chair **MUST** define a clear
procedure for handling a data breach, including **immediate notification**
to affected individuals (within 72 hours of discovery) and communication of
mitigation steps.

- **CoC Data Protection:** Sensitive personal data gathered during a Code of
Conduct investigation **MUST** have the highest level of restricted access
and be purged immediately after the case is closed and any mandatory retention
period (for audit logs only) is passed.

# IV. Unresolved Questions

- What specific technical standards (e.g., ISO certifications for cloud
hosting providers) will be required to ensure compliance with the **Data
Localization** requirement?

- How will the council fund and implement the necessary infrastructure (e.g.,
secure database, encryption tools) to guarantee the **two-year deletion and
30-day portability** rights?

# V. Future Possibilities

A future RFC could establish a Data Privacy Officer (DPO) role within the FLOSS
Uzbekistan council to oversee compliance, conduct regular privacy audits,
and serve as the final escalation point for data subject requests. This
would formalize accountability for the entire network.
