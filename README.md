# splunk-email-security-monitoring
Email Security Monitoring and Threat Detection Dashboard built with Splunk Enterprise. Analyse SMTP logs, TLS encryption, suspicious email activities, attachments, sender behaviour and geographical email traffic.
# Splunk Email Security Monitoring & Threat Detection Dashboard

## Project Overview

This project demonstrates the use of **Splunk Enterprise** as a Security Information and Event Management (SIEM) platform for monitoring, analysing and investigating email security activities.

The dashboard provides security visibility into email traffic, suspicious senders, email attachments, TLS encryption status and geographical email traffic patterns.

The primary objective is to help SOC analysts identify potentially malicious email activities, investigate suspicious messages and understand email-related security risks within an organisation.

## Project Objectives

- Monitor incoming and outgoing email activities.
- Analyse SMTP email logs.
- Identify suspicious email senders and recipients.
- Monitor emails containing attachments.
- Identify email connections without TLS encryption.
- Investigate potentially suspicious email activities.
- Analyse email traffic based on source IP addresses and geographical locations.
- Provide security visibility through Splunk dashboards.

## Dashboard Overview

The dashboard provides the following monitoring capabilities:

### 1. Email Security Overview

Displays key email security metrics:

| Metric | Description |
|---|---|
| Total Emails | Total number of email events monitored |
| Emails with Attachments | Emails containing file attachments |
| Unencrypted (No TLS) | Email events without TLS encryption |
| Suspicious Emails | Emails flagged for further security investigation |

### 2. Top Senders

Identifies the most active email senders.

This panel helps analysts investigate:

- Unusual email-sending volumes.
- Suspicious sender addresses.
- Potential phishing campaigns.
- Possible compromised email accounts.

### 3. Attachment Types

Visualises the distribution of email attachment extensions.

The dashboard includes file types such as:

- PDF
- DOCX
- XLSX
- ZIP
- EXE
- JS

This helps analysts identify potentially risky attachment types that may require further investigation.

### 4. Suspicious Email Details

Provides a detailed view of potentially suspicious email events.

The table includes:

| Field | Description |
|---|---|
| Timestamp (ts) | Date and time of the email event |
| Source IP (id.orig_h) | Originating IP address |
| Mail From | Sender email address |
| Recipient (rcptto) | Recipient email address |
| Subject | Email subject |
| Attachment Type | Type of attached file |
| TLS Version | TLS information recorded in the event |

### 5. Email Traffic by Source Country

Provides geographical visibility into email traffic based on source IP addresses.

This helps SOC analysts investigate:

- Unusual geographical email traffic.
- Unexpected source locations.
- Potentially suspicious external email activity.
- Traffic patterns requiring further investigation.

## Technologies Used

- **Splunk Enterprise:** SIEM platform for log ingestion, searching, analysis and visualisation.
- **SMTP Logs:** Email transmission and communication analysis.
- **TLS Logs:** Encryption and secure communication analysis.
- **SPL (Search Processing Language):** Searching, filtering, analysing and transforming log data.
- **Splunk Dashboards:** Security monitoring and visualisation.

## SOC Analyst Investigation Scenarios

This project supports practical investigation scenarios, including:

1. Identifying suspicious email senders.
2. Investigating emails containing executable attachments.
3. Detecting email traffic without TLS encryption.
4. Identifying unusual email-sending patterns.
5. Investigating suspicious source IP addresses.
6. Analysing potentially malicious email campaigns.
7. Investigating unusual geographical email traffic.

**Important:** A suspicious indicator does not automatically confirm a security incident. Further investigation and correlation with other security logs are required.

## Dashboard Screenshot

![Splunk Email Security Monitoring Dashboard](screenshots/email-security-dashboard.png)

## Learning Outcomes

Through this project, I gained practical experience in:

- Working with Splunk Enterprise.
- Understanding SMTP and TLS logs.
- Analysing email security events.
- Using SPL for security log analysis.
- Building security monitoring dashboards.
- Identifying suspicious email indicators.
- Developing SOC investigation and threat detection skills.
- Presenting security findings through visual dashboards.

## Project Purpose

This project was developed as part of my practical cybersecurity and Security Operations Centre (SOC) Analyst learning journey.

It demonstrates how SIEM technology can be used to improve email security visibility and support security monitoring and incident investigation.

## Disclaimer

This project is intended for educational and cybersecurity training purposes. The dashboard indicators are intended to support investigation and should not be treated as definitive evidence of malicious activity.

---

**Author:** Adexbit  
**Project:** Splunk Email Security Monitoring & Threat Detection  
**Platform:** Splunk Enterprise  
**Category:** Security Operations Centre (SOC) / SIEM / Email Security
