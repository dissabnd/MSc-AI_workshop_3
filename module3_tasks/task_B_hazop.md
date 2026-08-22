# Task B — HAZOP row to draft

Slide 16 prompt: *"Using the guideword HIGH FLOW on the feed line, draft a
HAZOP entry: deviation, cause, consequence, existing safeguard, recommended
action. Cite the SOP where relevant. Flag anything needing human review."*
(Swap "the feed line" for "the cooling water line to C-201" for this
version.)

## Context to paste first (same for every guideword)

> Cooling water loop to condenser C-201: supply normal 22–28 °C, alarm
> above 32 °C; return normal ≤38 °C, alarm above 42 °C; flow per design
> duty, alarm below 90% of design (SOP-WTR-022 §2).

## Model answer — guideword LOW FLOW on the cooling water line

| Field | Content |
| --- | --- |
| Deviation | Low flow of cooling water to condenser C-201 |
| Cause | FCV-301 sticks/fails partly shut; strainer blockage; cooling water pump underperforming |
| Consequence | Condenser duty falls; return temperature rises toward 42 °C alarm; column top pressure (PT-201) can trend upward (SOP-WTR-022 §2 cross-reference to SOP-D201-014 §6) |
| Existing safeguard | Low-flow alarm below 90% of design duty (SOP-WTR-022 §2); FCV-301 fails open, so a control failure itself doesn't cause low flow |
| Recommended action | Check strainer and pump performance first, per SOP-WTR-022 §2, before touching column operation |
| Human review needed? | **Yes** for anything beyond checking strainer/pump — dosing rates, blowdown rates, or cooling tower fan/pump duty must not be changed without utilities-engineer sign-off (SOP-WTR-022 §5) |

**Check it:** did the model correctly route the fix to *checking the cooling
water side first* rather than jumping straight to adjusting the column — and
did it flag that dosing/duty changes need sign-off?

## Backup guidewords (give one per pair for variety)

**HIGH TEMPERATURE on the cooling water supply**
- Cause: cooling tower underperforming (fouling, fan fault, high ambient
  wet-bulb); make-up water too warm.
- Consequence: supply temperature approaches the 32 °C alarm; less
  condensing duty available at C-201.
- Safeguard: supply-temperature alarm at 32 °C (SOP-WTR-022 §2).
- Action: check cooling tower fan operation and basin level before any
  column-side adjustment.
- Human review: cooling tower fan/pump duty changes need utilities-engineer
  sign-off (SOP-WTR-022 §5).

**OUT OF BAND on W-301 feed water hardness**
- Cause: softener resin exhausted/needs regeneration; softener bypass valve
  left open in error.
- Consequence: feed water hardness rises above the 2 ppm (as CaCO₃) alarm,
  risking boiler tube scaling downstream (SOP-WTR-022 §3).
- Safeguard: hardness alarm at 2 ppm; routine shift sampling (SOP-WTR-022
  §4).
- Action: re-check the reading before acting (a single out-of-band reading
  should be re-checked); if it's a sustained trend across two shifts,
  escalate.
- Human review: any water-treatment issue that could affect boiler safety
  requires engineering sign-off before corrective action (SOP-WTR-022 §5).
