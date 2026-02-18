# splunk-log-analysis.md
## Lab: SIEM Log Analysis – Suspicious Login Activity

### Objective
Analyze authentication logs in a SIEM to identify suspicious login behavior and determine potential security risks.

### Tools Used
- Splunk
- Windows Event Logs
- MITRE ATT&CK

### Scenario
Multiple failed login attempts followed by a successful login were detected from a single IP address.

### Steps Taken
1. Queried authentication logs using Event ID 4625 and 4624
2. Identified repeated failed login attempts from the same IP
3. Correlated timestamps between failed and successful attempts
4. Checked IP reputation using threat intelligence sources
5. Mapped behavior to MITRE technique T1110 (Brute Force)

### Findings
- Source IP showed brute-force behavior
- Successful login occurred after multiple failures
- Account potentially compromised

### Outcome
Alert escalated as **High Severity**. Recommended password reset, IP blocking, and enabling MFA.

### Skills Demonstrated
- Log Analysis
- SIEM Querying
- Threat Detection
- MITRE ATT&CK Mapping
