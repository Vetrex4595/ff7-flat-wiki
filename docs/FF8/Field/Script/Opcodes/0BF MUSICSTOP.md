---
title: 0BF MUSICSTOP
---

[Home](/Main%20Page.md) > [FF8](/FF8.md) > [Field](/FF8/Field.md) > [Script](/FF8/Field/Script.md) > [Opcodes](/FF8/Field/Script/Opcodes.md) > 0BF MUSICSTOP

-   Opcode: **0x0BF**
-   Short name: **MUSICSTOP**
-   Long name: Stop Music

#### Argument

none

#### Stack

  
*0 or 1*

**MUSICSTOP**

#### Description

Presumably stops the music from playing. There are some points where
MUSICSTOP is called twice in a row like this:

  
PSHN\_L 1

MUSICSTOP

PSHN\_L 0

MUSICSTOP