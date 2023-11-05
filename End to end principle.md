---
tags:
  - 🌱
  - ComputerScience
date: 19--Mar--2023
---

# End to end principle

- Normal routers only use Data layer and Network layer.
- Key idea is to ensure flow (oppose to packets), packet that flows from one end to the other

## Fair allocation of resources
- [[CHOKe]]
    - Ensures fair bandwidth partitioning
    - Preemptive dropping of packets
    - Randomised algorithm
    - Pick 2 packets and if they are the same, then drop it
    - Else sample again
- [[SIFT algorithm]]
    - [[Elephant traps]]
    - Reduce average delays for short and long flows
    - Samples random packet to identify if a packet belongs to a short or long flow
    - They are separated in different buffers

---
Links: 