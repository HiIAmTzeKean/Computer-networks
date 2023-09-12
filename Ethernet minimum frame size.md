---
tags: 🌱
date: 24--Feb--2023
---

# Ethernet minimum frame size

The minimum size is 64 bits
- 14 byte header
    - 6 Destination
    - 6 Source
    - 2 Length
- 4 byte CRC

- Key idea
    - Host should still be transmitting when collision occurs
    - Suppose collision occurs near Receiver (R) and R sends jamming signal
    - Take T_p to reach Sender (S)
    - S would normally take T_f + T_p to send frame
    - So the total time taken would be T_f + 2T_p
        - If T_f is too small, then collision might occur after S is done transmitting frame
        - Goal is to find a T_f such that S still transmitting
        - Then T_f \ge 2 T_p for R to send a jam signal and to be received by S while it is still transmitting
    - Ethernet [[Bandwidth]] is 10Mbps, and RTT for Ethernet bounded by 51.2microsec
    - Minimum size is 512 bits

---
Links: 