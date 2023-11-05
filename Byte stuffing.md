---
tags:
  - 🌱
  - ComputerScience
date: 23--Feb--2023
---

# Byte stuffing

Connection for telephone line

- Frame starts with 01111110 (7E)
- 7D is used as escape character
- Data viewed as bytes instead of bits

## Algorithm
- Sender
    - Replaces 7E or 7D by inserting byte
    - 7E → 7D 5E
    - 7D → 7D 5D
- Receiver
    - Remove 7D and XOR 2nd bit with 0x20

---
Links: 