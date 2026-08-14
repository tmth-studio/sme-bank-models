# SME Bank Models

Bottom-up unit-economics workbooks for a synthetic UK SME bank, provided for
reference use. **Every figure is synthetic or from cited public sources; nothing here
describes any real institution's internal data.**

**Current workbook version: v1.2 (12 August 2026).** Every download self-identifies —
the Guide tab's first line shows its version, with a change history beneath it. If your copy shows an older version, re-download — or fetch that exact version from the
**Releases** page, where every published version remains permanently downloadable.
Adapted copies should note which version they started from on their change-log tab.

| File | What it is |
|---|---|
| `UK_SME_Bank_Bottom_Up_Unit_Economics.xlsx` | The reference model: 9 tabs, ~600 live formulas, from customer bounding through per-product economic profit, plus a flow register. |
| `meridian_model.xls` | A second worked example at a smaller scale ("Meridian", fictional), built from the same method. |
| `meridian_fact_pack.md` | The synthetic input data behind the Meridian model, including how missing inputs were flagged and banded. |

## How to use with an AI assistant

1. **Download the workbook** (binary — do not copy code or cells via the clipboard)
   and open it in Excel. All formulas are live and recalculate on open.
2. Ask your assistant to **replace the values on the Inputs tab with your own
   numbers, one section at a time** — every input is a single labelled cell with a
   source note.
3. **The built-in check:** the bridge-check cell on the Unit Economics tab must stay
   at ~0 after every change. If it moves, structure was broken — undo and retry.
4. Record every edit on a **change-log tab** you add — the workbook is the model, so
   its audit trail matters.
5. Structural changes (adding or removing products or cost lines) go beyond input
   replacement — follow the row and column patterns already present, and verify the
   bridge check still holds.

## Notice

© TMTH Studio 2026. Provided for reference and evaluation. No licence is granted for
redistribution or commercial reuse of the models or the methodology they embody.
