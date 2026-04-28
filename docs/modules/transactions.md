# Transactions

Transactions are the operational records that Bizak uses to move business activity into accounting and reporting.

This section gives a cross-module view so users understand how the major workflows connect.

## Transaction families

| Family | Examples | Output |
| --- | --- | --- |
| Sales | Estimate, order, invoice, credit memo, return | Revenue, receivables, stock changes |
| Procurement | Purchase order, receipt, bill, vendor credit | Payables, stock intake, supplier balances |
| Payment | Customer receipt, vendor payment | Cash or bank movement, outstanding settlement |
| Finance | Journal entry, budget, expense report, opening balance | Direct accounting impact |
| Inventory | Transfer order, fulfill reference, adjustment | Stock movement and valuation |

## Sales workflow example

1. Create an opportunity or estimate
2. Confirm the sales order or invoice
3. Fulfill the goods or service
4. Receive payment
5. Review customer ledger and sales reports

### Example

A customer orders 10 printers. Bizak can track the estimate, sales order, invoice, payment, and final receivable position in separate but connected steps.

## Procurement workflow example

1. Create a purchase order
2. Receive goods
3. Enter the vendor bill
4. Apply credits if needed
5. Review the vendor ledger and procurement reports

### Example

A supplier delivers 100 cartons of stock. The purchase order, goods receipt, and vendor bill should all align so accounting and inventory remain consistent.

## Payment workflow example

### Customer receipt

| Field | Meaning |
| --- | --- |
| Customer | The buyer making the payment |
| Receipt date | When payment was received |
| Payment mode | Cash, bank, cheque, transfer, or similar |
| Deposit account | Where the money is going |
| Amount received | Value collected from the customer |
| Invoice selection | Which open invoices to settle |
| Unallocated amount | Amount left as advance or credit |

### Vendor payment

| Field | Meaning |
| --- | --- |
| Vendor | The supplier being paid |
| Payment date | When the payment is recorded |
| Payment mode | Cash, bank, cheque, transfer, or similar |
| Account | Source account for the payment |
| Amount paid | Total value sent to the vendor |

## Finance workflow example

| Entry | Debit | Credit |
| --- | --- | --- |
| Salary expense | 50,000 |  |
| Bank |  | 50,000 |

This type of journal entry is used when the user needs to post directly to the general ledger without going through a sales or procurement form.

## Inventory workflow example

If a physical count shows that stock is short, the user records an inventory adjustment:

1. choose the adjustment date
2. select the item
3. review current quantity
4. enter the adjusted quantity
5. save the correction

That adjustment then updates stock reporting and valuation.

