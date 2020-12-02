---
title: E0 BGON
---

[Home](/Main%20Page.md) > [FF7](/FF7.md) > [Field](/FF7/Field.md) > [Script](/FF7/Field/Script.md) > [Opcodes](/FF7/Field/Script/Opcodes.md) > E0 BGON

-   Opcode: **0xE0**
-   Short name: **BGON**
-   Long name: Background On

#### Memory layout

| 0xE0 | *B1 / B2* | *A* | *L* |
|------|-----------|-----|-----|

#### Arguments

-   **const Bit\[4\]** *B1*: Bank to retrieve *A*, or zero if *A* is
    specified as a literal.
-   **const Bit\[4\]** *B2*: Bank to retrieve *L*, or zero if *L* is
    specified as a literal.
-   **const UByte** *A*: The ID of the background area to manipulate, as
    specified in the background's sprite.
-   **const UByte** *L*: The ID of the layer of *L* to display (turn
    on), as specified in the background's sprite.

#### Description

Turns on the portion of background whose [background sprite][] belongs
to the scripted area and state specified.

Parts of the background image (or more accurately, specific sprites) may
be assigned a "scripted area" that allows control over that portion of
the background by the scripting system. Within each scripted area,
backgrounds are drawn on top of each other in layers, on the same
location; these can represent a door in both open and closed states, for
example, allowing the script to switch between an open door when a
trigger is crossed and a closed door otherwise by simply [turning off][]
the "closed door" background and turning on the "open door" background.

  [background sprite]: /FF7/Field/Sprite.md "wikilink"
  [turning off]: /FF7/Field/Script/Opcodes/E1%20BGOFF.md "wikilink"