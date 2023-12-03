## Terminology

- protocol: rules to kominicate on internet
- encoding
- formatting 
- size
- timing 
- delivery options
	- unicast
	- multicast
	- broadcast

## Protocols

- HTTP: server and client
- TCP: manage convo
- IP: butcher TCP into packets

## Internet Standards

![[net-standard-organizations.png]]

## Layered Model

Why do you think that it is good?

| TCP/IP | Protocols | OSI |
| --- | --- | --- |
| Application | HTTP, DNS, DHCP, FTP | Application, Presentation, Session (Data) | 
| Transport | TCP, UDP | Transport (Segment) | 
| Internet | IPv4, IPv6 | Network (Packet) |
| Network | PPP, Frame Relay, Ethernet | Data Link (Header), Physical |

## Data Transfer

Since they transfer by packet, it can handle multiple shit at once (multiplexing).

