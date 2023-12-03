#cybersec

<div style="page-break-before: always">S62079</div>

## TASK 1: SETTING UP THE VIRTUAL LAB NETWORK

it worked. 

![](20231202194605.png)

<div style="page-break-before: always">S62079</div>

## TASK 2: MAN-IN-THE-MIDDLE ATTACK USING ARP POISONING 

![](20231202195752.png)

and the password is revealed.

1. In your own words, explain ARP poisoning. 
	- when someone is transmitting data, you pretend to be the destination machine by sending malicious ARP packets and corrupt the ARP table. which means now you have access to **every** data transmitted between the two machines.
2. How can we prevent the ARP poisoning attack? 
	- get a good firewall that filter packets
	- use VPN (questionable)
	- have a static ARP table
3. Why do you think telnet is not a safe way to connect to a remote machine? What is the safer way to do so?
	- because transmitted data is not encrypted, it makes people easier to access your sensitive information. 

<div style="page-break-before: always">S62079</div>

## TASK 3: ANALYSING THE NETWORK PACKET

![](20231202225638.png)

![](20231202235558.png)

![](20231202235530.png)

![](20231202235942.png)

![](20231203000215.png)

<div style="page-break-before: always">S62079</div>

1. Based on your understanding, what is a network security and what are the basic objectives of network security? 
	- protecting network from unauthorized events (that mostly cause troubles)
	- "Unauthorized access to the network. Disruption or degradation of performance, or any other interference with normal functioning of the network. Use of the network in violation of Responsible Use of Information Resources" - University of Michigan
	- TL; DR, make sure there is no unauthorized usage
2. Differentiate between Intrusion Detection System (IDS) and Intrusion Prevention System (IPS). 
	- the name literally tells you, one only **detects** the intrusion, while the other **prevents** the intrusion
3. Why Virtual Private Network (VPN) is important for network security? 
	- make sure data are safely transmitted
4. In what situation you might want to install a Demilitarized Zone (DMZ) on your network? 
	- DMZ is an "area" where the network is unprotected from outside
	- probably use for stuffs like security camera access or web hosting
5. What is the role of Network Address Translation (NAT) on a network?
	- translate your local network address to public network address before going internet
6. To applied and manage the security principle, you must understand how the network devices and technologies operate. Explain how the proxy server operates to provide security on the network
	- proxy server can be hosted to filter out most danger stuffs before routing the actual useful part of data to your machine