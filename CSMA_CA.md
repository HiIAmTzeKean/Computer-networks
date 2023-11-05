---
tags:
  - 🌱
  - ComputerScience
date: 24--Feb--2023
---

# CSMA_CA

Unlike [[CSMA_CD]], [detecting energy surge from wireless signal is tough](https://www.geeksforgeeks.org/carrier-sense-multiple-access-csma/).
Nodes are made to detect if other nearby nodes are communicating with target, if not idle, wait till idle.
- Hidden node problem
    - B within A reach
    - B within C reach
    - A and C outside of each other's range
    - A does not know when C is communicating with B
- Exposed node problem
    - B, C within A reach
    - A, C within B reach
    - B, D within C reach
    - B, C within D reach
    - B is transmitting to A, C can sense B is transmitting
        - C might want to transmit to D but does not know if B is transmitting to D
    - Interference is not certain as the exposed node could be transmitting to another node with no collision

## Solution
- Sender and Receiver exchange control frames before transmitting data
- S sends Request To Send (RTS) to indicate how long transmission should hold
    - Nodes that see RTS but not CTS know they are not close enough to interfere with their own transmission → address Exposed Node problem
- R sends Clear To Send (CLS) to S
    - Nodes that see CLS knows they are within range of R
    - Nodes also know they cannot transmit with R → address **Hidden Node problem**

---
Links: 