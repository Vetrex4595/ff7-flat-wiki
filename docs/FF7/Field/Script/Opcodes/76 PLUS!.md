---
title: 76 PLUS!
---

[Home](/Main%20Page.md) > [FF7](/FF7.md) > [Field](/FF7/Field.md) > [Script](/FF7/Field/Script.md) > [Opcodes](/FF7/Field/Script/Opcodes.md) > 76 PLUS!

-   Opcode: **0x76**
-   Short name: **PLUS!**
-   Long name: Saturated Addition (8-bit)

#### Memory layout

| 0x76 | *D/S* | *Dest* | *Oper* |
|------|-------|--------|--------|

#### Arguments

-   **const Bit\[4\]** *D*: Destination bank
-   **const Bit\[4\]** *S*: Source bank
-   **const UByte** *Dest*: The destination variable, to which the
    operand is added.
-   **const UByte** *Oper*: The operand, added to the destination.

#### Description

Adds two numbers together and stores the result back into "Dest". The
result of the addition is capped at 255. If the Source Bank is 0 then
the â€œOperâ€ is added to the destination value. If the Source Bank is
an 8 bit bank, then the â€œOperâ€ is the address in that bank where the
operand is.