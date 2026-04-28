# 🌐 Computer-Network Lab Assignments

---

## 🧪 **Experiment - 1**

**Design and simulate a simple computer network using various connection topologies (bus, star, ring, mesh). Compare the advantages and disadvantages of each topology in terms of data flow and network efficiency.**

---

### 🔹 **BUS TOPOLOGY**

**Steps:**

1. Open Cisco Packet Tracer
2. Drag 4–5 PCs
3. Drag 1 Hub
4. Connect all PCs to the hub using Copper Straight-through cables
5. Assign IP addresses:

   * PC1 → 192.168.1.1
   * PC2 → 192.168.1.2
   * PC3 → 192.168.1.3
6. Use **Add Simple PDU** (envelope icon) to send packets
7. Observe packet flow *(shared medium behavior)*

---

### 🔹 **STAR TOPOLOGY**

**Steps:**

1. Place 1 Switch
2. Add 4–6 PCs
3. Connect each PC to the switch using Straight-through cable
4. Assign IPs *(same network)* → `192.168.2.x`
5. Send PDU between PCs
6. Observe communication via central switch

---

### 🔹 **RING TOPOLOGY**

**Steps:**

1. Packet Tracer does not directly support ring via a single device, so simulate manually
2. Place 4 PCs and connect:

   * PC1 → PC2
   * PC2 → PC3
   * PC3 → PC4
   * PC4 → PC1
3. Use Cross-over cables
4. Assign IPs → `192.168.3.x`
5. Send PDU and observe circular path

---

### 🔹 **MESH TOPOLOGY**

**Steps:**

1. Place 4 PCs
2. Connect each PC to every other PC
3. Use Cross-over cables
4. Assign IPs → `192.168.4.x`
5. Send PDU
6. Observe multiple paths for data

---

### 🔹 **HYBRID TOPOLOGY**

**Steps:**

1. Add 2 Switches + 1 Hub + PCs
2. PCs → Switches *(Star)*
3. Switches → Hub *(Bus backbone)*
4. Test and observe combined behavior

---

## 🧪 **Experiment - 2**

**Create a network simulation to demonstrate packet switching and circuit switching. Compare performance and efficiency.**

---

### 🔌 **What is Circuit Switching?**

Circuit switching establishes a **dedicated path** between sender and receiver before transmission.

**Steps:**

1. Create a network with two PCs connected through routers via a single path
2. Connect devices using appropriate cables
3. Assign IP addresses
4. Enable router interfaces using `no shutdown`
5. Configure static routing
6. Send data using `ping`
7. Observe fixed path
8. Note reserved path during communication
9. Verify transmission
10. Conclude dedicated path usage

---

### 📦 **What is Packet Switching?**

Packet switching divides data into **small packets** and sends them through different paths.

**Steps:**

1. Create network with multiple PCs and switch
2. Connect using straight-through cables
3. Assign IPs in same network
4. Switch to Simulation Mode
5. Send PDU
6. Observe packet division and transfer
7. Track packet movement
8. Verify delivery
9. Repeat for different nodes
10. Conclude packet-based transmission

---

## 🧪 **Experiment - 3**

**Analyze packet delay, loss, and throughput.**

**Steps:**

1. Create network with two PCs and switch
2. Assign IP addresses
3. Ping to verify connectivity
4. Start continuous ping
5. Disconnect cable *(simulate failure)*
6. Observe packet loss
7. Reconnect cable
8. Observe recovery
9. Record behavior
10. Conclude impact of errors

---

## 🧪 **Experiment - 4**

**Implement error detection and correction using block coding and CRC.**

**Steps:**

1. Create simple topology
2. Assign IPs
3. Verify using `ping`
4. Switch to Simulation Mode
5. Send PDU
6. Observe transmission
7. Drop/modify packets
8. Re-send packets
9. Explain CRC
10. Explain block coding

---

## 🧪 **Experiment - 5**

**Flow control & error control protocols (Stop & Wait, Go-Back-N, Selective Repeat).**

**Steps:**

1. Create topology
2. Assign IPs
3. Configure gateway
4. Switch to Simulation Mode
5. Send PDU
6. Observe flow
7. Drop packets
8. Retransmit
9. Repeat process
10. Analyze results

---

## 🧪 **Experiment - 6**

**Multiple Access Protocols (ALOHA, CSMA/CD, CSMA/CA).**

---

### 📡 **CSMA/CA (Wireless)**

1. Sense channel
2. If idle → Wait (IFS)
3. Send RTS
4. Receive CTS
5. Transmit data
6. Receive ACK
7. Retransmit if needed

---

### 🔌 **CSMA/CD (Wired)**

1. Sense channel
2. If idle → Transmit
3. If busy → Wait
4. Detect collision
5. Send jam signal
6. Stop transmission
7. Wait (Backoff)
8. Retransmit

---

## 🧪 **Experiment - 7**

### 🔗 **ARP**

Maps IP address to MAC address.

**Steps:**

1. Create network with switch and PCs
2. Assign IPs
3. Switch to Simulation Mode
4. Send PDU
5. Observe ARP request
6. Observe ARP reply
7. Verify mapping
8. Continue simulation
9. Complete ICMP
10. Verify resolution

---

### 🌐 **DHCP**

Automatically assigns IP configuration.

**Steps:**

1. Create network with server and PCs
2. Connect devices
3. Assign server IP
4. Enable DHCP service
5. Create pool
6. Configure gateway & DNS
7. Set IP range
8. Save config
9. Set PCs to DHCP
10. Verify assignment

---

## 🧪 **Experiment - 8**

**Sliding window protocol with piggybacking.**

**Steps:**

1. Create topology
2. Assign IPs
3. Verify using `ping`
4. Simulation Mode
5. Send bidirectional PDU
6. Observe flow
7. Send multiple packets
8. Observe piggybacking
9. Drop packets
10. Analyze ACK handling

---

## 🧪 **Experiment - 9**

**Transport layer protocols (RIP).**

**Steps:**

1. Assign IPs
2. Configure PCs
3. Enable interfaces
4. Start RIP → `router rip`
5. Set version → `version 2`
6. Disable auto-summary
7. Add networks
8. Configure all routers
9. Check → `show ip route`
10. Test using ping

---

## 🧪 **Experiment - 10**

### 🌐 **DNS & DDNS**

DNS converts domain names into IP addresses.

**Steps:**

1. Assign IPs to PC, DNS Server, Web Server
2. Configure DNS server
3. Add record:

   ```
   www.krmu.edu → 192.168.1.200
   ```
4. Enable HTTP
5. Open browser
6. Enter URL
7. Observe resolution

---

## 🧪 **Experiment - 11**

**HTTP & Web Server Simulation**

**Steps:**

1. Assign IPs
2. Configure DNS
3. Enable HTTP
4. Open browser
5. Enter URL
6. Observe webpage loading

---

