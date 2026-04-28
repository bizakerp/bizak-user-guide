# Transfer Order

This page covers the stock transfer order flow.
Use it when stock moves between locations.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `transfer_order_no` | Transfer order number |
| `source_location_id` | Source location |
| `destination_location_id` | Destination location |
| `transfer_order_date` | Transfer date |
| `employee_id` | Responsible employee |
| `approval_status` | Approval status |
| `transit_status` | Transit status |
| `is_firmed` | Firm transfer flag |
| `is_item_cost_as_transfer_cost` | Transfer cost flag |
| `incoterm` | Incoterm |
| `department_id` | Department |
| `class_id` | Class |
| `is_box_transfer` | Box transfer flag |
| `transfer_order_details` | Item lines |

## Example

A store sends stock to another branch.
The transfer order records the source, the destination, and the items.
The team can then track the stock while it is in transit.

