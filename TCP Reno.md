---
tags: 🌱
date: 19--Mar--2023
---

# TCP Reno


- Slow start
    - Increase window size till timeout
        - Get slowstart threshold, which is half of timeout window
        - Slowstart to the threshold
- Perform additive increase
    - Till [[Triple duplicate acknowledgement]]
    - Then multiplicative decrease by half
    - Protocol also known as [[AIMD]]

The whole protocol gives a Saw Tooth graph shape.

---
Links: 