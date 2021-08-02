---
title: Light Level (Condition)
date: 2021-08-02
---
# Light Level

[Block Condition](../block_conditions.md).

Allows checking the light level at the block's position.

Type ID: `dieyourway:light_level`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`light_type` | [String](../data_types/string.md) | _optional_ | The type of light level to compare. Either `sky` or `block`. If no type is provided, the greater value of the two types will be used, which is the "resulting" light level of that position.
`comparison` | [Comparison](../data_types/comparison.md) | | How the light level should be compared to the specified value.
`compare_to` | [Integer](../data_types/integer.md) | | The value to compare the light level at the block's position to.

### Example:
```json
"block_condition": {
    "type": "dieyourway:light_level",
    "light_type": "block",
    "comparison": ">",
    "compare_to": 10
}
```
This example checks if the light level at the specified position is emitted by a block, and more than 10.