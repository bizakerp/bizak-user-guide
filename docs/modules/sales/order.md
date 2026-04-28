# Order

This page covers the customer order flow.
Use it when the customer confirms the sale.

## Before you start

- Confirm the customer exists.
- Confirm the estimate or sales quote is ready if you use one.
- Confirm the items, prices, and taxes are set up.
- Confirm the user can create sales orders.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `order_number` | Order number |
| `party_name` | Customer name |
| `address` | Address |
| `secondary_address` | Alternate address |
| `date` | Order date |
| `memo` | Notes |
| `invoice_number` | Linked invoice number |
| `due_date` | Due date |
| `term_name` | Payment term |
| `mode` | Order mode |
| `location_name` | Location |
| `sales_representative` | Sales rep |
| `is_cancelled` | Cancel flag |
| `cancellation_reason` | Cancel reason |
| `class_name` | Class |
| `department_name` | Department |
| `currency_name` | Currency |
| `exchange_rate` | Exchange rate |
| `partner` | Partner |
| `booking_amount` | Booking amount |
| `down_payment_amount` | Down payment |
| `expected_delivery_date` | Expected delivery |
| `supplier_po` | Supplier PO reference |

The order also stores item details, notes, files, tasks, events, messages, and relationships.

## Related pages

- [Sales Overview](../sales.md)
- [Estimate](estimate.md)
- [Invoice](invoice.md)
- [Customer Receipt](../../payment/customer-receipt.md)

## Example

A customer approves a quote for office furniture.
Bizak records the order date, expected delivery date, and the booking amount.
The team then moves the order to fulfillment and invoice.
