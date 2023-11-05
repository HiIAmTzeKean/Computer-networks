---
tags:
  - 🌱
  - ComputerScience
date: 21--Feb--2023
---

# Ethernet

## Architecture
[[Ethernet cabling]]
[[Ethernet frame]]
[[Ethernet address]]
[[Ethernet minimum frame size]]

## Fixes
Ethernet uses broadcast based transmission
- Collision detection
    - No coordination between host. When there is collision, signal energy doubles
    - [[CSMA_CD]]
- Retransmission
    - Collision issue
    - [[Exponential backoff algorithm]]

## Lan types
- Bus-based
    - Single collision domain
- Hub-based
    - When frame received on port, copied and forwarded to all other ports
    - Single collision domain
    - All host shares the same [[Bandwidth]]
- Switch-based
    - Similar to hub configuration (Star)
    - Store and forward
    - No collision between ports, only within ports themselves
    - Duplex connection and bandwidth can be multiplexed

---
Links: 