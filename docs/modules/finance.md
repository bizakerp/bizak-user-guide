# Finance

The Finance module covers accounting entries and financial controls.

## Before you start

- Confirm ledgers and ledger groups are ready.
- Confirm fiscal year and posting periods are set.
- Confirm users can post or review finance records.
- Confirm company setup for currency, department, and location is complete.

## Main routes in the app

| Route | Purpose |
| --- | --- |
| `journal` | Create journal entries |
| `opening` | Set opening balances |
| `expenses/report` | Enter expense reports |
| `budget` | Manage budgets |
| `bank-reconcile` | Reconcile bank activity |

## Related pages

- [Account Setup](../setup/account-setup.md)
- [Journal Entry](finance/journal.md)
- [Opening Balance](finance/opening-balance.md)
- [Expense Report](finance/expense-report.md)
- [Budget](finance/budget.md)
- [Bank Reconcile](finance/bank-reconcile.md)
- [Account Reports](../reports/account-reports.md)

## Journal entry

The journal entry DTO includes:

| Field | Meaning |
| --- | --- |
| `journal_no` | Journal number |
| `date` | Entry date |
| `memo` | Journal memo |
| `party_id` | Related party if used |
| `currency_id` / `exchange_rate` | Currency handling |
| `class_id` / `location_id` / `department_id` / `project_id` / `subsidiary_id` | Segmentation fields |
| `cheque_no` / `cheque_date` | Cheque details |
| `bill_no` / `bill_date` / `due_date` | Bill references |
| `is_defer_entry` | Deferred entry flag |
| `reversal_date` | Reversal date |
| `journal_entry_details` | Debit and credit lines |

The code also checks that debit and credit totals match before the entry is valid.

## Detailed pages

- [Journal Entry](finance/journal.md)
- [Opening Balance](finance/opening-balance.md)
- [Expense Report](finance/expense-report.md)
- [Budget](finance/budget.md)
- [Bank Reconcile](finance/bank-reconcile.md)

## Opening balance

The opening balance DTO is simple:

| Field | Meaning |
| --- | --- |
| `LedgerId` | Ledger id |
| `LedgerName` | Ledger name |
| `FiscalYearId` | Fiscal year |
| `BookClosedId` | Book close reference |
| `DrAmount` | Debit balance |
| `CrAmount` | Credit balance |

## Budget

The budget setup DTO includes:

| Field | Meaning |
| --- | --- |
| `fiscal_year_id` | Fiscal year |
| `posting_period_id` | Budget period |
| `ledger_id` | Ledger |
| `class_id` / `department_id` / `location_id` / `project_id` | Segmentation |
| `vendor_id` / `item_id` | Additional budget dimensions |
| `amount` | Budget amount |

## Expense report

The expense report DTO includes:

| Field | Meaning |
| --- | --- |
| `document_no` | Document number |
| `date` | Expense date |
| `purpose` | Purpose text |
| `employee_id` | Employee who submitted it |
| `account_name` | Expense account |
| `ledger_id` | Linked ledger |
| `location_name` | Location |
| `project_name` | Project |
| `class_id` / `department_id` | Segmentation |
| `advance_to_apply` | Advance amount to apply |
| `advance_allocations` | Advance allocation details |
| `tax_details` | Tax detail lines |

## Example

If salary expense is recorded manually, the finance team may post a journal entry that debits salary expense and credits the bank or payable account.

## Practical note

Finance pages often feed directly into the account reports section.
That is why the setup data matters so much.
