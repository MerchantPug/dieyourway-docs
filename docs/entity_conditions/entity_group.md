---
title: Entity Group (Condition)
date: 2021-08-02
---
# Entity Group

[Entity Condition](../entity_conditions.md).

Checks whether the entity is of a specific entity group.

Type ID: `dieyourway:entity_group`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`group` | [String](../data_types/string.md) | |  Entity group required for the entity to pass the check. One of `default`, `undead`, `arthropod`, `illager` and `aquatic`.

### Example
```json
"condition": {
    "type": "dieyourway:entity_group",
    "group": "undead"
}
```
This example checks if the entity is included in the [`undead entity group`](../power_types/entity_group.md).