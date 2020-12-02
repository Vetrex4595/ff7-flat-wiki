---
title: 06F AASK
---

[Home](/Main%20Page.md) > [FF8](/FF8.md) > [Field](/FF8/Field.md) > [Script](/FF8/Field/Script.md) > [Opcodes](/FF8/Field/Script/Opcodes.md) > 06F AASK

-   Opcode: **0x06F**
-   Short name: **AASK**
-   Long name: AAsk

#### Argument

none

#### Stack

  
*Message Channel*

*Field message ID*

*Line of first option*

*Line of last option*

*Line of default option*

*Line of cancel option*

*X position of window*

*Y Position of window*

**AASK**

#### Description

Opens a field message window and lets player choose a single line. AASK
saves the chosen line index (first option is always 0) into a temp
variable which you can retrieve with PSHI\_L 0.