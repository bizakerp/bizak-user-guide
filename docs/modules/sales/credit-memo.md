# Credit Memo

This page covers the credit memo flow.
Use it when the customer account needs a credit adjustment.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `credit_memo_no` | Credit memo number |
| `customer` | Customer name |
| `credit_memo_date` | Credit memo date |
| `memo` | Notes |
| `status` | Memo status |
| `currency_name` | Currency |
| `exchange_rate` | Exchange rate |
| `ref_invoice_id` | Linked invoice |
| `invoice_reference_no` | Invoice reference |
| `location_name` | Location |
| `department_name` | Department |
| `class_name` | Class |
| `project_name` | Project |
| `sales_rep_name` | Sales rep |
| `ledger_name` | Ledger |
| `job_no` | Job number |
| `credit` | Credit amount |
| `purpose` | Purpose |
| `customer_po_ref` | Customer PO reference |
| `promise_date` | Promise date |
| `contract_period` | Contract period |
| `kilometerage` | Kilometer value if used |
| `discount_item_id` | Discount item |
| `discount` | Discount |
| `item_rate` | Item rate |
| `unapplied` | Unapplied amount |
| `applied` | Applied amount |
| `auto_apply` | Auto apply flag |
| `service_type` | Service type |
| `order_type` | Order type |
| `ride_date` | Ride date |
| `car_details` | Car details |
| `payment_mode` | Payment mode |
| `pos_session_id` | POS session |
| `credit_memo_details` | Line details |

## Example

A customer is owed a credit after a pricing correction.
Bizak records the memo, links the invoice, and stores the credit amount.
The team can then apply the credit to a later invoice.

