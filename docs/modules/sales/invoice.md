# Invoice

This page covers the sales invoice flow.
Use it when the sale is ready to post and collect.

## Before you start

- Confirm the customer and order are ready.
- Confirm the items and prices are correct.
- Confirm the user can post sales invoices.
- Confirm the payment and tax setup is ready.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `manual_no` | Manual number if used |
| `doc_no` | Document number |
| `invoice_number` | Invoice number |
| `party_name` | Customer name |
| `address` | Billing address |
| `secondary_address` | Alternate address |
| `date` | Invoice date |
| `memo` | Notes |
| `due_date` | Due date |
| `status` | Invoice status |
| `approved_status` | Approval status |
| `form_status` | Form status |
| `term_name` | Payment term |
| `location_name` | Location |
| `subsidiary_id` | Subsidiary |
| `sales_representative` | Sales rep |
| `payment_mode` | Payment mode |
| `class_name` | Class |
| `ledger_name` | Ledger |
| `discount` | Header discount |
| `project_name` | Project |
| `currency_name` | Currency |
| `exchange_rate` | Exchange rate |
| `department_name` | Department |
| `is_pos` | POS invoice flag |
| `pos_session_id` | POS session |
| `pos_auto_number_mode` | Auto number mode |
| `pos_tax_invoice_threshold` | Tax threshold |
| `order_type` | Order type |
| `ride_date` | Service or ride date |
| `car_details` | Vehicle details |
| `is_bill_discount` | Bill discount flag |
| `bill_discount_type` | Discount type |
| `counter_name` | Counter |
| `payment_method` | Payment method |
| `payment_type` | Payment type |
| `bank_name` | Bank name |
| `cheque_no` | Cheque number |
| `cheque_date` | Cheque date |
| `invoice_details` | Line items |
| `invoice_charge_list` | Extra charges |
| `payment_method_list` | Payment method list |

The invoice details include item, unit, quantity, rate, discount, tax, and amount.

## Related pages

- [Sales Overview](../sales.md)
- [Order](order.md)
- [Customer Receipt](../../payment/customer-receipt.md)
- [Sales Reports](../../reports/sales-reports.md)

## Example

A sales rep invoices a confirmed order.
The invoice shows the customer, the due date, the discount, and the line items.
If the sale came from POS, the invoice also carries the counter and session data.
