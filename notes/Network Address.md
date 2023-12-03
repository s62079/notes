## A Math Section, You're Welcome

- Binary Decimal: power 2
- Binary Hexadecimal: pair of 4
- Logical AND

## Ok, Back to IPv4

- IPv4 is hierarchical, which I have no idea what that means
- it consists of 2 part, network portion and host portion, which can be identified with subnet mask.

### Subnet Mask

- refer above
- can be shorthand expressed in prefix length

### Prefix Length

| Mask | Address | Prefix Length |
| --- | --- | --- | 
| 255.0.0.0 | 11111111.00000000.00000000.00000000 | /8 |  
| 255.255.255.0 | 11111111.11111111.11111111.00000000 | /24 |  
| 255.255.255.248 | 11111111.11111111.11111111.11111000 | /29 | 

### Roles

- first address is network address (outside use)
- last address is broadcast address (to all hosts)
- others are host addresses

### Public and Private

> [!History]
> At some point, they've finally realized that IPv4 is just not enough, but nobody seemed to take IPv6 _that_ seriously yet (though it's the same for NAT), though business need made the push for it. And there comes NAT.

#### Private Address

Internal use, yada yada

- 10.0.0.0/8 or 10.0.0.0 to 10.255.255.255
- 172.16.0.0/12 or 172.16.0.0 to 172.31.255.255192.168.0.0/16
- 192.168.0.0 to 192.168.255.255

##### Special

- loopback (127.0.0.0/8 or 127.0.0.1): also known as localhost, the host itself
- link-local (169.254.0.0/16 or 169.254.0.1): also known as I MADE IT OUT address (**the address PC declare itself as**), when DHCP not working and IPv4 is unconfigured
- TEST-NET (192.0.2.0/24 or 192.0.2.0 to 192.0.2.255): educational purposes

> [!Note]
> - Link-local on IPv6 is `FE80::` 
> - DHCP is broadcast in IPv4
> - IPv6 don't broadcast
> - So instead, link-local on IPv6 is also used for router discovery
> - Oh yeah, so DHCPv6 uses multicast 

### Address Class

- A (0.0.0.0/8 - 127.0.0.0/8): largest
- B (128.0.0.0/16 - 191.255.0.0/16): mid
- C (192.0.0.0/24 - 223.255.255.0/24): smallest

> [!History]
> And then they have decided that it's a waste of resource and time, gone classless since then.

## IPv6

```
FFFF:FFFF:FFFF:FFFF:FFFF:FFFF:FFFF:FFFF
```

### Shorthand

- `0` for `0000`
- chain of `0`s can be hidden with `::` (**only 1** `::` in address)

### Types

- unicast
- multicast
- ~~broadcast~~ anycast: an address that can be assign to multiple devices

### Prefix Length

Same shit but in hex.

### Special

- global unicast: public address
- link-local (`FE80::`)
- unique local (`FC00::/7` - `FDFF::/7`): local stuff
- loopback (`::1/128`)
- unspecified (`::/128`)

## Verification

Check alive.

- ping them
- ping them, but with convoluted method such as ICMPv4 or ICMPv6
- self ping
- ping gateway 

### Migration From IPv4

- dual stack: run both IPv4 and IPv6
- tunneling: encapsulate IPv6 packet in IPv4
- translation: NAT64, allow IPv4 to talk to IPv6
