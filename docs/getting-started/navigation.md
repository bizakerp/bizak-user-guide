# Navigation Overview

Bizak is organized around major business modules.

## Main areas

- Dashboard
- Sales
- Procurement
- Inventory
- Finance
- Payment
- Bank
- POS
- CRM
- Field Operations
- Reports
- Setup and Administration

## How users should think about navigation

- **Master data** is where you define the business objects.
- **Transactions** are where you record activity.
- **Reports** show the result of that activity.
- **Setup** controls company behavior, defaults, and permissions.

## Main routes in the current app

| Area | Example path |
| --- | --- |
| Dashboard | `/app/main/dashboard` |
| Sales | `/app/main/sales/*` |
| Procurement | `/app/main/procurement/*` |
| Inventory | `/app/main/inventory/*` |
| Finance | `/app/main/finance/*` |
| Payment | `/app/main/payment/*` |
| Bank | `/app/main/bank/*` |
| POS | `/app/main/pos/*` |
| Reports | `/app/main/report/*` |
| CRM | `/app/main/crm/*` |
| Field operations | `/app/main/sfm/*` |

## Recommended user pattern

1. Start from the dashboard
2. Identify the module you need
3. Open the relevant create, list, or update screen
4. Save the transaction
5. Confirm the report or posting result

## Reading the screen

List screens show existing records.
Create and update screens collect data.
Detail screens show what was saved and what related records were created.
