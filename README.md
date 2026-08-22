# SME Bank Models

Bottom-up unit-economics workbooks for a synthetic UK SME bank, provided for
reference use. **Every figure is synthetic or from cited public sources; nothing here
describes any real institution's internal data.**

**Current workbook version: v1.5 (22 August 2026).** Every download self-identifies —
the Guide tab's first line shows its version, with a change history beneath it. If your copy shows an older version, re-download — or fetch that exact version from the
**Releases** page, where every published version remains permanently downloadable.
Adapted copies should note which version they started from on their change-log tab.

| File | What it is |
|---|---|
| `UK_SME_Bank_Bottom_Up_Unit_Economics.xlsx` | The reference model: 13 tabs, from customer bounding through per-product economic profit, plus a flow register, a demand layer and a process register. |
| `meridian_model.xls` | A second worked example at a smaller scale ("Meridian", fictional), built from the same method. |
| `meridian_fact_pack.md` | The synthetic input data behind the Meridian model, including how missing inputs were flagged and banded. |

## Two optional layers (v1.4 and v1.5)

Both ship **OFF**. With both off the workbook behaves exactly as v1.3 did, to the last
decimal — that property is asserted by a gate on every build, not assumed.

**`1b. Demand & CEPs` — the demand layer (v1.4).** The nine product penetrations and the
customer count are normally asserted. This layer derives them from category entry
points — the situations in which a customer's job arises:

    penetration = (lambda*c x L) / (1 + lambda*c x L)
    lambda*c    = events x presence x conversion

That is Little's Law run forwards, so it needs no time axis and the model stays a
steady-state snapshot. Set the mode on Inputs section L. `CALIBRATE` is worth running
first: it changes nothing and reports the event rate implied by the assumptions already
in the workbook — one won loan moment per 29.3 customer-years, asset finance 40.2,
invoice finance 129.3. Those are claims you can argue with; a 12% penetration is not.

**`3. HR & Activity` columns M–T and `3b. Process Index` — the process layer (v1.5).**
Step 2 of the method is running costs, so the process register lives on the Step 2 tabs
rather than on a sheet of its own. Every activity gains a yield, a best-in-class
intensity and yield, a benchmark source and a £ gap. Below the activity table sits a
register of 22 head-office processes that the flow register already named but nothing
ever costed.

Yield inflates **attempts** and never deflates outcomes — that is what stops it
double-counting with the demand layer's conversion. Head-office costs are carved *out*
of the existing pools, so naming a process moves money from unallocated to attributed
and the total never changes.

`3b` indexes every process to the numbers it moves and imputes what each would have to
become to reach a target cost:income.

**Both layers ship empty on purpose.** Every cell that needs an institution's own data is
blank and carries the query that would fill it. Invented rates get contradicted by real
cohort data, which discredits the parts of a model that are right.

## How to use with an AI assistant

1. **Download the workbook** (binary — do not copy code or cells via the clipboard)
   and open it in Excel. All formulas are live and recalculate on open.
2. Ask your assistant to **replace the values on the Inputs tab with your own
   numbers, one section at a time** — every input is a single labelled cell with a
   source note.
3. **The built-in checks:** the bridge-check cell on the Unit Economics tab must stay
   at ~0 after every change. If it moves, structure was broken — undo and retry. With
   the layers on, `1b` carries its own self-check block.
4. Record every edit on a **change-log tab** you add — the workbook is the model, so
   its audit trail matters.
5. Structural changes (adding or removing products or cost lines) go beyond input
   replacement — follow the row and column patterns already present, and verify the
   bridge check still holds.

## Notice

© TMTH Studio 2026. Provided for reference and evaluation. No licence is granted for
redistribution or commercial reuse of the models or the methodology they embody.
