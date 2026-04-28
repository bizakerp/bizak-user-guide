# Field Reference

This page explains the most common fields used in Bizak.
It is a quick reference, not a full field list for every form.

## How to read fields

- Some fields are required.
- Some fields depend on role or setup.
- Some fields only appear on specific screens.
- Some values come from related master data such as items, ledgers, customers, or vendors.

## Common fields

| Field | Simple meaning | Typical use |
| --- | --- | --- |
| `status` | Current state of the record | Shows whether the record is open, posted, closed, or similar |
| `approval_status` | Approval state | Shows whether the record can be posted or needs review |
| `date` | Transaction date | Used for posting and reports |
| `posting_date` | Accounting date | Used when a document affects ledgers |
| `reference` | Source or document reference | Helps trace the record later |
| `reference_from` | Source text or document source | Links one record to another |
| `ref_type` | Source document type | Tells the system which workflow created the record |
| `ref_id` | Source document id | Links to the exact source record |
| `memo` | Short note | Stores a simple explanation |
| `currency_name` | Currency used | Supports multi-currency records |
| `exchange_rate` | Currency conversion rate | Converts values when currency changes |
| `department_name` | Department label | Tracks results by department |
| `class_name` | Class label | Adds another reporting split |
| `project_name` | Project label | Ties the record to a project |
| `location_name` | Location label | Tracks branch, store, or warehouse use |
| `source_location` | Source warehouse | Shows where stock comes from |
| `destination_location_id` | Destination warehouse | Shows where stock goes |
| `ledger_name` | Linked ledger | Connects the record to accounting |
| `account_name` | Account label | Used on finance and adjustment screens |
| `item_name` | Item label | Identifies the product or service line |
| `unit_name` | Unit label | Shows the unit used for quantity |
| `customer` | Customer record | Used in sales and receipt flows |
| `vendor_name` | Vendor record | Used in procurement and payment flows |
| `payment_mode` | Method of payment | Used for cash, bank, cheque, or transfer |
| `order_type_name` | POS order type | Separates dine-in, takeout, or other POS flows |

## Typical field groups

### Identity fields

These fields tell the system what the record is.

- code
- number
- name
- type
- category

### Link fields

These fields point to another record.

- customer
- vendor
- item
- ledger
- location
- project
- department

### Control fields

These fields affect behavior.

- status
- approval status
- active or inactive
- tax settings
- stock settings
- payment settings

### Tracking fields

These fields help users trace a record later.

- reference
- memo
- date
- posting date
- created by
- updated by
- workflow history

## Example by screen

### Sales invoice

Common fields usually include:

- customer
- invoice date
- reference
- currency
- item lines
- tax
- payment terms

### Purchase order

Common fields usually include:

- vendor
- order date
- reference
- delivery date
- item lines
- location
- currency

### Journal entry

Common fields usually include:

- date
- reference
- ledger lines
- department
- project
- memo

### Inventory adjustment

Common fields usually include:

- date
- location
- item
- quantity
- reason
- account

## Quick tips

- Use the same reference format across the team.
- Keep dates in the format set in company preferences.
- Check the linked master record when a dropdown is empty.
- Use a ledger or account name that matches finance setup.
