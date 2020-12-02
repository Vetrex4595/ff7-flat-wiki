---
title: 7B INC2!
---

[Home](/Main%20Page.md) > [FF7](/FF7.md) > [Field](/FF7/Field.md) > [Script](/FF7/Field/Script.md) > [Opcodes](/FF7/Field/Script/Opcodes.md) > 7B INC2!

-   Opcode: **0x7B**
-   Short name: **INC2!**
-   Long name: Saturated Increment (16-bit)

#### Memory layout

| 0x7B | *0/D* | *Dest* |
|------|-------|--------|

#### Arguments

-   **const Bit\[4\]** *D*: Destination bank
-   **const UByte** *Dest*: The destination address in the bank where
    the variable is incremented.

#### Description

Increments the value in â€œDestâ€ by 1. The result is capped at 32767.