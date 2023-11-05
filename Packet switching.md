---
tags:
  - 🌱
  - ComputerScience
date: 21--Feb--2023
---

# Packet switching

[[Store and forward]] technique
- Forward based on forwarding table (MAC table)
- Statistical [[TDM]]
- Packets can travel through different routes based on link utilisation and capacity
    - Possibility of congestion
## Calculating demand
- With 35 users, each active 10% of the time
- Link of 1Mb/sec and user will use 100kb/sec when active
    - Hence maximum of 10 active users before congestion
- P(users>10)
    - [[Binomial distribution]]
    - B(trials=35, events=10)
    - Probability is 0.0005
## Delay
- Node processing
    - Bit error checking
- Queueing
    - Packet waiting at output link for transmission
- Transmission delay
    - [[Bandwidth]] and packet size
- Propagation delay
---
Links: 