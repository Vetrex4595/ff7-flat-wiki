---
title: A0 PC
---

[Home](/Main%20Page.md) > [FF7](/FF7.md) > [Field](/FF7/Field.md) > [Script](/FF7/Field/Script.md) > [Opcodes](/FF7/Field/Script/Opcodes.md) > A0 PC

-   Opcode: **0xA0**
-   Short name: **PC**
-   Long name: Playable Character

#### Memory layout

| 0xA0 | *C* |
|------|-----|

#### Arguments

-   **const UByte** *C*: Character ID.

#### Description

Defines the entity in which this script resides as a playable character.
The entity then becomes associated with the character ID *C*, including
the entity's visible object, animation set, and scripts. For example,
creating a visible entity and inserting PC(0) into its initialisation
script will associate this entity with character ID 0.