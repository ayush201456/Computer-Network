# Computer-Network
Lab Assignments


**Experiment - 1**

Design and simulate a simple computer network using various connection topologies (bus, star, ring, mesh). Compare the advantages and disadvantages of each topology in terms of data flow and network efficiency.

BUS TOPOLOGY 

Steps:
1. Open Cisco Packet Tracer
2. Drag 4–5 PCs
3. Drag 1 Hub
4. Connect all PCs to the hub using Copper Straight-through cables
5. Assign IP addresses:
PC1 → 192.168.1.1
PC2 → 192.168.1.2
PC3 → 192.168.1.3
6. Use Add Simple PDU (envelope icon) to send packets
7. Observe packet flow (shared medium behavior)

STAR TOPOLOGY

Steps:
1. Place 1 Switch
2. Add 4–6 PCs
3. Connect each PC to the switch using Straight-through cable
4. Assign IPs (same network):
192.168.2.x
5. Send PDU between PCs
6. Observe: communication via central switch

RING TOPOLOGY

Steps:
1. Packet Tracer does not directly support ring via a single device, so simulate manually:
2. Place 4 PCs
Connect:
PC1 → PC2
PC2 → PC3
PC3 → PC4
PC4 → PC1
3. Use Cross-over cables
4. Assign IPs (same network: 192.168.3.x)
5. Send PDU and observe circular path

MESH TOPOLOGY

Steps:
1. Place 4 PCs
2. Connect each PC to every other PC
3. Use Cross-over cables
4. Assign IPs:
192.168.4.x
5. Send PDU
6. Observe multiple paths for data

HYBRID TOPOLOGY

Steps:
1. Add 2 Switches + 1 Hub + PCs
2. PCs → Switches (Star)
3. Switches → Hub (Bus backbone)
4. Test → observe combined behavior

**Experiment - 6**

Develop a simulation to demonstrate multiple access protocols such as Pure ALOHA, Slotted ALOHA, CSMA/CD, and CSMA/CA. Analyze the performance of each protocol in handling network collisions and maximizing data transmission efficiency.

CSMA/CA is a network protocol used in wireless networks (Wi-Fi) to avoid collisions before they happen.

Steps:-

1. Sense channel
2. If idle → Wait (IFS time)
3. Send RTS (Request to Send)
4. Receive CTS (Clear to Send)
5. Transmit data
6. Receive ACK
7. If no ACK → Retransmit

CSMA/CD is a network protocol used in wired Ethernet LANs to control how devices share a communication channel.

Steps:-
1. Sense the channel – Device checks if medium is idle
2. If idle → Transmit data
3. If busy → Wait
4. During transmission → Detect collision
5. If collision occurs → Send jam signal
6. Stop transmission
7. Wait (Backoff time)
8. Retransmit



**Experiment - 7**
Create a simulation to demonstrate logical addressing using IPv4 and IPv6. Implement address mapping techniques such as ARP and DHCP to show how devices acquire and resolve network addresses.

**ARP**

ARP is used to map an IP address to its corresponding MAC address in a local network.

STEPS:-



**DHCP**

DHCP is used to automatically assign IP address, subnet mask, gateway, and DNS to devices in a network.

STEPS:-

1.Create a network with one server, one switch, and multiple PCs.
2. Connect server and PCs to the switch using straight-through cables.
3. Assign a static IP to the server (e.g., 10.0.0.1).
4. Open server → Services → DHCP and turn DHCP service ON.
5. Create a DHCP pool and set network (10.0.0.0) with subnet mask.
6. Configure default gateway (e.g., 10.0.0.1) and DNS server.
7. Set starting IP range (e.g., 10.0.0.2 onwards).
8. Save the DHCP configuration.
9. Set all PCs to DHCP mode in IP configuration.
10. Verify PCs receive IP addresses automatically and test using ping.
