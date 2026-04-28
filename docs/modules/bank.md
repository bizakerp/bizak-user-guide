# Bank

The Bank module supports banking transactions and cash movement.

## Main routes in the app

| Route | Purpose |
| --- | --- |
| `check` | Write a check |
| `make-deposit` | Record a deposit |
| `transfer-fund` | Move money between accounts |

## Deposit records

The deposit DTO includes:

| Field | Meaning |
| --- | --- |
| `account_id` | Deposit account |
| `amount` | Deposit amount |
| `date` | Deposit date |
| `memo` | Notes |
| `currency_id` / `exchange_rate` | Currency handling |
| `department_id` / `location_id` / `class_id` / `project_id` | Segmentation |
| `payment_method_name` | Payment method name |
| `bank_name` / `cheque_no` / `cheque_date` | Bank details |
| `other_deposits` | Additional deposit lines |

## Transfer fund

The transfer-fund filter shows that the module can search by:

| Filter | Meaning |
| --- | --- |
| `search` | Document, memo, or account text |
| `from_account_names` | Source accounts |
| `to_account_names` | Destination accounts |
| `approval_statuses` | Approval states |

## Detailed pages

- [Check](bank/check.md)
- [Make Deposit](bank/make-deposit.md)
- [Transfer Fund](bank/transfer-fund.md)

## Example

A user can transfer money from one bank account to another and then reconcile the movement later in accounting reports.

## Practical note

Bank actions usually end up in account reports.
That makes the bank module part of the accounting story, not a separate island.
