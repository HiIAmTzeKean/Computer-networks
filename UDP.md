---
tags: 🌱
date: 26--Apr--2023
---

# UDP
User datagram protocol
## Properties
- Lightweight communication
    - No overhead from delay of ordered delivery
    - Less bytes in header (4 byte)
- Optional error checksum
## Advantage
- No delay from application
    - Unlike [[TCP]], a packet can be sent once process writes data into socket
    - No minimum size needed for packet to be sent
- No connection delay
    - [[TCP]] requires a 3-way handshake which will take time
- No connection state
- No buffer or sequence number management
## Use case
- Video streaming service
    - Transmission of real time packet is not worthwhile
- Domain name service
    - Overhead for reliable connection not needed
---
Links: 