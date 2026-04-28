# POS

The POS module supports point-of-sale operations for retail or counter-based selling.

## Main routes in the app

| Route | Purpose |
| --- | --- |
| `setup` | Configure POS |
| `system` | Open the POS system |
| `system-2` | Alternate POS system view |
| `grid-system` | Grid-based POS screen |
| `grid-system-2` | Alternate grid POS screen |
| `payment` | POS payment screen |
| `counter/new` | Create a counter |
| `counter/list` | View counters |
| `session/start` | Start a POS session |
| `session/list` | View sessions |
| `shift/new` | Start a shift |
| `shift/list` | View shifts |
| `table/new` | Create a table |
| `order-type/new` | Create an order type |
| `modifier-group/new` | Create a modifier group |
| `modifier/new` | Create a modifier |
| `loyalty-point` | Configure loyalty points |
| `loyalty-reward` | Manage rewards |

## What POS supports

- counter-based selling
- held orders
- payment collection
- invoice generation
- session and shift control
- table and order type management
- modifiers and loyalty rules

## Example

A cashier opens the counter, searches for items, takes payment, and prints the POS invoice in one flow.

## What to document in detail

The POS pages should explain:

- setup before sales start
- how to start a session
- how to move between holds and active sales
- how payment finalization works
- how cash settlement closes the counter

## Practical note

The POS code includes session guards and multiple screen variants.
That means users should start with setup and session rules before learning the sale screen itself.
