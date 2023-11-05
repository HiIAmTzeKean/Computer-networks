---
tags:
  - 🌱
  - ComputerScience
date: 23--Feb--2023
---

# Bit stuffing

Sentinel based
- Frame starts with 01111110 flag (7E)
- Used in HDLC and PPP

## Algorithm
After 5 consecutive "1" insert a "0" for sender
Receiver will remove a "0" after 5 "1"

---
Links: 