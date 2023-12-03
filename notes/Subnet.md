Dividing a network into more networks for better internet traffic and easier management. 

## Octet Boundaries

It is easier to subnet the network by octet.

| Prefix Length | Subnet Mask | Subnet Mask (Binary) | 
| - | - | :-: | 
| /8 | 255.0.0.0 | 11111111.00000000.00000000.00000000 |
| /16 | 255.255.0.0 | 11111111.11111111.00000000.00000000 |
| /24 | 255.255.255.0 | 11111111.11111111.11111111.00000000 |

| Subnet | Hosts | Broadcast |
| :-: | :-: | :-: |
| ==10.0==.0.0/16 | 10.0.==0.1== - 10.0.==255.254== | 10.0.255.255 |
| ==10.1==.0.0/16 | 10.1.==0.1== - 10.1.==255.254== | 10.1.255.255 |
| ... | ... | ... |
| | | |
| ==10.0.0==.0/24 | 10.0.0.==1== - 10.0.0.==254== | 10.0.0.255 |
| ==10.0.1==.0/24 | 10.0.1.==1== - 10.0.1.==254== | 10.0.1.255 |
| ... | ... | ... |
| ==10.0.255==.0/24 | 10.0.255.==1== - 10.0.255.==254== | 10.0.255.255 |
| ==10.1.0==.0/24 | 10.1.0.==1== - 10.1.0.==254== | 10.1.0.255 |
| ... | ... | ... |

> [!Note]
> The number of subnets (left) are inversely proportional to the number of hosts (right) you can have.

## Classless Subnetting

You can, in fact, subnet a subnet. For example, if you were to subnet a /24 network:

| Prefix Length | Subnet Mask | Subnet Mask (Binary) | # of subnets | # of hosts | 
| :-: | :-: | :-: | :-: | :-: |
| /25 | 255.255.255.128 | 11111111.11111111.11111111.==1==0000000 | 2 | 126 |
| /26 | 255.255.255.192 | 11111111.11111111.11111111.==11==000000 | 4 | 62 |
| ... | ... | ... | ... | ... |

> [!Formula]
> $\#$ $of$ $hosts$ $= 2^n - 2$

So basically when you need to create $x$ amount of subnets, just get the closest value (rounded up) of $2^n$, $n$ will be the # of bits required for the subnets.

## Variable Length Subnet Mask (VLSM)

Slice the subnet until it fits the requirements.

## Addressing Schemes

- every address is unique (server, client, intermediary, gateway)
- allow a layer 3 address to control access of the server

## IPv6

- not for saving space, so no subnet for link-local address
- create hierarchy
- can make subnet for global unicast
