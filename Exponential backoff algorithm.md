---
tags: 🌱
date: 24--Feb--2023
---

# Exponential backoff algorithm

Protocol used when there is collision detected.
- First collision
    - Randomly picks a slot from $2^1$
- Second collision
    - Randomly picks slot form $2^2$
- For nth collision
    - Max number of slots is $2^{10}$
    - Gives up after 16 consecutive collision

---
Links: 