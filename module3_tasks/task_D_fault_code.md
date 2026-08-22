# Task D — fault code to interpret

Slide 18 prompt: *"Our pump VFD shows fault F0011. Explain likely causes in
plain language for a night-shift operator, the checks to run in order, and
when to escalate. If unsure, say so — don't guess a code."*

Slide 18's own caution still applies and should be repeated live: **"codes
are vendor-specific — verify F0011 against the real manual before acting."**
VFD fault-code numbering isn't standardised across manufacturers, so this
folder doesn't claim F0011 is a real code from any actual vendor's manual —
that would be exactly the kind of fabricated-citation risk the course
guardrails rule out. Paste the fictional, composite site reference below
instead, framed the same way as every other knowledge document in this
course (a made-up document for our fictional plant, not a real external
standard).

## Paste this as the "VFD fault-code reference"

> **Site VFD Fault-Code Quick-Reference (fictional, composite — not tied to
> any specific manufacturer's manual), Dosing Pump P-330**
>
> P-330 meters biocide/scale-inhibitor into the cooling tower basin per the
> site water treatment chemical program (SOP-WTR-022 §4).
>
> | Code | Description | Typical cause |
> | --- | --- | --- |
> | F0011 | Motor overcurrent trip | Dosing line blockage/crystallised scale inhibitor increasing back-pressure; worn pump head |
> | F0014 | Drive overtemperature | VFD cabinet cooling fan fault or blocked ventilation |
> | F0021 | Undervoltage trip | Site supply dip or loose incoming power connection |
> | F0033 | Communication fault | Loss of signal between VFD and DCS |

## Model answer for F0011

- **Likely causes, most to least common for a dosing pump:** a blocked or
  partially crystallised dosing line (scale inhibitor can crystallise if a
  line runs near-empty or dries out); a worn pump head drawing excess
  current; less likely, a genuinely seized motor bearing.
- **Checks, in order:** (1) check the dosing tank level and line for visible
  blockage/crystallisation; (2) check whether dosing has been running
  continuously or cycling erratically — erratic cycling points to a line
  fault rather than a motor fault; (3) if the line is clear, consider a
  mechanical pump-head fault.
- **What NOT to do:** don't reset and restart repeatedly without checking
  the line — restarting into a blocked line risks further motor damage, and
  a missed dosing cycle affects water treatment, not just the pump.
- **Escalate when:** any decision to keep dosing running, bypass dosing
  temporarily, or take the pump out of service needs utilities-engineer
  sign-off — biocide/scale-inhibitor dosing changes are explicitly called
  out in SOP-WTR-022 §4/§5 as requiring approval, not something an
  assistant decides.
- **The "if unsure, say so" test:** a well-guarded answer explicitly flags
  that F0011 is being interpreted from the *site's own* fictional
  quick-reference, not a real vendor manual, and tells the operator to
  confirm against the actual VFD nameplate/manual before acting.
