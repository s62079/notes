#cybersec

<div style="page-break-before: always">S62079</div>

## TASK 1: DISCOVERING FILE UPLOAD VULNERABILITIES

![](20240102235450.png)

![](20240102235728.png)

![](20240103000029.png)

<div style="page-break-before: always">S62079</div>

## TASK 2: DISCOVERING CODE EXECUTION VULNERABILITIES

![](20240103000436.png)

![](20240103000527.png)

![](20240103000618.png)

remote hijack, cool

<div style="page-break-before: always">S62079</div>

## TASK 3: DISCOVERING SQL INJECTION VULNERABILITIES

![](20240103001212.png)

![](20240103001400.png)

1. What is the table name for keeping the user details? 
`Account`
2. What are the fields of the identified table?
`username`, `password`, `signature`

![](20240103001605.png)

![](20240103001928.png)

<div style="page-break-before: always">S62079</div>

### REFLECTION QUESTIONS 

1. What are the most important steps you would recommend for securing a new Web application? 
2. How would you perform a security test on a web application for unauthenticated tests on log-in page scenarios? 
3. How does a web application firewall (WAF) detect and prevent attacks? 
4. List the challenges for the successful deployment and monitoring the web intrusion detection

---

1. have a good security developer team
2. hire a pentester, try to find bug by figuring out the rules to abuse
3. filter out possibly dangerous traffic, preventing stuff like XSS and SQL attacks
4. maybe
	- undiscovered zero day 
	- incompetent IT security department
	- deprecating and vulnerable not up to date software
