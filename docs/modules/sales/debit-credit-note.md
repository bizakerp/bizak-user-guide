# Debit and Credit Note

This page covers the debit and credit note flow.
Use it when you need a formal adjustment against an earlier sale.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `note_number` | Note number |
| `note_type` | Debit or credit note type |
| `note_against` | Source note type |
| `reason` | Adjustment reason |
| `adjustment_basis` | Adjustment basis |
| `party_id` | Customer or party |
| `issue_date` | Issue date |
| `due_date` | Due date |
| `approval_date` | Approval date |
| `approved_status` | Approval status |
| `form_status` | Form status |
| `gross_amount` | Gross amount |
| `discount_amount` | Discount amount |
| `taxable_amount` | Taxable amount |
| `tax_amount` | Tax amount |
| `net_total` | Net total |
| `currency_name` | Currency |
| `exchange_rate` | Exchange rate |
| `ledger_name` | Ledger |
| `tax_ledger_name` | Tax ledger |
| `accounting_period` | Accounting period |
| `is_posted_to_gl` | Posted to GL flag |
| `posting_date` | Posting date |
| `entity_ref_id` | Entity reference |
| `entity_type` | Entity type |
| `reference_from` | Reference source |
| `location_name` | Location |
| `subsidiary_name` | Subsidiary |
| `project_name` | Project |
| `department_name` | Department |
| `class_name` | Class |
| `sales_rep_name` | Sales rep |
| `memo` | Notes |
| `notes` | Extra notes |
| `purpose` | Purpose |
| `attachments_json` | Attachment data |
| `print_count` | Print count |
| `version` | Version |
| `affects_inventory` | Inventory impact flag |
| `is_linked_to_return` | Linked to return flag |
| `return_authorization_id` | Return authorization |
| `details` | Line items |
| `invoice_references` | Invoice references |

The detail lines can hold item, unit, serial number, description, quantity, rate, discount, tax, and stock detail data.

## Example

A customer asks for a formal note after a pricing dispute.
The note is linked to the original invoice.
The accounting team reviews the amount before it is posted.

