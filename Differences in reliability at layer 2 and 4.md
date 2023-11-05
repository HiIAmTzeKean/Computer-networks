---
tags:
  - 🌱
  - ComputerScience
date: 19--Mar--2023
---

# Differences in reliability at layer 2 and 4

[[Data layer]] vs [[Transport layer]]
- Retransmission at both if it fails

What is important is that if a packet is sent out from the sender, then the receiver receives it.

Data layer
- Hop by hop retransmission
- If we only had hop by hop, there is no guarantee that there is end-to-end reliability
    - When a node sends out the packet to the next hop, there is no guarantee that the next hop forwards the packet

Transmission layer
- End to end retransmission
- End-to-end alone is not sufficient


---
Links: 