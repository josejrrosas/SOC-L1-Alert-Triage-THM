# SOC L1 Alert Triage – TryHackMe Case Study  

## Objective  

This project was focused on learning the fundamentals of **alert triage** from the perspective of a SOC Level 1 analyst. The lab simulated incoming alerts inside a SIEM-like environment, requiring review, enrichment, and classification. The goal was to practice making quick decisions on whether alerts were false positives or true positives, and documenting reasoning for potential escalation.  

---

### Skills Learned  

- Practical experience with the SOC L1 alert triage workflow.  
- Reviewing alert metadata (source IPs, timestamps, usernames, severity).  
- Performing IOC enrichment using tools like VirusTotal and AbuseIPDB.  
- Differentiating between false positives and true positives with proper justification.  
- Writing concise escalation notes for L2 handoff.  
- Strengthening critical thinking and decision-making in a SOC environment.  

---

### Tools Used  

- SIEM-style dashboards provided within the TryHackMe lab.  
- External enrichment tools:  
  - VirusTotal  
  - WHOIS  
  - AbuseIPDB  
- Basic log analysis and alert correlation techniques.  

---

## Steps  

Below are the key steps and screenshots from the triage process.  

### Step 1 – Reviewing the Alert  
Checked the alert metadata in the SIEM dashboard. Looked at source IP, destination, severity, and login activity.  

*Ref 1: Initial alert details*  
<img width="2746" height="1688" alt="image" src="https://github.com/user-attachments/assets/daf7dd81-b15a-416d-a439-d13089df335a" />


### Step 2 – IOC Enrichment  
Took the suspicious IP and ran it through VirusTotal. Determined whether it had a reputation for malicious activity.  

*Ref 2: VirusTotal IP lookup*
<img width="3340" height="1814" alt="image" src="https://github.com/user-attachments/assets/8996173c-72d9-4429-bd4d-7be891c36cc4" />
  

### Step 3 – Log Correlation  
Cross-checked the alert against system logs to confirm whether the login attempts matched expected user behavior.  

*Ref 3: Log correlation results (screenshot here)*  

### Step 4 – Classification and Escalation  
Marked the alert as a **true positive** due to confirmed malicious IP combined with abnormal login activity. Documented reasoning and prepared notes for escalation to L2.  

*Ref 4: Escalation notes in SIEM (screenshot here)*  

---

## Example Detections  

- **IP-based IOC**: Outbound traffic to a known malicious C2 server.  
- **Domain-based IOC**: Login attempts tied to a newly-registered suspicious domain.  
- **Host Artifact**: Unusual process execution pattern (Word → PowerShell).  
- **Network Artifact**: Rare User-Agent string observed in HTTP POST requests.  

---

## Lessons Learned  

- Not every alert is worth escalating — context is key.  
- Enrichment is essential to avoid wasting time on false positives.  
- Having a consistent workflow (Review → Enrich → Decide → Escalate) keeps triage efficient and repeatable.  
- Documentation of reasoning is just as important as detection.  

---
