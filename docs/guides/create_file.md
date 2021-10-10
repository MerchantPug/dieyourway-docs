# Creating a Basic Death Message File
`Please note that this guide assumes that you have at least some knowledge with Apoli/Origins' systems. If you are completely new to these datapack systems my recommendation would be reading up on the Origins documentation.`

Death messages are defined in JSON files. They work off Apoli's damage, bientity and entity conditions to determine if they should be displayed. Say we would like to make a new death message that sends an insult in chat when a player die to berry bushes, the message would go like this.

The messages field uses Minecraft's Raw JSON Text Format and supports multiple messages. Make sure to use `\"` if you are wanting to use `"` in a message otherwise your quotes may end early resulting in an error.

```json
{
    "damage_condition": {
        "type": "dieyourway:name",
        "name": "sweetBerryBush"
    },
    "messages": [
        "\"This player who I won't be sharing the name of sucks!\""
    ]
}
```
![Result Image for Example #1](https://i.imgur.com/1G2q9YZ.png)

Something of note here is that you should use the `dieyourway` namespace whenever calling a condition as it'll allow for compatibility between when Apoli is installed and when it is not installed. Otherwise if you're using conditions from an Apoli/Origins addon it's fine to use their namespace.

If you would like a randomised choice between 2 or more messages in your message file. You are able to add another message into the "messages" field, such as below.
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

When this file's conditions are met on death the mod now has a chance to select between these messages to replace the default death message. If any other files have a condition that is met they too have a chance to display alongside these ones.

This specific tutorial is now concluded. If you'd like to understand more about DieYourWay's systems, your next step would be [Arguments](arguments.md)

### Related Pages
[DieYourWay JSON Format](../dieyourway_json.md)
[Damage Conditions (Origins Wiki)](https://origins.readthedocs.io/en/latest/damage_conditions/)
[Bi-entity Conditions (Origins Wiki)](https://origins.readthedocs.io/en/latest/bientity_conditions/)
[Entity Conditions](../entity_conditions.md)
[Raw JSON Text Format (Minecraft Wiki)](https://minecraft.fandom.com/wiki/Raw_JSON_text_format)
[Raw JSON Text Format Generator](https://www.minecraftjson.com/)