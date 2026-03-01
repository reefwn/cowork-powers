# /journal-entry

Prepare journal entries with proper debits, credits, supporting detail, and review documentation.

> **Important**: This command assists with journal entry workflows but does not provide financial advice. All entries should be reviewed by qualified financial professionals before posting.

## Usage

```
/journal-entry [type] [period]
```

### Arguments
- `type` — Entry type: `ap-accrual`, `fixed-assets`, `prepaid`, `payroll`, `revenue`
- `period` — Accounting period (e.g., `2024-12`, `2024-Q4`)

## Workflow

### 1. Gather Source Data

If ~~erp or ~~data warehouse is connected:
- Pull trial balance for the specified period
- Pull subledger detail for relevant accounts
- Pull prior period entries of the same type for reference

If no data source is connected:
> Prompt the user to provide trial balance data, subledger detail, or supporting schedules.

### 2. Calculate the Entry

**AP Accrual:** Goods/services received but not invoiced → Debit: Expense, Credit: Accrued liabilities
**Fixed Assets:** Depreciation schedule → Debit: Depreciation expense, Credit: Accumulated depreciation
**Prepaid:** Amortization schedule → Debit: Expense, Credit: Prepaid expense
**Payroll:** Accrued salaries, benefits, taxes, bonus → Debit: Compensation expenses, Credit: Accrued payroll/benefits
**Revenue:** Performance obligations and delivery → Debit: Deferred revenue/AR, Credit: Revenue

### 3. Generate the Journal Entry

```
Journal Entry: [Type] — [Period]
Prepared by: [User]    Date: [Period end date]

| Line | Account Code | Account Name | Debit | Credit | Department | Memo |
|------|-------------|--------------|-------|--------|------------|------|
| 1    | XXXX        | [Name]       | X,XXX |        | [Dept]     | [Detail] |
| 2    | XXXX        | [Name]       |       | X,XXX  | [Dept]     | [Detail] |
|      |             | **Total**    | X,XXX | X,XXX  |            |      |

Supporting Detail:
- [Calculation basis and assumptions]
- [Reference to supporting schedule or documentation]

Reversal: [Yes/No — if yes, specify reversal date]
```

### 4. Review Checklist

- [ ] Debits equal credits
- [ ] Correct accounting period
- [ ] Account codes are valid
- [ ] Amounts are calculated correctly with supporting detail
- [ ] Memo/description is clear and specific enough for audit
- [ ] Department/cost center coding is correct
- [ ] Consistent with prior period treatment
- [ ] Reversal flag set appropriately (accruals should auto-reverse)
- [ ] Supporting documentation referenced
- [ ] Entry is within approval authority

### 5. Output

1. Formatted journal entry
2. Supporting calculations
3. Comparison to prior period entry of the same type (if available)
4. Items flagged for review or follow-up
5. Instructions for posting
