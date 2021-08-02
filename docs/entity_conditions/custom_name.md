---
title: Custom Name (Entity Condition)
date: 2021-08-02
---
# Custom Name

[Entity Condition](../entity_conditions.md).

Checks if the entity's custom name is the specified string.

Type ID: `dieyourway:has_name`

### Fields:
Field  | Type | Default | Description
-------|------|---------|-------------
`name` | [String](../data_types/string.md) | | The name to check for on the entity. This ignores any other NBT and only goes for the name.


### Example:
```json
"condition": {
    "type": "dieyourway:custom_name",
    "name": "string"
}
```
This example checks if the entity's name is **string**.