---
title: Offset (Condition)
date: 2021-08-02
---
# Offset

[Block Condition](../block_conditions.md).

A meta-condition which instead checks the provided [Block Condition](../block_conditions.md) at a position offset from the current position.

Type ID: `dieyourway:offset`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`condition` | [Block Condition](../block_conditions.md) | | The condition to check with the given offset.
`x` | [Integer](../data_types/integer.md) | `0` |  How much to offset the position on the x-axis.
`y` | [Integer](../data_types/integer.md) | `0` |  How much to offset the position on the y-axis.
`z` | [Integer](../data_types/integer.md) | `0` |  How much to offset the position on the z-axis.

### Example:
```json
"block_condition": {
    "type": "dieyourway:offset",
    "condition": {
        "type": "dieyourway:block",
        "block": "minecraft:grass_block"
    },
    "y": 1
}
```
This example checks if the block above the block is a grass block.