---
title: Attacker (Argument)
date: date: 2021-08-02
---
# Attacker

[Argument Type](../argument_types.md).

Outputs the attacker's name in JSON format. This results in `{\"text:\":\"Attacker\"}` if there is no attacker.

Type ID: `dieyourway:attacker`

### Example:
```json
"arguments": [
    {
        "type": "dieyourway:attacker"
    }
]
```
This example would replace any instance of %1$s in a death message with the attacker's name.