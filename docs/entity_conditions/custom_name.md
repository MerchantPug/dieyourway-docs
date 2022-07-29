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
`name` | [String](https://origins.readthedocs.io/en/latest/data_types/string/) | | The name to check for on the entity. This ignores any other NBT and only goes for the name.
`case_sensitive` | [Boolean](https://origins.readthedocs.io/en/latest/types/data_types/boolean/) | `true` | Whether the check is case sensitive (capitalisation matters).

### Example:
```json
"condition": {
    "type": "dieyourway:custom_name",
    "name": "string"
}
```
This example checks if the entity's name is **string**.