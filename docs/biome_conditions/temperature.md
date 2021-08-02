---
title: Temperature (Condition)
date: 2021-08-02
---
# Temperature

[Biome Condition](../biome_conditions.md).

Checks for the temperature of a biome.

Type ID: `dieyourway:temperature`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`comparison` | [Comparison](../data_types/comparison.md) | | How the temperature should be compared to the specified value.
`compare_to` | [Float](../data_types/float.md) | | Which value the temperature should be compared to.

### Example:
```json
"condition": {
    "type": "dieyourway:biome",
    "condition": {
        "type": "dieyourway:temperature",
        "comparison": ">=",
        "compare_to": 2
    }
}
```
This example checks if the biome the player is currently in has a temperature of 2 or more. (e.g: `minecraft:badlands`, `minecraft:desert`, etc.)