<h1 align="center">☁️ AWS Cloud Security Lab</h1>

<p align="center">
Simulating a real-world cloud breach: credential compromise → reconnaissance → privilege escalation → persistence → data exposure
</p>

---

## 📖 Overview

This project simulates a **real-world AWS cloud security incident** where an attacker gains access to compromised IAM credentials and performs API-based reconnaissance, privilege escalation, and persistence.

The lab focuses on **detection, investigation, and security analysis** using AWS CloudTrail and Splunk, while mapping attacker behavior to MITRE ATT&CK and security frameworks.

---

## 🎯 Objectives

- Simulate a cloud attack lifecycle using AWS
- Analyze CloudTrail logs for attacker behavior
- Identify IAM abuse and misconfigurations
- Demonstrate detection engineering concepts
- Map activity to MITRE ATT&CK, NIST, and CIS

---

## 🧠 Skills Demonstrated

- AWS IAM & access control
- CloudTrail log analysis
- API-based attack simulation (AWS CLI)
- Detection thinking (SOC / IR mindset)
- Cloud misconfiguration analysis
- MITRE ATT&CK mapping
- NIST & CIS control mapping
- Splunk log analysis

---

## 🏗️ Lab Architecture
Kali Linux (Attacker)
↓
AWS (IAM, S3, CloudTrail)
↓
CloudTrail Logs (S3)
↓
Splunk (SIEM)
↓
Detection & Investigation


---

## ⚔️ Attack Scenario

> An IAM user's access keys were compromised (simulated phishing exposure).  
> The attacker used these credentials from an external system to enumerate resources, identify weaknesses, and attempt privilege escalation.

---

## 🔄 Attack Lifecycle

| Phase | Description |
|------|------------|
| 🟢 Initial Access | Compromised IAM credentials |
| 🔍 Reconnaissance | API enumeration via AWS CLI |
| 🔺 Privilege Escalation | Abuse of IAM misconfigurations |
| 🔁 Persistence | Creation of new access paths |
| 📂 Impact | S3 exposure / data access |

---

## 📂 Project Structure


aws-cloud-security-lab/
├── README.md
├── screenshots/
├── initial-access-recon/
├── privilege-escalation/
├── persistence/
├── s3-exposure/
├── detections/
└── mappings/


---

## 🧪 Lab Environment

- **Attacker:** Kali Linux  
- **SIEM:** Splunk (Ubuntu VM)  
- **Cloud:** AWS Free Tier  
- **Services:** IAM, S3, CloudTrail  

---

## 🧾 Evidence & Artifacts

- CloudTrail event logs (JSON)
- AWS CLI attack activity
- IAM configurations
- AccessDenied events (critical detection signal)
- Splunk queries and detections

---

## 🎯 MITRE ATT&CK Coverage

- Valid Accounts
- Account Discovery
- Cloud Service Discovery
- Account Manipulation

---

## 🛡️ Security Framework Alignment

- :contentReference[oaicite:0]{index=0} (NIST)
- :contentReference[oaicite:1]{index=1} (CIS Controls)

---

## 🚀 Status

✅ AWS environment configured  
✅ CloudTrail logging enabled  
✅ IAM attacker user created  
✅ Initial API activity generated  

🔄 Next: Initial Access & Recon documentation → Privilege Escalation

---

## 💼 Why This Project Matters

This lab demonstrates **real-world cloud attack simulation and detection**, aligning with responsibilities of:

- SOC Analyst  
- Incident Responder  
- Cloud Security Analyst  

---

<p align="center">🔥 Built for practical, real-world cloud security skills</p>
