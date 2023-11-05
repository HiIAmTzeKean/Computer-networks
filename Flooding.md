---
tags:
  - 🌱
  - ComputerScience
date: 12--Apr--2023
---

# Flooding

When a [[Node]] receives a packet, it will forward the packet to all other links except the incoming link. 
- The packet will be labelled with a unique identifier
- If a packet with the same identifier returns, it is discarded

## Advantage
- Packet will always get through entire network if one or more path exists

## Disadvantage
- Waste bandwidth
- Can cause [[Network congestion]]

---
Links: 