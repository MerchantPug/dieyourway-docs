---
title: Attacker Item (Argument)
date: date: 2021-08-02
---
# Attacker Item

[Argument Type](../argument_types.md).

Outputs the item the attacker used to kill the entity. This results in `{\"text:\":\"[ItemStack]\"}` if there is no attacker. If the attacking entity isn't a LivingEntity it results in `{\"text:\":\"[Air]\"}`

Type ID: `dieyourway:attacker_item`

### Example:
```json
"arguments": [
    {
        "type": "dieyourway:dead_entity"
    },
    {
        "type": "dieyourway:attacker"
    },
    {
        "type": "dieyourway:attacker_item"
    }
]
```
This example would replace any instance of %3$s in a death message with the item an attacker used to kill an entity.