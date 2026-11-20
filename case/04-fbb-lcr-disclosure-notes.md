# How to read FBB's LCR disclosure

`04-fbb-lcr-disclosure.csv` holds FBB's liquidity coverage ratio (LCR) disclosure for four quarter-ends: 31 December 2025, 31 March 2026, 30 June 2026 and 30 September 2026. The figures are fictional.

## Layout

The rows follow the EU LIQ1 template that banks use in their Pillar 3 reports, in a simplified form:

- Amounts are in **EUR million**.
- Each quarter shows an **unweighted** value (the outstanding balance) and a **weighted** value (after the run-off or inflow rates of the LCR rules are applied).
- Real EU LIQ1 disclosures show averages over the last twelve month-end observations. To keep the exercise simple, this file shows one value per quarter.
- Rows 1 and 21–23 only have a weighted (or adjusted) value. Rows 9 and 16 only have a weighted value in this file.

## The calculation

```
LCR = liquidity buffer (row 21) / total net cash outflows (row 22)

total net cash outflows = total cash outflows (row 16)
                          - min(total cash inflows (row 20), 75% of total cash outflows)
```

- The minimum requirement is 100%.
- Inflows count for at most 75% of outflows (the inflow cap). Check whether the cap binds before you subtract.
- "Of which" rows add up to their parent row: row 2 = rows 3 + 4, row 5 = rows 6 + 7 + 8, row 10 = rows 11 + 12 + 13.
- Row 16 = rows 2 + 5 + 9 + 10 + 14 + 15 (weighted). Row 20 = rows 17 + 18 + 19.
