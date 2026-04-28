# Order Type

This page covers POS order type setup.
Use it to define how a sale should behave.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `order_type_name` | Order type name |
| `order_type_code` | Order type code |
| `requires_table` | Table required flag |
| `print_kot` | Print KOT flag |
| `additional_charge` | Extra charge |
| `charge_type` | Charge type |
| `description` | Description |
| `is_active` | Active flag |
| `is_default` | Default flag |
| `display_order` | Sort order |

The route supports create, list, and update flows.

## Example

A restaurant uses one order type for dine-in and one for takeout.
The order type can control whether a table is needed and whether KOT prints.

