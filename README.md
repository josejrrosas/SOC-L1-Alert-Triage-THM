# SOC L1 Alert Triage – TryHackMe Case Study  

## 🔍 Objective  

This project was focused on learning the fundamentals of **alert triage** from the perspective of a SOC Level 1 analyst. The TryHackMe lab simulated incoming alerts in a SIEM-like environment and required me to review, prioritize, and make decisions on each ticket. The primary goal was to practice the Tier 1 SOC workflow of analyzing alerts, deciding whether to escalate or close them, and documenting reasoning clearly.  

---

## 🛠️ Skills Learned  

- Understanding the relationship between **events** and **alerts** inside a SIEM.  
- Interpreting **alert properties** (status, severity, assignee, verdict).  
- Applying **alert prioritization rules** (oldest first, medium > low severity).  
- Triaging alerts systematically and making escalation vs. closure decisions.  
- Practicing structured, repeatable SOC L1 workflows.  
- Reinforcing documentation habits in ticketing systems.  

---

## ⚙️ Tools Used  

- TryHackMe’s simulated SIEM dashboard  
- Basic alert fields and filtering functions (status, severity, timestamps)  
- No external enrichment tools in this room — focus was on workflow and prioritization  

---

## 📂 Process  

### Task 1 – Introduction  
Reviewed the simulated SOC ticket queue in TryHackMe’s SIEM. Objective: work through alerts, analyze issues, and either escalate or close them.  

### Task 2 – Events vs. Alerts  
Learned the difference between raw **events** (all logged activity) and **alerts** (filtered, rule-based triggers for suspicious activity).  

### Task 3 – Alert Properties  
Explored the SIEM alert columns: **status, name, verdict, severity, assignee, timestamp,** etc. Understood how these fields drive triage decisions.  

### Task 4 – Alert Prioritization  
Practiced prioritizing tickets:  
- Handle oldest alerts first.  
- Medium-severity alerts should be addressed before low-severity ones.  

### Task 5 – Alert Triage  
Worked through tickets one by one, analyzing context, then either **closing false positives** or **escalating true positives**. Learned the importance of making consistent, documented decisions.  

### Task 6 – Final Review  
Completed triage of the ticket queue, confirming understanding of the workflow and ensuring proper closure or escalation for all assigned alerts.  

---

## 🛡️ Example Takeaways from Triage  

- **Low-severity alert**: Closed after confirming expected behavior.  
- **Medium-severity alert**: Escalated when context suggested abnormal or potentially malicious activity.  
- **SIEM status fields**: Used to track progress and accountability across the SOC team.  

---

## 🧠 Lessons Learned  

- SOC L1 work is **pattern recognition and decision discipline** — you need to follow a repeatable process to avoid mistakes.  
- Not every alert is actionable; triage is about separating noise from signals.  
- Prioritization rules (oldest first, medium > low) help keep queues manageable.  
- Documentation of *why* an alert was closed or escalated is critical for SOC communication.  

---

## 🚀 Next Steps  

- Apply the same workflow to more complex labs with external enrichment.  
- Practice documenting triage decisions as if writing real SOC tickets.  
- Expand into L2 tasks: correlating multiple alerts, mapping activity to MITRE ATT&CK.  

---

## 📄 References  

- [TryHackMe: SOC L1 Alert Triage](https://tryhackme.com/room/socl1alerttriage)  
