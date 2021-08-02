---
title: Using Item (Condition)
date: 2021-08-02
---
# Using Item

[Entity Condition](../entity_conditions.md).

Checks whether the player is using an item (holding right-click, as in drinking a potion or eating food).

Type ID: `dieyourway:using_item`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`item_condition` | [Item Condition](../item_conditions.md) | _optional_ | If specified, the condition will only pass if the item that is being used fulfills this condition.

### Example:

```json
"condition": {
  "type": "dieyourway:using_item",
  "item_condition": {
    "type": "dieyourway:food"
  }
}
```
Checks whether the entity is currently eating food.
