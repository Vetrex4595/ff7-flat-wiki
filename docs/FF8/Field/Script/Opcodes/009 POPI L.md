---
title: 009 POPI L
---

[Home](/Main%20Page.md) > [FF8](/FF8.md) > [Field](/FF8/Field.md) > [Script](/FF8/Field/Script.md) > [Opcodes](/FF8/Field/Script/Opcodes.md) > 009 POPI L

-   Opcode: **0x009**
-   Short name: **POPI\_L**
-   Long name: Pop to Temp List (long)

#### Argument

Index position in the Temp List (0 &lt;= **Argument** &lt; 8).

#### Stack

..., *value* =&gt; ...

#### Description

Pop the top *value* from the stack and store the first four bytes (long)
at index position **Argument** in the Temp List.