---
title: 0CA SEPOSTRANS
---

[Home](/Main%20Page.md) > [FF8](/FF8.md) > [Field](/FF8/Field.md) > [Script](/FF8/Field/Script.md) > [Opcodes](/FF8/Field/Script/Opcodes.md) > 0CA SEPOSTRANS

-   Opcode: **0x0CA**
-   Short name: **SEPOSTRANS**
-   Long name: Sound Effect Pan Transition

#### Argument

none

#### Stack

  
*Sound channel*

*Frame count*

*Final pan (0-255)*

**SEPOSTRANS**

#### Description

Transitions the pan of the sound in *sound channel* over *frame count*.
0=left, 255=right.