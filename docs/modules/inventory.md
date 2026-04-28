# Inventory

The Inventory module manages stock movement and inventory accuracy.

## Before you start

- Confirm items and units are set up.
- Confirm locations exist.
- Confirm the user has inventory access.
- Confirm the stock rules for batch or serial tracking are clear.

## Main routes in the app

| Route | Purpose |
| --- | --- |
| `transfer-order` | Move stock from one location to another |
| `fulfillment` | Confirm a reference fulfillment |
| `inventory-adjustment` | Correct stock on hand |
| `batch` | Manage batch data |
| `serial-number` | Manage serial data |
| `expiry-dashboard` | View expiring items |
| `expiry-report` | Review expiry data |

## Related pages

- [Master Data](master-data.md)
- [Transfer Order](inventory/transfer-order.md)
- [Reference Fulfillment](inventory/reference-fulfill.md)
- [Inventory Adjustment](inventory/inventory-adjustment.md)
- [Inventory Reports](../reports/inventory-reports.md)

## Transfer order

The transfer order DTO includes:

| Field | Meaning |
| --- | --- |
| `transfer_order_no` | Transfer order number |
| `source_location_id` | Source warehouse |
| `destination_location_id` | Destination warehouse |
| `transfer_order_date` | Transfer date |
| `is_firmed` | Firm transfer flag |
| `is_item_cost_as_transfer_cost` | Cost handling flag |
| `incoterm` | Incoterm text |
| `employee_id` | Responsible employee |
| `approval_status` | Approval status |
| `transit_status` | Transit status |
| `transfer_order_details` | Item lines |

## Reference fulfill

The reference fulfill DTO includes:

| Field | Meaning |
| --- | --- |
| `ref_type` | Source entity type |
| `ref_id` | Source record id |
| `reference_fulfill_no` | Fulfill document number |
| `transit_status` | Transit status |
| `location_id` | Source location |
| `destination_location_id` | Destination location |
| `requested_by` | Requester |
| `details` | Fulfillment lines |
| `inventory_details` | Inventory detail mapping |

## Inventory adjustment

The inventory adjustment DTO includes:

| Field | Meaning |
| --- | --- |
| `inventory_adjustment_no` | Adjustment number |
| `adjustment_date` | Adjustment date |
| `account_name` | Adjustment account |
| `location_name` | Location |
| `memo` | Notes |
| `requisition_reference` | Source reference |
| `adjustment_details` | Item adjustment lines |
| `inventory_detail_maps` | Item-level stock detail mapping |

## Detailed pages

- [Transfer Order](inventory/transfer-order.md)
- [Reference Fulfillment](inventory/reference-fulfill.md)
- [Inventory Adjustment](inventory/inventory-adjustment.md)

## Batch and serial tracking

The item model supports both batch and serial flags.
The guide should explain these features when the relevant item is configured for them.

## Expiry tracking

The inventory report routes include expiry dashboard and expiry report pages.
That means the system supports item expiry review for configured items.

## Example

If physical stock does not match the system, record an inventory adjustment so the quantity and reports stay accurate.

## Practical note

Inventory records can also carry files, notes, relationships, tasks, events, and messages.
That helps teams trace stock movement with context.
