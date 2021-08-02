---
title: Fluid Height
date: 2021-08-02
---
# Fluid Height

[Entity Condition](../entity_conditions.md).

Checks how high a specific fluid is at the player. A fluid height of 0 means the player is not touching the fluid.

Type ID: `dieyourway:fluid_height`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`fluid` | [Identifier](../data_types/identifier.md) | | ID of the fluid tag of which the height should be checked. Most important examples: `minecraft:water` and `minecraft:lava`.
`comparison` | [Comparison](../data_types/comparison.md) | | How the fluid height should be compared to the specified value.
`compare_to` | [Float](../data_types/float.md) | | Which value the fluid height should be compared to.

### Example:
```json
"condition": {
    "type": "dieyourway:fluid_height",
    "fluid": "minecraft:lava",
    "comparison": "==",
    "compare_to": 0
}
```
This example checks if the player is not touching a lava fluid.