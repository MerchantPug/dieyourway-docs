---
title: Precipitation (Condition)
date: 2021-08-02
---
# Precipitation

[Biome Condition](../biome_conditions.md).

Checks for the precipitation type of a biome.

Type ID: `dieyourway:precipitation`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`precipitation` | [String](../data_types/string.md) | |  Which precipitation the biome has to have in order to succeed the check. One of `none`, `rain` and `snow`.

### Example:
```json
"condition": {
    "type": "dieyourway:biome",
    "condition": {
        "type": "dieyourway:precipitation",
        "precipitation": "snow"
    }
}
```
This example checks if the biome the player is currently in has a snowy precipitation. (e.g: `minecraft:snowy_taiga`, `minecraft:ice_spikes`, etc.)