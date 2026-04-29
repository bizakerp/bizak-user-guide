# Shift

This page covers POS shift setup.
Use it to define working hours for a POS counter.

## What the screen tracks

| Field | Meaning |
| --- | --- |
| `shift_name` | Shift name |
| `counter_id` | Counter |
| `department_id` | Department |
| `start_time` | Start time |
| `end_time` | End time |
| `is_active` | Active flag |
| `description` | Description |
| `display_order` | Sort order |

The route supports create, list, and update flows.

## What to notice on the shift screen

- Shift times define when a counter should be active.
- The counter link keeps the shift tied to the right station.
- The active flag helps managers control use.

## Example

A store defines a morning shift and an evening shift.
The POS session can then open under the right shift.
