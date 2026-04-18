# Auto-generate Excel SUMIF Macro (English)

## Use case
Aggregate store-by-store monthly sales automatically.
Manual work 40 min → Generated macro 5 sec.

## Prompt to paste into Claude Code

```
Please write an Excel VBA macro.

[Input data]
Sheet name: Sales
- Column A: Date (YYYY/MM/DD)
- Column B: Store name
- Column C: Sales amount (number)

[What I want]
- Pivot-style table with stores as rows and months as columns
- Output starts at column E
- Use SUMIFS
- Add a totals row and totals column

[Constraints]
- Write in VBA, 5 lines or fewer if possible
- Minimal error handling
```

## Expected output

```vba
Sub AggregateSalesByStoreMonth()
    Dim lastRow As Long: lastRow = Cells(Rows.Count, "A").End(xlUp).Row
    ' Claude Code returns the full working VBA including SUMIFS formulas
    ' and auto-totals. Paste into the VBA editor (Alt+F11) and run.
End Sub
```

## If it doesn't work

Paste the error message directly to Claude Code:
> "I got this error: 'Runtime Error 1004'. Where should I fix it?"

A fixed version will be returned.

## Variations

- Want weekly aggregation? Change "months as columns" → "weeks as columns"
- Want product breakdown? Add "Column D: Product" and mention it
- Want Google Sheets instead? Prepend "Please write in Google Apps Script"

## Related

- [meeting-notes-structure.md](meeting-notes-structure.md) — Structure meeting notes
- [expense-csv-classify.md](expense-csv-classify.md) — Classify expenses
