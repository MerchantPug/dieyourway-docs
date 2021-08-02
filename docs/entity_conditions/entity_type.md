---
title: Entity Type
date: 2021-08-02
---
# Entity Type

[Entity Condition](../entity_conditions.md).

Checks whether the entity is of a specific entity type.

Type ID: `dieyourway:entity_type`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`entity_type` | [Indentifier](../data_types/identifier.md) | |  ID of the entity type the entity needs to have to pass the check.

### Example
```json
"condition": {
    "type": "dieyourway:entity_type",
    "entity_type": "minecraft:creeper"
}
```
This example checks if the entity is a Creeper.