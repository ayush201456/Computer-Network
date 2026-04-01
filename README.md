# Computer-Network
Lab Assignments


**Experiment - 1**

Design and simulate a simple computer network using various connection topologies (bus, star, ring, mesh). Compare the advantages and disadvantages of each topology in terms of data flow and network efficiency.

BUS TOPOLOGY 

Steps:
Open Cisco Packet Tracer
Drag 4–5 PCs
Drag 1 Hub
Connect all PCs to the hub using Copper Straight-through cables
Assign IP addresses:
PC1 → 192.168.1.1
PC2 → 192.168.1.2
PC3 → 192.168.1.3
Use Add Simple PDU (envelope icon) to send packets
Observe packet flow (shared medium behavior)

STAR TOPOLOGY

Steps:
Place 1 Switch
Add 4–6 PCs
Connect each PC to the switch using Straight-through cable
Assign IPs (same network):
192.168.2.x
Send PDU between PCs
Observe: communication via central switch

RING TOPOLOGY

Steps:
Packet Tracer does not directly support ring via a single device, so simulate manually:
Place 4 PCs
Connect:
PC1 → PC2
PC2 → PC3
PC3 → PC4
PC4 → PC1
Use Cross-over cables
Assign IPs (same network: 192.168.3.x)
Send PDU and observe circular path

MESH TOPOLOGY

Steps:
Place 4 PCs
Connect each PC to every other PC
Use Cross-over cables
Assign IPs:
192.168.4.x
Send PDU
Observe multiple paths for data

HYBRID TOPOLOGY

Steps:
Add 2 Switches + 1 Hub + PCs
PCs → Switches (Star)
Switches → Hub (Bus backbone)
Test → observe combined behavior

**Experiment - 6** 

**Develop a simulation to demonstrate multiple access protocols such as Pure ALOHA, Slotted ALOHA, CSMA/CD, and CSMA/CA. Analyze the performance of each protocol in handling network collisions and maximizing data transmission efficiency.**

CSMA/CD
Steps:-
1. **Sense the channel** – Device checks if medium is idle
2. If idle -> Transmit data
3. If busy -> Wait
4. During transmission -> Detect collision
5. If collision occurs -> Send jam signal
6. Stop transmission
7. Wait (Backoff time)
8. Retransmit

CSMA/CA
Steps:-
1. **Sense channel**
2. If idle → Wait (IFS time)
3. Send RTS (Request to Send)
4. Receive CTS (Clear to Send)
5. Transmit data
6. Receive ACK
7. If no ACK → Retransmit
