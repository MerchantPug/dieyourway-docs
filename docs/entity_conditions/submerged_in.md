---
title: Submerged In
date: 2021-08-02
---
# Submerged In

[Entity Condition](../entity_conditions.md).

Checks whether the player is submerged in a fluid of a specific tag (submerged means: eyes are inside that fluid).

Type ID: `dieyourway:submerged_in`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`fluid` | [Identifier](../data_types/identifier.md) | | ID of the fluid tag that should be checked. Most important examples: `minecraft:water` and `minecraft:lava`.

### Example:
```json
"condition": {
    "type": "dieyourway:submerged_in",
    "fluid": "minecraft:water"
}
```
This example checks if the player is submerged in water.