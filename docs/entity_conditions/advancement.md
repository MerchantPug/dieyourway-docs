---
title: Advancement (Condition)
date: date: 2021-08-02
---
# Advancement

[Entity Condition](../entity_conditions.md).

Checks whether the player has completed a specified advancement.

Type ID: `dieyourway:advancement`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`advancement` | [Identifier](../data_types/identifier.md) | | ID of the advancement the player needs to have completed in order for this condition to evaluate to true.

### Example:

```json
"condition": {
  "type": "dieyourway:advancement",
  "advancement": "minecraft:story/smelt_iron"
}
```
This condition added to a power will make it only activate after the player has smelted or found their first iron ingot.
