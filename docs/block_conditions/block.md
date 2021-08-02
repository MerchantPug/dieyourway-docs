---
title: Block (Condition)
date: 2021-08-02
---
# Block

[Block Condition](../block_conditions.md).

Checks whether the block is a certain block (by ID).

Type ID: `dieyourway:block`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`block` | [String](../data_types/string.md) | | ID of the block that this block needs to be to pass the check.

### Examples:
```json
"block_condition": {
    "type": "dieyourway:block",
    "block": "minecraft:diamond_block"
}
```
This example checks if the block is a Diamond Block.

```json
"block_condition": {
    "type": "dieyourway:or",
    "conditions": [
        {
            "type": "dieyourway:block",
            "block": "minecraft:diamond_block"
        },
        {
            "type": "dieyourway:block",
            "block": "minecraft:emerald_block"
        }
    ]
}
```
This example checks if the block is either a Diamond Block or an Emerald Block, though using the [`dieyourway:in_tag`](../block_conditions/in_tag.md) block condition type would be better for checking multiple block types.