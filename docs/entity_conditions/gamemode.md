---
title: Gamemode (Condition)
date: 2021-08-02
---
# Gamemode

[Entity Condition](../entity_conditions.md).

Checks the gamemode of a player. Will return false if the entity is not a player.

Type ID: `dieyourway:gamemode`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`gamemode` | [String](../data_types/string.md) | | Name of the gamemode the player should have in order for this condition to evaluate to true.

### Example:

```json
"condition": {
  "type": "dieyourway:gamemode",
  "gamemode": "creative"
}
```
This condition will only pass on players which are in creative mode.
