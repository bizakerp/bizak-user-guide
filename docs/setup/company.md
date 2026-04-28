# Company Setup

Company setup defines the structural information Bizak uses across the application.

## Common company items

- company name
- class
- currency
- exchange rates
- department
- location
- auto-numbering
- company information
- job title definitions

## What the code shows

The codebase includes company, class, currency, exchange rate, department, location, and auto-numbering DTOs.
That means these are real configuration objects used across transactions and reports.

## Example

If a business operates across multiple departments and locations, those values should be set up early so they can flow into transactions, reports, and approval logic.

## Tip

Set the company structure before users start entering transactions.
That prevents missing dropdown data later.
