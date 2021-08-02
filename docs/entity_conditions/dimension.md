---
title: Dimension
date: 2021-08-02
---
# Dimension

[Entity Condition](../entity_conditions.md).

Checks whether the player is in a specified dimension.

Type ID: `dieyourway:dimension`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`dimension` | [Identifier](../data_types/identifier.md) | |  ID of the dimension the player needs to be in for this condition to evaluate to true. Vanilla dimensions are `minecraft:overworld`, `minecraft:the_nether` and `minecraft:the_end`, but IDs of custom/modded dimensions should also work.

### Example
```json
"condition": {
    "type": "dieyourway:dimension",
    "dimension": "minecraft:overworld",
    "inverted": true
}
```
This example checks if the player is **not** in the Overworld dimension.