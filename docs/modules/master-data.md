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

