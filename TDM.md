---
tags:
  - 🌱
  - ComputerScience
date: 21--Feb--2023
---

# TDM
Time division multiplexing.
Users use entire frequency but transmit on different time slice.

## Aggregating link
Suppose there are 2 links each with [[Bandwidth]] R, then the output must be 2R to ensure no loss of data. This process is called **Byte interleaving**. From a frame perspective, first byte is from link 1 and second byte from link 2.

## Fixed TDM
By default TDM is fixed time slice.
- Guarantee bandwidth and no queuing delay at node
- Inefficient bandwidth utilisation if input link not always active

## Statistical TDM
- No reservation of [[Bandwidth]] on output link
- Output link bandwidth based on statistic demand
    - Suppose inputs are active 60% of time, 2 input, each 10Mbps
    - Output [[Bandwidth]] reserved at 12Mbps
    - If input sum exceed output, excess frames queued in buffer
    - Loss of data if buffer overflow. Refer to [[Congestion control]]
- Efficient bandwidth utilisation

---
Links: 