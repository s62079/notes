- IEEE 802.2 & 802.3
- OSI's Layer 1 & 2 (data encapsulation something)
	- frame delimiting
	- addressing 
	- error detection

- An Ethernet MAC address is a 48-bit binary value expressed as 12 hexadecimal digits (4 bits per hexadecimal digit).
- The IEEE assigns the vendor a 3-byte (24-bit) code, called the Organizationally Unique Identifier (OUI).

Max value for MAC and IP is used for broadcasting

## LAN Switches 

^b33651

- Layer 2 Ethernet 
- Keep track of MACs by their request

### Switching Data

- Store and forward: store to check data validity with CRC before sending
- Cut-through: ~~spam~~ send to destination ASAP (Fast-forward) / Store first 64 byte before sending

How they store it though? Memory buffering. 

- port-based: queue in port
- shared: common

Duplex[^1] mismatch might occur if 2 are different mode.

`mdix auto` detects connection type (device to device).

## Address Resolution Protocol (ARP)

```
FFFF:FFFF:FFFF:FFFF,  255.255.255.255
```

When sending stuff to remote network, destination MAC is host default gateway. But then **how do you know what MAC they are?**

### I Mean, You Knew the Answer Already (Tips: Above) 

- it maps IPv4 with MAC
- if there is no record, ARP will figuritout
- oh yeah, they remove the entry if not used for too long
- or manually remove it, if you want
- ARP broadcasts too
- you can, of course, use ARP to spoof other peoples (pretend you are the destination, modify crap, send virus to actual destination)

> [!Note]
> IPv6 uses Neighbor Discovery Protocol (NDP) instead.

## References

[^1]: [[Network Access#^e40f12]]
