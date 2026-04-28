# Session

This page covers POS session start and session list flows.
Use it before selling begins.

## What the screen does

- It opens a session for a counter and shift.
- It collects opening cash.
- It can use either direct cash entry or a breakdown view.
- It checks whether a session is already active.
- It sends the user to the POS system after a successful start.

## What it tracks

| Field | Meaning |
| --- | --- |
| `counter_id` | Counter |
| `shift_id` | Shift |
| `opening_cash` | Opening cash |
| `remarks` | Remarks |
| `opening_denominations` | Cash breakdown when used |

## Example

The cashier opens a new session at the start of the day.
The system records the counter, shift, and opening cash before sales begin.

