---
tags:
  - 🌱
  - ComputerScience
date: 23--Feb--2023
---

# Sliding window

Multiple frames transmitted to improve link utilization
- Buffer of $w$ frames
    - Frames are sequenced
    - Can transmit up to $w$ frames without waiting for ACK
- ACK(n) or RR(n)
    - Indicates that frames till n-1 received
    - Or interpret as waiting for frame n

## Enhancement
- Receive not ready
    - Normal ACK to resume
- Piggybagging
    - Receiver can send ACK as part of data frame to another node

---
Links: 