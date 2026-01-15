# FUTURE_CS_01
Conduct security testing on a sample web application to identify vulnerabilities like SQL injection, XSS, and authentication flaws.

## Cyber Security Internship – Task 1

### Web Application Security Testing

## 📌 Overview

This repository contains my submission for **Task 1 of the Cyber Security Internship**, focused on **Web Application Security Testing**. The task involved analyzing a deliberately vulnerable web application to understand how common security vulnerabilities are identified using both **manual testing techniques** and **automated security tools**.

The primary goal of this task was to gain hands-on experience with real-world web security testing methodologies and develop an understanding of how insecure coding practices and misconfigurations can expose applications to potential attacks.

---

## 🎯 Objective

The main objectives of this task were to:

* Understand the fundamentals of **web application security testing**
* Identify and analyze common web vulnerabilities such as:

  * SQL Injection (SQLi)
  * Cross-Site Scripting (XSS)
  * Security misconfigurations
* Gain practical experience with industry-standard security testing tools
* Learn how security headers and configurations impact application security

---

## 🛠️ Tools & Technologies Used

* **OWASP Juice Shop** – Vulnerable web application used for testing
* **OWASP ZAP (Zed Attack Proxy)** – Automated web security scanner
* **Docker** – Used to deploy the vulnerable application locally
* **Web Browser** – Manual testing and payload injection

---

## 🔍 Testing Methodology & Findings

### 1️⃣ SQL Injection Testing

* The login functionality was tested using common SQL Injection payloads.
* The application successfully detected and blocked the malicious inputs.
* This demonstrates how proper input validation and defensive mechanisms can prevent authentication bypass attacks.
* The test highlights the importance of secure query handling and backend validation.

---

### 2️⃣ Cross-Site Scripting (XSS) Testing

* XSS payloads were injected through the search functionality.
* The injected scripts were not executed.
* This indicates that user inputs were being sanitized or properly encoded.
* The test emphasizes the role of input filtering in preventing client-side attacks.

---

### 3️⃣ OWASP ZAP Automated Scan

An automated vulnerability scan was conducted using **OWASP ZAP** against the application running locally at:

```
http://localhost:3000
```

#### ⚠️ Identified Issues:

* **Content Security Policy (CSP) Header Not Set**
* **Information Disclosure**
* **Cross-Domain Misconfiguration**

These findings are primarily related to missing security headers and weak security configurations, which could potentially be exploited if left unaddressed.

---

## 📂 Repository Structure

```
├── Report/
│   └── Web_Application_Security_Testing_Report.pdf
├── Screenshots/
│   └── Evidence of manual testing and OWASP ZAP scan results
└── README.md
```

* **Report Folder**: Contains a detailed security testing report
* **Screenshots Folder**: Includes screenshots as proof of testing activities and scan findings

---

## ✅ Conclusion

This task provided valuable practical exposure to **web application vulnerability assessment** using both **manual testing techniques** and **automated security tools**. It reinforced key concepts such as:

* The importance of secure input handling
* The role of security headers in protecting web applications
* How misconfigurations can lead to potential security risks
* The effectiveness of combining manual testing with automated scans

Overall, this task strengthened my foundational understanding of web application security and highlighted best practices in secure web development.

---

## 🏁 Status

✔ **Task 1 Successfully Completed**


