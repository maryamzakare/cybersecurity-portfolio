# My Incident Response Playbook

## What This Project Is About

This project is an Incident Response Playbook for a simulated company called SAM LLC, a small financial services company that experienced a phishing attack.

The goal of the playbook is to show how an Incident Response Team should respond to cyber incidents in a clear, repeatable, and professional way.

## Company Scenario

SAM LLC experienced a phishing attack where an employee clicked a malicious link and entered personal information and network login credentials.

After the incident, the company needed a formal Incident Response capability, including:

- An Incident Response Team
- A communication process
- A severity model
- Response steps for common cyber incidents
- Tools and logs for detection
- Containment and mitigation procedures

## Purpose of the Playbook

This playbook explains what the security team should do when a cyber event or incident occurs.

It helps the team:

- Identify incidents quickly
- Decide severity
- Communicate with the right people
- Contain the incident
- Preserve evidence
- Recover safely
- Document lessons learned

## Incident Response Phases

This playbook follows a NIST-style incident response process:

1. Preparation
2. Detection and Analysis
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

## Incident Response Team Roles

| Role | Responsibility |
| --- | --- |
| CISO / Incident Response Manager | Leads the response, briefs executives, approves major decisions |
| Security Analyst | Reviews alerts, logs, network activity, and suspicious behavior |
| Forensics Analyst | Preserves and analyzes digital evidence |
| IT/System Administrator | Isolates systems, resets accounts, patches devices, restores services |
| Communications Officer | Handles internal updates, executive communication, and user notices |
| Legal/Compliance Contact | Reviews regulatory, legal, and reporting requirements |

## Severity Model

| Severity | Description | Example | Response |
| --- | --- | --- | --- |
| Low | Limited issue with no confirmed compromise | Suspicious email reported but not clicked | Document and monitor |
| Medium | Possible compromise or limited exposure | User clicked phishing link but no confirmed lateral movement | Investigate, reset password, monitor account |
| High | Confirmed compromise or sensitive data risk | Stolen credentials used to access systems | Contain, escalate, preserve evidence |
| Critical | Major business impact or active attack | Ransomware, data exfiltration, DDoS affecting services | Activate full IR team and executive response |

## Communication Tree

During an incident, communication should follow this path:

1. User or monitoring tool reports suspicious activity.
2. Security Analyst performs initial triage.
3. Incident Response Manager reviews severity.
4. IT/System Administrator performs technical containment.
5. CISO or IR Manager briefs executive leadership.
6. Communications Officer prepares user or customer messaging if needed.
7. Legal/Compliance reviews reporting requirements.

## Playbook 1: Phishing Incident

### Identification

- Review the reported email.
- Check sender address, links, attachments, and message content.
- Ask whether the user clicked the link or entered credentials.
- Search for similar emails sent to other users.

### Containment

- Block the sender, domain, or malicious URL.
- Remove similar emails from user inboxes if possible.
- Reset the affected user's password.
- Revoke active sessions.
- Enable or verify MFA.
- Monitor the account for unusual activity.

### Evidence to Collect

- Original email
- Email headers
- Sender address
- URLs and attachments
- User actions
- Login history
- Related alerts

### Recovery

- Confirm the account is secured.
- Restore normal access only after verification.
- Educate the user on phishing indicators.
- Update email filtering rules.

## Playbook 2: Credential Theft

### Identification

- Review failed and successful login attempts.
- Look for logins from unusual locations or devices.
- Check whether credentials were entered into a phishing page.
- Review account activity after the suspected compromise.

### Containment

- Reset password.
- Revoke sessions and tokens.
- Disable the account temporarily if needed.
- Require MFA enrollment.
- Review permissions and access history.

### Recovery

- Restore access after the account is verified secure.
- Monitor for repeat login attempts.
- Document the incident timeline.

## Playbook 3: Malware Discovery

### Identification

- Review suspicious processes.
- Check unusual files or services.
- Compare running processes against expected system behavior.
- Use endpoint tools to validate findings.

### Static Analysis

- Review file name, hash, location, and metadata.
- Check indicators of compromise.
- Do not execute the file during static analysis.

### Dynamic Analysis

- Analyze malware behavior only in a controlled lab or sandbox.
- Observe network connections, file changes, and process activity.

### Containment

- Isolate the infected system from the network.
- Preserve evidence before cleaning.
- Block malicious indicators.
- Reimage the system if needed.

## Playbook 4: Ransomware

### Identification

- Look for encrypted files.
- Review ransom notes.
- Check abnormal file changes.
- Identify affected systems and shared drives.

### Containment

- Disconnect affected systems from the network.
- Disable compromised accounts.
- Block suspicious network traffic.
- Stop spread to shared resources.

### Recovery

- Restore from clean backups.
- Rebuild affected systems.
- Validate that ransomware is removed.
- Review backup and patching gaps.

## Playbook 5: DDoS Attack

### Identification

- Monitor unusual traffic spikes.
- Check service availability.
- Identify affected systems or websites.
- Review firewall, IDS, and network logs.

### Containment and Mitigation

- Contact internet service provider or DDoS protection provider.
- Block or rate-limit malicious traffic where possible.
- Prioritize critical services.
- Communicate service status to leadership.

### Recovery

- Confirm services are stable.
- Review traffic patterns.
- Update DDoS response procedures.

## Playbook 6: Physical Security Incident

### Identification

- Report unauthorized access to restricted areas.
- Review camera footage and access logs.
- Identify missing equipment or documents.

### Controls

- Physical controls: locked server rooms, access cards, visitor logs.
- Deterrent controls: cameras, alarms, warning signs.
- Preventive controls: biometric readers, locked cabinets, secure document destruction.

### Response

- Restrict access immediately.
- Preserve access logs and video evidence.
- Notify management and security personnel.
- Review whether cyber systems may also be affected.

## Tools and Logs

Useful tools and logs for this playbook include:

- Nmap
- Incident response scripts
- `netstat -ano`
- `tasklist`
- Malwarebytes
- Endpoint detection tools
- Firewall logs
- Authentication logs
- Email security logs
- VPN logs
- IDS/IPS alerts

## Containment and Mitigation Steps

Common containment actions include:

- Isolating infected systems
- Blocking malicious IP addresses or domains
- Resetting passwords
- Revoking user sessions
- Disabling compromised accounts
- Applying security patches
- Removing malicious emails
- Preserving evidence before system changes

## Lessons Learned

After each incident, the team should document:

- What happened
- How it was discovered
- What systems or users were affected
- What response actions were taken
- What worked well
- What needs improvement
- What controls should be added or changed

## What I Learned

This project helped me understand that incident response is both technical and organizational.

A strong playbook must include technical steps, team roles, communication, severity levels, evidence handling, and executive decision-making.
