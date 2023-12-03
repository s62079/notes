## Terminology

- shell: access kernel
- kernel: talk with hardware
- hardware

- CLI: text 
- GUI: visual

## Internetwork Operating System (IOS)

Cisco IOS is CLI used to configure network device. It can be accessed with: 

- console
- SSH
- telnet

### Commands 

^bfa558

- `[enable | disable]`: user & privileged mode
	- `configure terminal`: enter config mode
		- `interface $DEVICE`: configure network
			- `show`
				- `ip`
					- `interface brief`
					- `interfaces`
					- `route`
			- `ip`
				- `address`
				- `default-gateway`
			- `no shutdown`: keep the device alive
		- `line [console 0 | vty 0 15]`: configure console
			1. `password $PW`: set console password
			2. `login`
		- `hostname $NAME`
		- `service password-encryption`
		- `enable secret $PW`: set EXEC password
	- `show [run | start]`
	- `copy run start`: change startup config 

## Address Schemes

- Address
- Subnet mask
- Default gateway

Assign IP address automatically with DHCP.

### Some Other ~~Useless~~ Basic Commands

- `ping`
- `ipconfig`
