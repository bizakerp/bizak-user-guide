# Supplier Quotation

This page covers the supplier quotation flow.
Use it when you want a vendor quote before purchase.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `order_id` | Related order |
| `vendor_id` | Vendor |
| `address` | Vendor address |
| `contact_person` | Contact person |
| `date` | Quotation date |
| `base_period_id` | Base period |
| `vendor_bill` | Vendor bill reference |
| `memo` | Notes |
| `approver` | Approver |
| `approval_status` | Approval status |
| `next_approver` | Next approver |
| `term` | Payment term |
| `location_id` | Location |
| `department_id` | Department |
| `po_type` | Purchase type |
| `job_card_id` | Job card id |
| `job_card_no` | Job card number |
| `currency_id` | Currency |
| `exchange_rate` | Exchange rate |
| `subsidiary_id` | Subsidiary |
| `project_id` | Project |
| `organisation_id` | Organization |
| `order_details` | Line items |
| `lc_details` | LC details |
| `user_note_details` | Notes |
| `file_details` | Attachments |
| `relationship_details` | Related contacts |

## Example

A buyer requests a quote from a vendor for spare parts.
The quotation stores the vendor, the item lines, and the approval chain.
It can then be used before the purchase order is created.

