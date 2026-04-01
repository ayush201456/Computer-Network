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
