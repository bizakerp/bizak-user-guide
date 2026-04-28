# POS

The POS module supports point-of-sale operations for retail or counter-based selling.

## Visual guide

![POS counter setup illustration](../assets/images/workflows/pos/counter-bg.png)

!!! note "Start with setup"
    POS is centered on a counter and a live session.
    Set the defaults first.
    Then open a session before you sell.

## Before you start

- Confirm the POS setup exists.
- Confirm the counter or grid screen is configured.
- Confirm the default customer and payment method are ready.
- Confirm the user can open sessions and shifts.

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

## Related pages

- [POS Setup](pos/setup.md)
- [POS System](pos/system.md)
- [Session](pos/session.md)
- [Shift](pos/shift.md)
- [Payment Screen](pos/payment.md)
- [Order Type](pos/order-type.md)
- [Counter](pos/counter.md)

## Detailed pages

- [POS Setup](pos/setup.md)
- [POS System](pos/system.md)
- [POS System 2](pos/system-2.md)
- [Grid POS](pos/grid-system.md)
- [Grid POS 2](pos/grid-system-2.md)
- [Payment Screen](pos/payment.md)
- [Counter](pos/counter.md)
- [Session](pos/session.md)
- [Shift](pos/shift.md)
- [Table](pos/table.md)
- [Order Type](pos/order-type.md)
- [KOT List](pos/kot.md)
- [Modifier Groups and Modifiers](pos/modifier.md)
- [Loyalty Point Setup](pos/loyalty-point.md)
- [Loyalty Reward](pos/loyalty-reward.md)

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
