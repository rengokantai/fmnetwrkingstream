# fmnetwrkingstream
## Networking, servers and clients
### Networking and Packets
tcp vs udp
- TCP: reliable transport: if a packet is not acknowledged (ACK) on the other hand, it gets resent
- UDP: unreliable transport, packets are sent but there is no confirmation that the packet was received at
the other end

#### port and permission
By default systems can only listen to ports below 1024 as the root user.
```
nc -lp 1024 //no problem
nc- lp 1023 //permission issue
```

#### p2p
Nodes in the network are symmetric with no fixed central servers
node1
```
nc -lp 50000
```
node2
```
nc localhost 5000
```
