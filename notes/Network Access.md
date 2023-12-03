## Physical

- Network Interface Card (NIC)
- WLAN NIC

### Signals

- electrical: copper
- light: optic fiber
- microwave: wireless

### Functions

Convert bit to code. One of the method is signaling.

- Bandwidth: max data transfer rate
- Throughput: _actual_ throughput

## Media

Real-life application, everything is screwed to a certain extent (interference).

### So They R&D Shit to Reduce Interference

- Twisted cable
	- Shielding
- Coaxial cable
	- Shielding
	- Plastic insulation
- UTP Connector (Ethernet)

But optic fiber cable is better because it is immune to the interferences (EMI, RFI, Electrical Hazards).

## Data Link

If a packet have to travel by router, its frame (MAC Address) will be changed (re-encapsulate) until it reaches the destination something.

## Media Access Control (MAC)

Traffic manager, based on topology[^1].

### Physical Topology: The Sequel 

#### WAN

- Point-to-Point: 1-to-1
- Hub and Spoke: one in the middle
- Mesh: battle royale

#### LAN

- Star: Hub and Spoke, but middle is _something_[^2]
- Extended Star: middle chain
- Bus: linear chain, old stuff
- Ring: also old stuff

## Duplex

^e40f12

- Half: "turn based"
- Full: "real time"

## The Frame

- Head
- Data
- Trailer

## References

[^1]: [[Explore the Network#^9b496a]]
[^2]: [[Network Layer#^b33651]]