# Predictive Maintenance — Capstone Group Brief

**Process area:** Predictive Maintenance
**Your job:** read the situation below, fill Appendix B, then write your OWN `agent_instructions.txt` — nothing is pre-built for you this time.

## The situation (read this before you open the worksheet)

Feed pump P-450's bearing vibration has crept from 3 to 6 mm/s over the last three days — trending toward the 7.1 mm/s alarm, but not there yet. Suction pressure has also dipped to 0.7 bar while vibration keeps rising. Nothing has tripped. Is this a maintenance item that can wait for the next planned window, or something that needs escalating before the next shift starts?

## Your knowledge document(s)

- `knowledge/Column_Setpoints_Datasheet.pdf` (DS-D201-02)
- `knowledge/P-450_pump_maintenance_SOP.pdf`

Attach these in the **chat window**, first message of every new chat with your agent — not in Agent Builder's Knowledge/Configure tab (it doesn't work on this licence tier).

## What you do next

1. Read the situation above and skim your knowledge document — you don't need to memorise it, just know roughly what's in there.
2. Fill **Appendix B — Capstone worksheet** (in `WS3_outline.docx`) for your area. The **"one task it COMPLETES"** row is the one that's graded hardest — answering a question does not count; your agent has to *produce something* (a HAZOP row, a corrective-action plan, a shift-handover note, a routing decision, a go/no-go check).
3. Open `agent_instructions_TEMPLATE.txt` and write your own instructions from your worksheet answers — persona, how it answers, guardrails, tone, starter prompts. This is the actual design work being assessed; there's no answer to copy.
4. Build the agent in Copilot Agent Builder: paste in what you wrote, add your starter prompts, save — then attach your knowledge document(s) in the chat panel as described above.
5. Test it against the situation above, **and** against at least one request it must refuse or escalate rather than answer.
6. Prepare your 2-minute pitch: show it completing its one task on a grounded input, and show it correctly refusing the unsafe one.

## The question you're answering

*Can AI help run this part of the plant — and where must a human stay in the loop?*
