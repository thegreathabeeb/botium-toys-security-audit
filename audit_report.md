# Security Audit Report – Botium Toys  

## 1. Introduction  
Botium Toys is a mid-sized toy company handling customer data, including payment information and personally identifiable information (PII/SPII).  
This audit, conducted as part of the Google Cybersecurity Fundamentals course, assesses the company's security posture, identifies gaps, and provides actionable recommendations.  

---

## 2. Scope  
The audit focused on:  
- Data protection and confidentiality  
- Access controls and user permissions  
- Network and system security  
- Disaster recovery and business continuity  
- Physical security  

---

## 3. Findings  

### 3.1 Access Management  
- All employees currently have access to internally stored data, including potential access to cardholder data and customers’ PII/SPII.  
- Access controls related to least privilege and separation of duties have not been implemented.  

### 3.2 Data Protection & Encryption  
- Customer credit card information is accepted, processed, transmitted, and stored locally without encryption.  
- Although privacy policies and procedures exist, there is no technical enforcement of data confidentiality.  

### 3.3 Authentication & Password Policies  
- A password policy exists but does not meet current minimum complexity requirements (e.g., eight characters, combination of letters, numbers, and special characters).  
- No centralized password management system is in place, causing productivity issues when password resets are requested.  

### 3.4 System & Network Security  
- Firewalls are in place with defined security rules.  
- Antivirus software is installed and monitored regularly.  
- No intrusion detection system (IDS) is currently installed.  
- Legacy systems are monitored inconsistently, with unclear intervention schedules.  

### 3.5 Disaster Recovery & Backups  
- No disaster recovery plans exist.  
- Critical data is not backed up, leaving the company vulnerable to data loss.  

### 3.6 Regulatory & Privacy Compliance  
- IT department has a plan to notify EU customers within 72 hours in case of a security breach.  
- Privacy policies, procedures, and processes are enforced and properly documented.  

### 3.7 Physical Security  
- Main office, store front, and warehouse have proper locks, up-to-date CCTV surveillance, and functioning fire detection and prevention systems.  
- Physical security controls are adequate and regularly monitored.  

---

## 4. Recommendations  

1. **Access Controls**:  
   - Implement least privilege and separation of duties to limit exposure of sensitive data.  

2. **Data Encryption**:  
   - Encrypt credit card information and sensitive PII/SPII at rest and in transit.  

3. **Authentication & Password Management**:  
   - Enforce strong password policies (minimum 8–12 characters, mix of letters, numbers, special characters).  
   - Deploy a centralized password management system to streamline password resets.  

4. **Network & System Security Enhancements**:  
   - Install an intrusion detection system (IDS).  
   - Establish a scheduled monitoring and maintenance plan for legacy systems.  

5. **Disaster Recovery & Backups**:  
   - Create and implement a disaster recovery plan.  
   - Ensure critical data is regularly backed up and tested.  

6. **Continuous Training & Awareness**:  
   - Conduct regular cybersecurity awareness training for all employees.  

---

## 5. Evidence (Sample)  

- [weak-password.png](EVIDENCE/weak-password.png) → Example of weak password accepted  
- [open-data-access.png](EVIDENCE/open-data-access.png) → Screenshot showing all employees have access to sensitive data  
- [firewall-status.png](EVIDENCE/firewall-status.png) → Firewall configuration screenshot  

---

## 6. Conclusion  
Botium Toys has some strong foundational security measures (firewall, antivirus, physical security, privacy policies), but significant gaps exist in **access management, encryption, disaster recovery, and authentication**.  

Implementing the recommendations above will improve data confidentiality, system integrity, and overall cybersecurity resilience.
