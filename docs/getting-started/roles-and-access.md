# Roles and Access

Bizak uses role-based access control so users only see the forms and actions they are allowed to use.

## What roles control

- menu visibility
- form access
- create, edit, and delete permissions
- posting or approval actions
- organization-specific access

## What the code shows

The authentication and permission DTOs show the system is designed around:

- user accounts
- security questions and reset flows
- permission setup
- role permission maps
- tenant and organization filtering

## Example

An accountant may be allowed to:

- view ledger and journal reports
- enter journal entries
- process bank actions

A sales user may instead be allowed to:

- create estimates
- issue invoices
- record customer receipts

## Role design example

A finance role can see journals, opening balances, bank reconciliation, and account reports.
A sales role can see opportunities, estimates, orders, invoices, and customer ledgers.
A warehouse role can see item receipt, transfer order, adjustment, and stock reports.

## Why this matters

Correct role design keeps data safe and reduces user confusion. The guide will later explain the most common role patterns by department.
