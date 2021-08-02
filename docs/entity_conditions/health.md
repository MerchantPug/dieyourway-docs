---
title: Health
date: 2021-08-02
---
# Health

[Entity Condition](../entity_conditions.md).

Checks the current health (absolute value) of the player.

Type ID: `dieyourway:health`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`comparison` | [Comparison](../data_types/comparison.md) | | How the health of the player should be compared to the specified value.
`compare_to` | [Float](../data_types/float.md) | | Which value the health should be compared to.

### Example:
```json
"condition": {
    "type": "dieyourway:health",
    "comparison": "<",
    "compare_to": 20
}
```
This example checks if the player's health is less than 10 hearts (or 20 health points), which is the default value for the player's max health.