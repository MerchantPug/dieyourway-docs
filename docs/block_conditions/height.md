---
title: Height (Condition)
date: 2021-08-02
---
# Height

[Block Condition](../block_conditions.md).

Compares the y position of the block to a value.

Type ID: `dieyourway:height`

### Fields:

Field  | Type | Default | Description
-------|------|---------|-------------
`comparison` | [Comparison](../data_types/comparison.md) | | How the Y position of the block should be compared to the specified value.
`compare_to` | [Float](../data_types/float.md) | | The value to compare the Y position of the block to.

### Example:
```json
"block_condition": {
    "type": "dieyourway:height",
    "comparison": "<=",
    "compare_to": 11
}
```
This example checks if the block is within Y=11 or lower.