---
tags: 🌱
date: 23--Feb--2023
---

# Error detection

## CRC
Given a message, allocate k bits for error detection
-  Uses divisor polynomial theory
- If k=3, then there are 4 terms

- Sender
    - Transmit polynomial divisible by k bits represented by C(x)
    - Logical left shift message by k bits
    - Subtract remainder with $T(x)/C(x)$
        - Intuition is $x/y = r$
        - Then $(x-r)/y = 0$
- Receiver
    - Divide received polynomial by C(x)
    - Remainder zero implies
        - There is no error
        - Error not detected as it is evenly divisible

## Properties of C(x)
- Single bit errors detectable if $x^k$ and $x^0$ are non-zero coefficient
- Odd number of error detectable if C(x) has factor x+1

---
Links: 