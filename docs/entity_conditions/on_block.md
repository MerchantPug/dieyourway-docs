---
title: On Block
date: 2021-08-02
---
# On Block

[Entity Condition](../entity_conditions.md).

Checks whether the player is standing on the ground, and optionally has a block that matches a specified block condition under them.

Type ID: `dieyourway:on_block`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`block_condition` | [Block Condition](../block_conditions.md) | _optional_ |  If set, a block that satisfies this block condition needs to be right below the player's feet.

### Example:

```json
"condition": {
  "type": "dieyourway:on_block",
  "block_condition": {
    "type": "dieyourway:block",
    "block": "minecraft:grass"
  }
}
```

This condition applied to a power will make sure it's only active while the player is on grass.
