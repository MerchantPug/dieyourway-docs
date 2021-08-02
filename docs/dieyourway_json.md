---
title: DieYourWay JSON
date: 2021-04-05
---
# DieYourWay JSON Format

This is the format of a JSON file describing a dieyourway file. They need to be placed inside the `dieyourway` folder within your namespace.

### Fields

Field  | Type | Default | Description
-------|------|---------|-------------
`loading_order` | [Integer](data_types/integer.md) | `2147483647` | Specifies when this death message is loaded in the death message randomiser. Lower numbers mean the file is loaded earlier which allows overriding to be controlled.
`damage_condition` | [Damage Condition](damage_conditions.md) | _optional_ | If set, this message will only have a chance to display when the damage source that causes the death of a player fulfills the condition.
`condition` | [Entity Condition](entity_conditions.md) | _optional_ | If set, this message will only have a chance to display when a player that dies fulfills the condition.
`messages` | [Array](data_types/array.md) of [Strings](data_types/string.md) | | The messages that have a chance to display upon meeting any specified condition in this file.
`arguments` | [Array](data_types/array.md) of [Arguments](arguments.md) | | Any arguments that are to be used in the death message. To access these arguments place %X$s in your message string where the normal JSON syntax would go. X being the index of the argument 
`override` | [Boolean](data_types/boolean.md) | `false` | Determines if this file is the only one considered in the death message randomiser when loaded.