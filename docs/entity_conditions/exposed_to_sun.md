---
title: Exposed to Sun
date: 2021-08-02
---
# Exposed to Sun

[Entity Condition](../entity_conditions.md).

```
NOTICE: This condition is not included in 1.0.0 of DieYourWay.
```

Checks whether the player is currently exposed to the sun. Essentially a [Brightness](../entity_conditions/brightness) check for `brightness > 0.5` combined with and an [Exposed to Sky](../entity_conditions/exposed_to_sky) check.

Type ID: `apoli:exposed_to_sun`

### Fields:

_None._

### Example:
```json
"condition": {
    "type": "apoli:exposed_to_sun"
}
```