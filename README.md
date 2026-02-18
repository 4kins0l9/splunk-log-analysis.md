# splunk-log-analysis.md
## Lab: Phishing Email Investigation

### Objective
Investigate a suspected phishing email and determine its impact on the organization.

### Tools Used
- SIEM
- VirusTotal
- Email Headers
- MITRE ATT&CK

### Scenario
User reported a suspicious email requesting credential verification.

### Steps Taken
1. Reviewed email headers for sender authenticity
2. Extracted URLs and attachment hashes
3. Analyzed indicators using VirusTotal
4. Checked SIEM for user click activity
5. Assessed potential account compromise

### Findings
- Sender domain spoofed a legitimate service
- URL flagged as malicious by multiple vendors
- No evidence of credential submission detected

### Outcome
Classified as **Confirmed Phishing Attempt**. Email removed from inboxes and awareness advisory sent to users.

### Skills Demonstrated
- Incident Response
- Email Security Analysis
- Threat Intelligence
- User Risk Assessment
