# Task A — P&ID snippet to paste

Slide 15 prompt: *"You are a process engineer. Here is a P&ID description
(pasted). List the control loop: what is measured, the controller, the final
control element, and what it regulates. Note any interlocks."*

## Paste this as the "P&ID description"

> **Cooling water flow control to condenser C-201 (P&ID excerpt, text
> description)**
>
> - FT-301 measures cooling water flow to condenser C-201.
> - FT-301's signal goes to flow controller FIC-301.
> - FIC-301's output positions FCV-301, the cooling water control valve.
> - FCV-301 fails **open** on loss of signal or instrument air (starving the
>   condenser of cooling water is the worse failure, so the valve is
>   designed to open, not close, if control is lost).
> - If flow falls below 90% of design duty, the DCS raises a low-flow alarm
>   (SOP-WTR-022 §2); operators check the strainer and pump before taking
>   any other action.

## What a correct answer says

- **Measured variable:** cooling water flow to C-201 (FT-301).
- **Controller:** FIC-301.
- **Final control element:** FCV-301 (cooling water control valve),
  fail-**open**.
- **What it regulates:** cooling water flow to condenser C-201, holding it
  at design duty.
- **Alarm (not a hard trip here):** low-flow alarm below 90% of design
  (SOP-WTR-022 §2) — action is to check strainer/pump first, not adjust the
  column.

**Live "check it" moment (30 s):** did the model get the fail-safe direction
right? A cooling-water valve failing **open** (not closed) is the opposite
of the steam valve pattern students may expect from other examples — a good
answer explains *why* (loss of cooling water is worse than a temporary
excess), not just states it.
