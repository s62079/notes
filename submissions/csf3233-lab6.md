#cybersec

<div style="page-break-before: always">S62079</div>

## TASK 1: RUNNING GREEN BONE SECURITY MANAGER (GSM)

![](20231206090951.png)

![](20231206090933.png)

![](20231206091028.png)

![](20231206091247.png)

![](20231206091230.png)

## TASK 2: SETTING UP THE NETWORK FOR METASPLOITABLE

![](20231206092331.png)

<div style="page-break-before: always">S62079</div>

## TASK 3: SCANNING THE VULNERABILITIES IN METASPLOITABLE

![](20231206100539.png)

![](20231206100625.png)

what a dangerous machine

<div style="page-break-before: always">S62079</div>

1. Referring to the result of the scanning, complete the table of the severity class below: 
2. What are vulnerabilities that have the highest severities? List them. 
3. What is the vulnerability for port 513/tcp? 
4. List three (3) vulnerabilities with medium severity. 
5. Based on the given information by GSM, how do we solve the “VNC Brute Force” vulnerability?

---

1. here

| severity | total |
| :-: | :-: | 
| high | 25 | 
| medium | 39 | 
| low | 6 | 
| log | 91 |
| grand total | 145 | 

2. critical
	- `Distributed Ruby (dRuby/DRb) Multiple Remote Code Execution Vulnerabilities`
	- `TWiki XSS and Command Execution Vulnerabilities`
	- `Operating System (OS) End of Life (EOL) Detection`
3. `rlogin Passwordless Login`
4. medium
	- `Multiple Vendors STARTTLS Implementation Plaintext Arbitrary Command Injection Vulnerability`
	- `TWiki Cross-Site Request Forgery Vulnerability`
	- `Anonymous FTP Login Reporting`
5. as such
![](20231206101832.png)

<div style="page-break-before: always">S62079</div>

1. In your own words, explain about Common Vulnerability Scanning System (CVSS) and Common Vulnerability Enumeration (CVE). 
2. Explain the difference(s) between CVSS and CVE. 
3. How many severity levels are there in the CVSS version 3.0? 
4. Draw a table of CVSS3.0 severity levels and their base score range. 
5. Observe the information provided at vuldb.com and answer the questions below: 
	1. List three (3) most recent vulnerabilities and their severities. 
	2. List three (3) latest available exploits. 
	3. List three (3) vulnerabilities in current CVSS Top 5.

---

1. CVSS is a scoring system for a vulnerability based on multiple factors, while CVE is an identifier for a vulnerability for better classification
2. CVSS is the score, CVE is the identifier, codename, description, yada yada. 
3. 5
4. here

| score range | severity |
| :-: | :-: |
| 0 | none |
| 0.1 - 3.9 | low |
| 4.0 - 6.9 | medium | 
| 7.0 - 8.9 | high |
| 9.0 - 10.0 | critical |

<div style="page-break-before: always">S62079</div>

### question 5

too long

1. 3 most recent ![](20231206102350.png)![](20231206102436.png)![](20231206102454.png)
2. 3 exploitable ![](20231206102602.png)![](20231206102626.png)![](20231206102733.png)

3. 3 top 5
	- `Unitronics Vision Series PLC all insecure default initialization of resource`
	- `Zyxel NAS326/NAS542 WSGI Server os command injection`
	- `Zyxel NAS326/NAS542 HTTP POST Request show_zysync_server_contents os command injection` 