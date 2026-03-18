# Computer-Network
Lab Assignments

Experiment - 6 **Develop a simulation to demonstrate multiple access protocols such as Pure ALOHA, Slotted ALOHA, CSMA/CD, and CSMA/CA. Analyze the performance of each protocol in handling network collisions and maximizing data transmission efficiency.**

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
