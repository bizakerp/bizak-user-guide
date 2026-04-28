# Shared Transaction Tools

Bizak includes shared tools that appear across many transaction screens.

These tools help users review, print, and trace documents after they are created.

## Main routes in the app

| Route | Purpose |
| --- | --- |
| `transaction-shared/item-receipt` | Shared item receipt screen |
| `transaction-shared/print-preview` | Print preview screen |

## Why this section matters

Many Bizak transactions share the same support features.
Those features include notes, files, related records, workflow history, and print output.

## Common shared tools

| Tool | What it does |
| --- | --- |
| Files | Attach supporting documents |
| User notes | Leave internal notes |
| Relationships | Store related contacts or references |
| Workflow history | Review the path a record took |
| Related record | Jump to linked documents |
| Print preview | Review the printed output before printing |
| System information | Show document metadata |
| System note | Store record-level note text |

## Item receipt

The shared item receipt model includes these fields:

| Field | Meaning |
| --- | --- |
| `recipient_id` | Record owner or recipient |
| `vendor_name` | Vendor name |
| `ref_type` | Source entity type |
| `ref_id` | Source document id |
| `reference_from` | Source reference text |
| `date` | Receipt date |
| `memo` | Notes |
| `transport` / `transport_amount` | Freight information |
| `truck_no` / `driver_name` | Logistics details |
| `location_name` | Location |
| `source_location` | Source location |
| `currency_name` / `exchange_rate` | Currency handling |
| `department_name` / `class_name` / `project_name` | Segmentation |
| `approval_status_type` | Approval state |
| `recipient_details` | Receipt line items |
| `landed_cost_details` | Landed cost details |

## Example

A purchase order can move into item receipt.
That receipt can then feed the vendor bill and inventory reports.

## Practical note

The shared tools are not a separate business module.
They are the supporting layer that makes the main workflows easier to trace and print.
