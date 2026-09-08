# Week-4-Internship-Update-Penetration-Testing-Engagement-Mediroza-General-Hospital
🔐 Mediroza Hospital – Penetration Testing & Security Assessment

«Educational / Authorized Security Assessment»

A controlled penetration-testing project focused on assessing web application security, authentication controls, data exposure, database security, and password/hash protection in an authorized assessment environment.

---

📌 Project Overview

This project documents a structured penetration-testing assessment performed against the Mediroza Hospital web application environment.

The assessment was divided into multiple milestones to understand how weaknesses in authentication, access control, exposed resources, database protection, and password security could affect the confidentiality and integrity of sensitive information.

All testing was performed within an authorized and controlled scope.

---

🎯 Objectives

The primary objectives of this assessment were:

- Identify weaknesses in web application authentication.
- Evaluate access-control mechanisms.
- Assess potential sensitive-data exposure.
- Identify risks associated with exposed database resources or backups.
- Analyze password and hash-storage security.
- Document evidence for each assessment milestone.
- Classify findings according to security impact.
- Provide practical remediation recommendations.

---

🧪 Assessment Methodology

The assessment followed a structured workflow:

Reconnaissance
      ↓
Application Analysis
      ↓
Authentication Assessment
      ↓
Data Exposure Assessment
      ↓
Database Security Assessment
      ↓
Password / Hash Security Assessment
      ↓
Risk Analysis
      ↓
Remediation Recommendations
      ↓
Final Report

---

📂 Assessment Milestones

M1 – Initial Access

Focus:

- Authentication workflow analysis
- HTTP request/response inspection
- Access-control validation
- Controlled testing of application inputs
- Evidence collection

Objective: Determine whether authentication or input-handling weaknesses could result in unauthorized access.
<img width="1920" height="982" alt="login" src="https://github.com/user-attachments/assets/f3de8ec8-46ef-4bdc-a3c8-131aa6b868a0" />

---

M2 – Data Extraction / Exposure

Focus:

- Application data-access review
- Sensitive-data exposure assessment
- Authorization boundary validation
- Evidence collection

Objective: Determine whether application weaknesses could expose information outside the intended authorization boundary.

«Sensitive patient information is intentionally excluded/redacted from this repository.»
<img width="1920" height="982" alt="pdf1_pass" src="https://github.com/user-attachments/assets/2ea87e46-c6c7-49be-a8ff-fbb9908484b6" />
<img width="1920" height="982" alt="pdf2" src="https://github.com/user-attachments/assets/403d287d-3df3-44e1-9067-11e17ff1bfc8" />
<img width="1920" height="982" alt="pdf2_pass" src="https://github.com/user-attachments/assets/fbe73469-0fb5-4a6a-ab56-4957d3822e8e" />
<img width="1920" height="982" alt="pdf3" src="https://github.com/user-attachments/assets/fea378d1-7db0-4d34-91d9-0fac81ea59d0" />
<img width="1920" height="982" alt="pdf3_pass" src="https://github.com/user-attachments/assets/aac07b9a-cf3d-40d3-b7f4-884e3e2d2b12" />


---

M3 – Database Exposure

Focus:

- Database exposure assessment
- Publicly accessible database artifacts/backups
- Database structure review
- Security-impact analysis

Objective: Evaluate the potential impact of exposed database resources and determine whether they could lead to unauthorized access to sensitive application information.

«Database records, credentials and other sensitive information are not published in this repository.»![Uploading pdf1.png…]()
<img width="911" height="291" alt="M3-share-holders" src="https://github.com/user-attachments/assets/137b1f49-de8f-4740-9f9b-a97648acbd9a" />


---

M4 – Password & Hash Security Assessment

Focus:

- Hash-format identification
- Password-storage assessment
- Controlled password-recovery testing
- Password-strength evaluation
- Credential-security analysis

Objective: Determine whether password protection mechanisms provide adequate resistance against credential compromise.

Actual passwords and recoverable credential values are not included in this repository.

---

🛠️ Tools Used

Tool / Technique| Purpose
Burp Suite| HTTP traffic inspection and web application testing
Web Browser| Application analysis and validation
SQL Injection Testing| Input-handling and database-security assessment
Hash Identification| Identify password/hash formats
John the Ripper| Controlled password-recovery testing
Networkwalks Security Tools| Hash analysis and security assessment
Screenshot Capture| Evidence collection and documentation

---

📊 Risk Summary

Finding| Severity| Potential Impact
Authentication / Access-Control Weakness| 🔴 High| Unauthorized access to protected functionality
Sensitive Data Exposure| 🔴 Critical| Disclosure of sensitive information
Database Exposure| 🔴 Critical| Database compromise and large-scale information disclosure
Weak Password / Hash Protection| 🔴 High| Credential compromise and possible account takeover

---

🔍 Key Security Observations

The assessment highlighted several areas requiring security attention:

1. Authentication Security
   
   - Authentication controls should be validated server-side.
   - Strong access-control enforcement should be implemented.

2. Sensitive Data Protection
   
   - Sensitive application information should only be accessible to authorized users.
   - Data exposure should be minimized.

3. Database Security
   
   - Database backups and sensitive database artifacts should never be publicly accessible.
   - Database permissions should follow the principle of least privilege.

4. Password Security
   
   - Passwords should never be stored in plaintext.
   - Modern adaptive password-hashing algorithms should be used.
   - MFA and rate-limiting controls should be considered.

---

🛡️ Recommendations

Authentication

- Implement strong server-side authentication.
- Enforce proper authorization checks.
- Implement rate limiting.
- Consider multi-factor authentication.
- Monitor repeated authentication failures.

Database

- Remove database backups from publicly accessible directories.
- Restrict database permissions.
- Rotate exposed credentials.
- Regularly audit backup storage locations.

Password Security

- Use modern adaptive password hashing.
- Use unique salts for password hashes.
- Enforce appropriate password policies.
- Implement MFA for sensitive accounts.
- Monitor suspicious authentication activity.

Web Application

- Use parameterized queries/prepared statements.
- Validate and sanitize server-side inputs.
- Apply least-privilege access control.
- Maintain secure configuration management.
- Perform regular vulnerability assessments.

---

```📁 Repository Structure

mediroza-hospital-pentest/
│
├── README.md
├── REPORT.md
│
├── Evidence/
│   ├── M1-Initial-Access/
│   │   ├── login.png
│   │   └── initial_access.png
│   │
│   ├── M2-Data-Extraction/
│   │   ├── evidence-01.png
│   │   └── evidence-02.png
│   │
│   ├── M3-Database-Exposure/
│   │   ├── database-evidence.png
│   │   └── exposure.png
│   │
│   └── M4-Password-Assessment/
│       ├── hash-analysis.png
│       └── password-assessment.png
│
└── Documentation/
    └── Penetration-Testing-Report.docx

```

📄 Documentation

The complete assessment report contains:

- Introduction
- Scope and Rules of Engagement
- Tools Used
- M1–M4 Activities
- Risk Analysis
- Recommendations
- Conclusion
- Evidence References

---

⚠️ Disclaimer

This repository is intended only for authorized cybersecurity education, research, and security assessment.

Do not use the techniques, tools, evidence, credentials, or information contained in this project against systems without explicit authorization.

Sensitive information has been redacted or omitted from the public documentation.

The author assumes no responsibility for unauthorized or illegal use of the information contained in this repository.

---

👤 Author

Shahzeb Hassan 

Cybersecurity Student
Cybersecurity / Ethical Hacking Project

---

📚 Project Classification

Project Type: Penetration Testing
Domain: Cybersecurity
Assessment: Web Application & Password Security
Environment: Authorized / Controlled
Milestones: M1 – M4
Purpose: Educational and Security Assessment
