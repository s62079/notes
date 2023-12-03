## Protocols

Temporary communication between applications to transfer data.

- track communication
- segment data
- identify application

On this layer, there are 2 protocols that can be used to handle the data, namely TCP and UDP. Here is a brief overview of how the respective protocol handles their data.

![[net-tcp-vs-udp.png|400]]

## TCP

- tracks data segments
- acknowledge received data
- redo the job when its not ack-ed

Header size: 20 bytes (_everything UDP have_, seq #, ack #, control bits, window size)

- control bits: purpose of TCP segment
- window size: number of bytes that can be accepted at one time

### 3-Way Handshake

Yes, destination exists.

- kominication starts with TCP segment of `SYN`,  `SYN, ACK` and `ACK`
- ends with `FIN`

## UDP

- fast
- no ack

Header size: 8 bytes (source port, destination port, length, checksum)

## Ports

- `0 - 1023`: reserved for service
- `1024 - 49151`: registered for specific app
- `49152 - 65535`: dynamic or private, client OS said so

![[net-transport-ports.png|400]]

