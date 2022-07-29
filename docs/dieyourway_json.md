---
title: DieYourWay JSON
date: 2021-04-05
---
# DieYourWay JSON Format

This is the format of a JSON file describing a dieyourway file. They need to be placed inside the `dieyourway` folder within your namespace.

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`loading_order` | [Integer](https://origins.readthedocs.io/en/latest/types/data_types/integer/) | `2147483647` | Specifies when this death message is loaded in the death message randomiser. Lower numbers mean the file is loaded earlier which allows overriding to be controlled.
`damage_condition` | [Damage Condition](https://origins.readthedocs.io/en/latest/types/damage_condition_types/) | _optional_ | If set, the messages in this message file  will only have a chance to display when the damage source that causes the death of a player fulfills the condition.
`bientity_condition` | [Bi-entity Condition](https://origins.readthedocs.io/en/latest/types/bientity_condition_types/) | _optional_ | If set, the messages in this message file will only have a chance to display when this bi-entity condition is met by the attacker as the actor and dead entity as the actor.
`condition` | [Entity Condition](entity_conditions.md) | _optional_ | If set, the messages in this message file will only have a chance to display when a player that dies fulfills the condition.
`messages` | [Array](https://origins.readthedocs.io/en/latest/types/data_types/array/) of [Strings](https://origins.readthedocs.io/en/latest/types/data_types/string/) | | The messages that have a chance to display upon meeting any specified condition in this file.
`arguments` | [Array](https://origins.readthedocs.io/en/latest/types/data_types/array/) of [Arguments](arguments.md) | | Any arguments that are to be used in the death message. To access these arguments place `%X$s` in your message string where the normal JSON syntax would go. X being the index of the argument 
`override` | [Boolean](https://origins.readthedocs.io/en/latest/types/data_types/boolean/) | `false` | Determines if this file is the only one considered in the death message randomiser when loaded.