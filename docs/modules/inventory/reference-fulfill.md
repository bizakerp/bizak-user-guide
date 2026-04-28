# Reference Fulfillment

This page covers the reference fulfillment flow.
Use it when Bizak needs to fulfill stock from an earlier reference document.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `ref_type` | Source type |
| `ref_id` | Source id |
| `reference_fulfill_no` | Fulfillment number |
| `reference_from` | Source reference |
| `transit_status` | Transit status |
| `approval_status` | Approval status |
| `date` | Fulfillment date |
| `memo` | Notes |
| `remarks` | Remarks |
| `transport` | Transport method |
| `transport_amount` | Transport cost |
| `truck_no` | Truck number |
| `driver_name` | Driver name |
| `currency_id` | Currency |
| `exchange_rate` | Exchange rate |
| `location_id` | Source location |
| `destination_location_id` | Destination location |
| `department_id` | Department |
| `class_id` | Class |
| `requested_by` | Requester |
| `details` | Fulfillment lines |
| `inventory_details` | Inventory detail mapping |

## Example

A transfer or issue needs to be fulfilled from stock.
The fulfillment document stores the source reference and the item level mapping.
That keeps the stock trail traceable.

