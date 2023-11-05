---
tags:
  - 🌱
  - ComputerScience
date: 24--Feb--2023
---

# Ethernet frame

Manchester encoding. Uses similar format to [[Counter-based]] framing.
- Preamble has 8 bytes
    - 7 sync
    - 1 to mark start of frame
- Type/ Length
    - If value is less than 1500 then the field indicates length of frame
    - Else it indicate frame type

---
Links: 