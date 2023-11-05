---
tags:
  - 🌱
  - ComputerScience
date: 24--Feb--2023
---

# Extended LAN

Interconnect multiple LAN using bridges/ switches.

## Spanning Tree bridge
Also known as transparent bridge

- Host mapping to port are learnt through [[Backward learning method]]
- Issue of looping in typical LAN
    - Loops may exist to ensure reliability of links
    - Tree does not have loop
        - Every pair of node has unique path to each other
        - Shortest spanning tree
    - [[Distributed spanning tree algorithm]]
- When node is not root
    - Stop generating config message
- When node is not bridge
    - Stops forwarding config message

---
Links: 