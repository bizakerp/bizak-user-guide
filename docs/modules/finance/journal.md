# Journal Entry

This page covers the journal entry flow.
Use it when you need to post a manual accounting entry.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `journal_no` | Journal number |
| `date` | Entry date |
| `memo` | Entry memo |
| `party_id` | Related party |
| `currency_id` | Currency |
| `exchange_rate` | Exchange rate |
| `class_id` | Class |
| `location_id` | Location |
| `department_id` | Department |
| `project_id` | Project |
| `subsidiary_id` | Subsidiary |
| `cheque_no` | Cheque number |
| `cheque_date` | Cheque date |
| `bill_no` | Bill number |
| `bill_date` | Bill date |
| `due_date` | Due date |
| `is_defer_entry` | Deferred entry flag |
| `reversal_date` | Reversal date |
| `journal_entry_details` | Debit and credit lines |

The code validates that debit and credit totals match before the entry is valid.

## Example

The finance team posts rent expense at month end.
The journal debits rent expense and credits the bank account.
The entry keeps the books balanced.

