---
title: Category (Condition)
date: 2021-08-02
---
# Category

[Biome Condition](../biome_conditions.md).

Checks for the category of a biome.

Type ID: `dieyourway:category`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`category` | [String](../data_types/string.md) | |  Which category the biome must be in order to succeed the check. See the [list of biome categories](../misc/biome_categories.md).

### Example:
```json
"condition": {
    "type": "dieyourway:biome",
    "condition": {
        "type": "dieyourway:category",
        "category": "forest"
    }
}
```
This example checks if the player is inside a Forest-like biome.