# Adding Arguments to your files

Arguments are a way to specify specific text components that you couldn't get normally through text formatting such as the attacker, the attacker's item and the dead entity.

Let's say you have the file from the [Create File tutorial](create_file.md) (shown below).
```json
{
    "damage_condition": {
        "type": "dieyourway:name",
        "name": "sweetBerryBush"
    },
    "messages": [
        "\"This player who I won't be sharing the name of sucks!\"",
        "{\"text\":\"A player has become meesed\",\"bold\":true,\"color\":\"dark_red\"}"
    ]
}
```

To add arguments to the file, you'll have to write `%n$s` replacing the `n` with the index of the argument starting from 1 (not 0).

```json
{
    "damage_condition": {
        "type": "dieyourway:name",
        "name": "sweetBerryBush"
    },
    "messages": [
        "[\"\",%1$s,\" sucks!\"]",
        "[\"\",%1$s,{\"text\":\" has been meesed\",\"bold\":true,\"color\":\"dark_red\"}]"
    ],
    "arguments": [
        {
            "type": "dieyourway:dead_entity"
        }
    ]
}
```
This example will replace any instance of `%1$s` with text component relating to the dead entity.

```json
{
    "damage_condition": {
        "type": "dieyourway:name",
        "name": "sweetBerryBush"
    },
    "messages": [
        "[\"\",%1$s,{\"text\":\" has been meesed by \",\"bold\":true,\"color\":\"dark_red\"},%2$s]"
    ],
    "arguments": [
        {
            "type": "dieyourway:dead_entity"
        },
        {
            "type": "dieyourway:attacker"
        }
    ]
}
```
This example will replace any instance of `%1$s` with a text component relating to the dead entity and will replace any instance of `%2$s` with text relating to the attacker who killed said entity.

This concludes this tutorial, hopefully this explains how arguments are used within the mod.

### Related Pages
- [Argument Types](../argument_types.md)