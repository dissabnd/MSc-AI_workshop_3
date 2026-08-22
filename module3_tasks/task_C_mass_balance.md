# Task C — water balance to critique

Slide 17 prompt: *"Here is a colleague's mass balance (pasted). Check it
step by step. Does it close? Are the units consistent? State any errors and
the corrected figures."* (Here it's a cooling-tower water balance instead
of a distillation mass balance — same idea, simpler numbers, no
density/composition conversion needed since it's dilute aqueous
throughout.)

## Paste this as "a colleague's cooling tower water balance"

> **Cooling tower water balance — cooling water loop to C-201, shift
> engineer draft, for review (SOP-WTR-022 §2)**
>
> Make-up water flow: 45 m³/h
> Blowdown flow: 9 m³/h
> Evaporation (by difference): 45 − 9 = **36 m³/h**
>
> Make-up water conductivity: 300 µS/cm
> Blowdown conductivity: 1,500 µS/cm
>
> "Cycles of concentration" (COC) tells us how many times the dissolved
> solids have been concentrated by evaporation before being purged in the
> blowdown. Calculated from flows:
>
> COC = Make-up flow ÷ Evaporation flow = 45 ÷ 36 = **1.25 cycles**
>
> "1.25 cycles is close to design — no action needed."

## What's actually wrong (a standard relationship, verified independently)

The flow numbers themselves are fine (45 = 9 + 36 closes). The error is in
which flow the colleague divided by. The standard cooling-tower water
balance (steady state, evaporation carries no dissolved solids — a normal,
stated simplification that ignores windage/drift loss) gives:

**Make-up = Evaporation + Blowdown**, and because everything the make-up
water brings in ends up concentrated into the blowdown:

**Make-up × C(make-up) = Blowdown × C(blowdown)**

which rearranges to **COC = Make-up ÷ Blowdown** — not make-up ÷
evaporation. Using the colleague's own flow numbers correctly:

COC (from flows) = 45 ÷ 9 = **5.0 cycles**

That should be cross-checked against the conductivity data already on the
page, since COC also equals the conductivity ratio directly:

COC (from conductivity) = 1,500 ÷ 300 = **5.0 cycles**

Both correct methods agree at **5.0**, not 1.25. The colleague divided by
the wrong flow (evaporation instead of blowdown) and the answer came out
4× too low — and the same page already had the conductivity data needed to
catch the contradiction (1.25 vs. 5.0), it just wasn't cross-checked.

**Why it matters, not just arithmetically:** COC = 1.25 vs. COC = 5.0 is
the difference between "using much more make-up water than the design
dosing plan assumes" and "operating normally" — SOP-WTR-022 §2 flags
conductivity/COC outside the dosing plan band as something to check before
adjusting anything, and a wrong COC changes what "outside the band" even
means for this shift.

**Check it:** did the model catch that COC should use blowdown, not
evaporation, in the denominator — and did it think to cross-check the flow-
based number against the conductivity-based number already given?
