# Master Data

Master data is the shared foundation that Bizak transactions depend on.

If master data is incomplete or inconsistent, users may run into blocked forms, missing dropdown values, or incorrect postings.

## Key master data areas

| Component | What it is | Why it matters |
| --- | --- | --- |
| Item | Goods or services sold, purchased, or tracked in stock | Drives sales, procurement, inventory, and costing |
| Unit | Measurement standard such as piece, kg, or box | Ensures quantity consistency across transactions |
| Item Category | Classification for reporting and rules | Supports grouping, pricing, taxes, and inventory control |
| Ledger | Financial account used for accounting postings | Required for accurate journal impact and financial reports |
| Ledger Group | Higher-level grouping for ledgers | Supports structured reporting and account organization |
| Withhold Tax | Tax deducted at source rules | Automates tax withholding on vendor or service payments |
| Brand | Manufacturer or brand reference | Supports segmentation and analysis |
| Relation | Business contact type such as customer or vendor | Connects business parties to sales, purchase, payroll, or support workflows |

## Item setup

The item model in the codebase includes these core fields:

| Field | Meaning |
| --- | --- |
| `item_name` | Display name of the item |
| `item_code` | Unique code for the item |
| `standard_unit_name` | Base unit used for the item |
| `item_type_name` | Inventory or non-inventory type name |
| `item_sub_type` | More specific item behavior |
| `purchase_unit_name` / `sales_unit_name` | Units used in purchasing or sales |
| `category_name` | Item category |
| `brand_name` | Brand or manufacturer |
| `tax_name` | Tax setup |
| `wh_tax_code` | Withholding tax code |
| `income_account_name` / `expense_account_name` | Accounting linkage |
| `asset_account_name` | Asset account for fixed assets |
| `cogs_account_name` | Cost of goods sold account |
| `purchase_description` / `sales_description` | Default item descriptions |
| `is_maintain_stock` | Turns stock tracking on or off |
| `is_multiple_uom` | Enables multiple unit of measure fields |
| `is_fixed_assets` | Marks the item as a fixed asset |
| `is_serialized` / `is_batch_no` | Enables serial or batch tracking |
| `is_track_landed_cost` | Enables landed cost handling |
| `is_allow_negetive_stock` | Allows negative stock if enabled |
| `default_discount_amount` / `default_discount_percentage` | Default discount rules |

## Item behavior rules

When stock tracking is on, the item needs a unit.
When a fixed asset flag is on, stock behavior changes.
When multiple UOM is on, the item can use more than one unit field.
If the item is not stock-tracked, the form can allow service or discount-style behavior.

## Example item types

| Example | Why it fits |
| --- | --- |
| Printer stock item | It needs quantity, rate, and inventory control |
| Consulting service | It needs accounting but not stock |
| Office laptop | It is a fixed asset |
| Bundle or kit | The child items carry the accounting or stock detail |

## Customer setup

The customer DTO includes the following real fields:

| Field | Meaning |
| --- | --- |
| `full_name` | Customer name |
| `code` | Customer code |
| `personal_email` | Email address |
| `permanent_address` | Main address |
| `secondary_address` | Extra address field |
| `primary_contact` | Main contact number |
| `secondary_contact` | Extra contact number |
| `pan_no` / `vat_no` | Tax identity numbers |
| `login_email` | Login email if the customer is also a portal user |
| `opening_balance` | Opening balance |
| `customer_type` | Customer classification |
| `branch_ids` | Branch access or ownership |
| `area_id` | Geographic area |
| `latitude` / `longitude` | Location coordinates |

## Vendor setup

The vendor DTO includes these important fields:

| Field | Meaning |
| --- | --- |
| `company_name` | Vendor company name |
| `first_name` / `last_name` | Contact person names |
| `vendor_number` | Vendor code |
| `vendor_category_name` | Vendor category |
| `ledger_name` | Linked ledger |
| `term_name` | Payment term |
| `tax_name` | Tax setup |
| `with_tax_name` | Withholding tax setup |
| `shipping_address` | Delivery or shipping address |
| `pan` | Tax number |
| `email` / `phone` / `mobile_no` | Contact fields |
| `web_address` | Website |
| `industry` | Industry label |
| `is_inactive` / `is_banned` | Status controls |

## Employee setup

The employee DTO shows these important fields:

| Field | Meaning |
| --- | --- |
| `first_name` / `last_name` | Employee name parts |
| `full_name` | Display name |
| `code` | Employee code |
| `personal_email` / `login_email` | Email addresses |
| `primary_contact` / `secondary_contact` | Contact numbers |
| `designation_id` / `job_title` | Role or title |
| `department_name` | Department |
| `location_name` | Location |
| `supervisor_name` | Reporting manager |
| `is_sales_rep` / `is_support_rep` / `is_project_rep` | Functional flags |
| `purchase_limit` / `expenses_limit` | Control values |
| `purchase_approver` / `expenses_approver` / `time_approver` | Approval routing |
| `user_account_dto` | Linked user account data |

## Relationship records

Relationship entries use the shared DTO with these fields:

| Field | Meaning |
| --- | --- |
| `contact_no` | Required contact number |
| `job_title` | Job title |
| `email` | Email address |
| `phone` | Phone number |
| `entity_type` | Related Bizak entity type |
| `entity_ref_id` | Related record id |
| `role_type` | Relationship role such as decision maker |

## Item behavior examples

### Inventory item

An inventory item is used when you need stock tracking.

- maintain stock is enabled
- units become mandatory
- inventory-related fields are available
- ledger and costing logic become relevant

**Example:** a retail product such as a printer, carton, or raw material lot.

### Non-inventory item

A non-inventory item is used when stock tracking is not required.

- maintain stock is disabled
- the item type can be service, discount, kit, or similar non-stock behavior
- accounting is still relevant, but stock quantity is not

**Example:** consulting work, delivery service, or a discount line.

### Fixed asset

When an item is marked as a fixed asset, the form behavior changes.

- subtype behavior changes or disappears
- stock tracking is disabled
- landed cost handling becomes relevant
- some unit and brand behavior may be limited

**Example:** a company laptop or machine purchased for long-term use.

## Unit rules

- a unit code should be unique
- a unit used in transactions should not be deleted
- units should be standardized across the organization

**Example:** use `pcs`, `box`, `kg`, and `ltr` consistently instead of creating multiple variants for the same concept.

## Ledger rules

- ledgers are the backbone of accounting postings
- group ledgers can organize reporting but may not post transactions directly
- ledgers tied to actual transactions should be protected from deletion

**Example:** `Sales Revenue`, `Cost of Goods Sold`, and `Rent Expense` should be modeled as distinct ledgers.

## Relation types

| Type | Typical use |
| --- | --- |
| Lead | Unqualified prospect or potential contact |
| Prospect | Qualified sales opportunity |
| Customer | Active buyer |
| Vendor | Supplier or service provider |
| Partner | Distributor, collaborator, or strategic ally |
| Project | A scoped piece of work or engagement |
| Employee | Internal staff member |

## Recommended setup order

1. Create units
2. Create item categories
3. Create ledgers and ledger groups
4. Define tax or withholding rules
5. Create items
6. Create relation records
