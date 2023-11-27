# CSM3233 Lab 4
#### Gary Lim S62079

<div style="page-break-after: always"><br></div>

## TASK 1: DISCOVERING OPEN PORTS IN WINDOWS

![](20231116151432.png)

![](20231116151731.png)

1. Explain what is defense in-depth and how to relate to the host security? 
	- Defense in depth is having multiple layers of security. Using strong passwords, keeping software updated are some of the layers for host security. 
2. Based on your understanding, explain why host security is important?
	- Because nobody wants their privacy getting exposed, nor they want someone to do crime using their identity. 

<div style="page-break-after: always"><br></div>

## TASK 2: KALI LINUX AND METASPLOITABLE NETWORK SET UP

![](20231116160314.png)

![](20231116161607.png)

1. Is there any security issue with the ping command? If so, explain briefly
	- It is possible to spam ping someone to their death (machine)

<div style="page-break-after: always"><br></div>

## TASK 3: SCANNING THE OPEN PORTS

![](20231116164124.png)

![](20231116163908.png)

<div style="page-break-after: always"><br></div>

4. Investigate the open ports of the `Metasploitable` virtual machine (192.168.1.4) detected by the Nmap scanning tool. How many open ports are there? 

| Port | Name                                     |
|------|------------------------------------------|
| 21   | File Transfer Protocol                   |
| 22   | Secure Shell (SSH)                       |
| 23   | Telnet Protocol                          |
| 25   | Simple Mail Transfer Protocol            |
| 53   | Domain Name System                       |
| 80   | Hypertext Transfer Protocol              |
| 139  | NetBIOS Session Service                  |
| 445  | Server Message Block                     |
| 512  | Remote Process Execution                 |
| 513  | Remote Login                             |
| 514  | Syslog Protocol                          |
| 5432 | PostgreSQL Database System               |
| 5900 | Virtual Network Computing                |
| 6000 | X11 Window System                        |
| 1099 | Java RMI (Remote Method Invocation)      |
| 1524 | Ingres Database Management System Lock   |
| 2049 | Network File System                      |
| 2121 | CCProxy FTP Proxy                        |
| 3306 | MySQL Database                           |
| 6667 | Internet Relay Chat                      |
| 8009 | Apache JServ Protocol                    |
| 8180 | Apache Tomcat HTTP Connector             |

<div style="page-break-after: always"><br></div>

1. Scanning can be done without proper consent. Why? 
	- because scanning **IS** pinging / requesting from the server
2. At your organization, is there any statement in the security policy related to scanning activity? Please state it here.
	- yes, if you try to scan them, they are allowed to collect your data for record in return, as mentioned at [Policies and agreements (umt.edu.my)](https://epembelajaran.umt.edu.my/oceania/admin/tool/policy/viewall.php). 

> **b.**   **Usage Data**
> We may also collect information on how the Service is accessed and used ("Usage Data"). This Usage Data may include information such as your computer's Internet Protocol address (e.g. IP address), browser type, browser version, the pages of our Service that you visit, the time and date of your visit, the time spent on those pages, unique device identifiers and other diagnostic data.

<div style="page-break-after: always"><br></div>

## TASK 4: EXPLOITING THE VULNERABLE SERVICE

![](20231116170110.png)

![](20231116170327.png)

1. Why security baseline is important to be applied to a particular host in the enterprise or any company? 
	- because it is the minimum requirement to make sure that the company host is *at least* secure
2. Explain five (5) security techniques to properly secure a virtual host machine. 
	1. configure firewall to filter out extra traffic
	2. update software to make sure exploits are always patched
	3. segment network to isolate breach events
	4. authentication so that nobody have unrestricted access
	5. monitoring and security audits to respond to incident fast
3. Explain five (5) ways to manage host security.
	1. use firewall, as usual
	2. have some sort of anti-virus
	3. make good password
	4. always monitor the log
	5. restrict service access whenever possible