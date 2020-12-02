---
title: 07 RETTO
---

[Home](/Main%20Page.md) > [FF7](/FF7.md) > [Field](/FF7/Field.md) > [Script](/FF7/Field/Script.md) > [Opcodes](/FF7/Field/Script/Opcodes.md) > 07 RETTO

-   Opcode: **0x07**
-   Short name: **RETTO**
-   Long name: Return To

#### Memory layout

| 0x07 | *P / F* |
|------|---------|

#### Arguments

-   **const Bit\[3\]** *P*: The [priority][] at which we want to execute
    the remote script (high 3 bits of byte).
-   **const Bit\[5\]** *F*: The ID of the specific member function of
    the current entity to be executed to (low 5 bits of byte).

#### Description

Stops the active script loop for this entity and also any script loops
(except the main) that are queuing to be executed after the current
script. This is essentially the same as adding a RET onto each of the
active / queued scripts next execution position and returning the
current op index to index for each script.

THEN the script control is passed to the script *F* within the current
entity with the priority *P*.

  [priority]: /FF7/Field/Script/Priorities.md "wikilink"