---
title: Dead Entity (Argument)
date: date: 2021-08-02
---
# Dead Entity

[Argument Type](../argument_types.md).

Outputs the player that died's name.

Type ID: `dieyourway:dead_entity`

### Example:
```json
"arguments": [
    {
        "type": "dieyourway:attacker"
    },
    {
        "type": "dieyourway:dead_entity"
    }
]
```
This example would replace any instance of %2$s in a death message with the player that just died's name.