---
tags:
  - 🌱
  - ComputerScience
date: 23--Feb--2023
---

# ARQ

## Stop and wait
[[Stop and wait]]
- Sender waits for ACK before transmitting next frame
- Receiver uses timeout mechanism to trigger resend
- Error free assumption
    - 1 frame per $T_f + 2T_p$
    - $U = \frac{T_f}{T_f + 2T_p} = \frac{1}{1 + 2a}$
- Error case
    - Number of retransmitted frame = $1/(1-P_f)$
    - Recall [[Geometric mean]]
    - $U = \frac{P_s}{1+2a}$
## Go back N
[[Sliding window]]
- If there is no error, continue as normal
- If there is error, discard all future frames
    - Error can be due to damaged frame or lost frame
    - Lost frame might require sender to probe receiver after timeout
- Error case
    - $U = \frac{1-P_f}{1+2aP_f}$
    - $U = \frac{w(1-P_f)}{(1+2a)(P_s+wP_f)}$
## Selective reject
- Only rejected frames retransmitted
- Error free case
    - There are 2 cases, when the window size is large such that there is no idle time (time for 1st frame to reach receiver smaller than window exhaustion rate)
    - When $w*T_f \ge T_f + 2T_p$
        - $U = 1$ there is no idle
    - Otherwise
        - Window exhausted before 1st frame reach
        - Then time taken is still $T_f + 2T_p$
        - Number of frames sent is w
        - $U = \frac{w*T_f}{T_f + 2T_p}$
- Error case
    - $U=P_s$ if w greater than $1+2a$
    - $U=\frac{w*P_s}{1+2a}$
---
Links: 