# networkwalks-B082-week4-Capstone-Project
## Penetration Testing Report for Mediroza General Hospital

### Web Application Security Assessment

<div align="center">

| **Batch** | **B082** |
| :--- | :--- |
| **Name** | **Iyaloo Shivute** |
| **Program** | Cybersecurity Training at Networkwalks Academy |
| **Milestones successfully completed** | M1, M2, M3 & M4 |

</div>

## 📌 1. Executive Summary
In this lab, I was given the task of performing a black-box penetration test on Mediroza General Hospital's website at https://medirozahospital.com. This assessment was authorized in writing by the customer. The objective was to find weaknesses, show how they could be exploited in the real world, and offer recommendations for strengthening the organization's security posture.

Several vulnerabilities ranging in severity from medium to critical were found throughout the testing process. The most important discovery was that the patient portal login page had a SQL injection vulnerability that let me entirely bypass authentication without knowing any credentials. I was able to see three confidential patient lab report PDFs as a result. I found crucial metadata in one of the files that led to a forgotten database backup stored in a publicly accessible directory on the server after using password cracking software to break the PDF encryption. Ten shareholders' shareholding information and the monthly wages of all thirty-hospital staff were included in this backup.

The target's overall security posture is subpar. With little effort and no specialized equipment, an unauthenticated attacker could access sensitive patient data, employee financial records, and corporation ownership information due to a number of serious vulnerabilities.
 

## 📌 2. Scope and Methodology
### 2.1  Scope
As agreed, upon with the client, the assessment was restricted to the following target domain:  https://medirozahospital.com
The Social engineering, denial-of-service attacks, and any testing outside the designated domain were not included in the scope.

### 2.2  Methodology
**I used a four-phase, organized black-box penetration testing process.** <br><br>
	**Reconnaissance:** Passive information collection using web-based resources and publicly accessible data. <br><br> 
	**Vulnerability Identification:** Examining the behavior of the program to identify input handling and authentication flaws.<br><br>
	**Exploitation:** Using controlled exploitation to show the true impact of each vulnerability.<br><br>
	**Documentation:** Including all conclusions, supporting data, and recommendations for corrective action in this report.


## 📌 3. Tools utilized

The tools used and their functions are listed in the table below:


| Tool used| Function/Purpose |
| :--- | :--- |
| **Kali Linux & Windows** | Operating systems used for reconnaissance activities |
| **Browser developer tools** | To examine the behavior of login forms and page sources |
| **wget** | To download files from the web server. |
| **Networkwalks Hash Calculator** | For extracting password hashes from PDF files. |
| **Networkwalks Password Cracker** | Uses wordlists to crack PDF password hashes. |
| **curl -I** | A command-line utility for reading web server responses and submitting HTTP requests. |
| **gpdf** | To decrypt password-protected PDF files following cracking. |
| **exiftool** | To reading hidden metadata from PDF files. |
| **ChatGPT** | To transform unprocessed SQL data into comprehensible tables. |

---

## 📌 4. Target Files

| File | Password cracked | Status |
| :--- | :--- | :--- |
| patient_report_1.pdf  | 123456 | Password successfully cracked ✅|
| patient_report_2.pdf | password | Password successfully cracked ✅ |
| patient_report_3.pdf | !@#$%^& | Password successfully cracked ✅ |

---


## 📌 5. Findings and Proof of Exploitation 

### Summary Table
I identified the following vulnerabilities based on the data gathered during reconnaissance and footprinting activities.

<img width="1180" height="328" alt="image" src="https://github.com/user-attachments/assets/55536166-3483-48e1-909e-b0e52d8a8c27" />


### _The detailed Report for Week 4: Penetration Testing for Mediroza General Hospital is attached in the repository_. 

## 📌 6. Conclusion
A full attack chain from the login page to extremely sensitive internal data was discovered during this assessment. There was no need for advanced tool or expertise. Every vulnerability identified in this research is well-known and has established remedies. Before the system is utilized to store or provide actual patient data, I recommend the client to address all Critical and High findings immediately.

Moreover, this lab made it easier for me to comprehend how password cracking works and why it's crucial to use strong passwords for security. I also discovered that short or common passwords are easily cracked, which further highlights the need for strong passwords.


## 📌 7. Evidences
### _Logged in into the patient portal_
<img width="1050" height="560" alt="image" src="https://github.com/user-attachments/assets/e1b422cf-533c-4409-8c69-482890d5e13a" />

## _Milestone 1 successfully achieved._

<img width="479" height="342" alt="image" src="https://github.com/user-attachments/assets/5bd507d1-4d9f-4a9d-ae63-aea99814dab0" />

_Downloaded the three PDF files with patient records._

### _Results for patient_report_1.pdf
<img width="602" height="377" alt="image" src="https://github.com/user-attachments/assets/664df2ea-90d8-467d-a6e6-ad10d0ea5bac" />

### _Results for patient_report_2.pdf
<img width="602" height="373" alt="image" src="https://github.com/user-attachments/assets/b7a1f373-99b2-4a08-ad29-88aadf332785" />

### _Results for patient_report_3.pdf
<img width="602" height="360" alt="image" src="https://github.com/user-attachments/assets/eb04c724-546d-417c-ae1f-12d9cfb8eae6" />

## _Milestone 2 successfully achieved._

<img width="634" height="255" alt="image" src="https://github.com/user-attachments/assets/25a26b0d-d070-4b18-bad0-3daf62325a8f" />

<img width="560" height="632" alt="image" src="https://github.com/user-attachments/assets/ad3a3aeb-bfcf-4f96-a64b-4f6c37642f0d" />

## _Milestone 3 successfully achieved._

<br><br>
### 👤 Submitted by: Iyaloo Shivute
### 👤 Cybersecurity Mentor: Waqas Karim, CCIE

### **Organisation:** Networkwalks
### Batch B082 | Week 4 Capstone Project
LinkedIn:  www.linkedin.com/in/iyaloo-shivute

## 📌 Project Information
**Program Name**: Cybersecurity at Networkwalks | **Week**: 04 | **Project**: Penetration Testing _ Mediroza General Hospital  | **Repository**: GitHub
