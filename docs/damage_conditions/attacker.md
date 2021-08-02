---
title: Attacker (Condition)
date: 2021-08-02
---
# Attacker

[Damage Condition](../damage_conditions.md).

Checks whether the condition has an attacker, and optionally whether the attacker fulfills a specified [Entity Condition](../entity_conditions.md).

Type ID: `dieyourway:attacker`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`entity_condition` | [Entity Condition](../entity_conditions.md) | _optional_ | If set, the attacking entity must fulfill the provided entity condition in order for this condition to evaluate to true.

### Example
```json
"damage_condition": {
    "type": "dieyourway:attacker",
    "entity_condition": {
        "type": "dieyourway:entity_type",
        "entity_type": "minecraft:zombie"
    }
}
```
This example checks if the attacker is a Zombie using the [`dieyourway:entity_type`](../entity_conditions/entity_type.md) entity condition type.