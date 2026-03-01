# /reconciliation

Reconcile GL account balances to subledger, bank, or third-party balances. Identify and categorize reconciling items and generate a reconciliation workpaper.

> **Important**: This command assists with reconciliation workflows but does not provide financial advice. All reconciliations should be reviewed by qualified financial professionals before sign-off.

## Usage

```
/reconciliation [account] [period]
```

### Arguments
- `account` — Account to reconcile: `cash`/`bank`, `ar`/`accounts-receivable`, `ap`/`accounts-payable`, `fixed-assets`/`fa`, `intercompany`/`ic`, `prepaid`, `accrued-liabilities`, or any GL account code
- `period` — Period end date (e.g., `2024-12`, `2024-12-31`)

## Workflow

### 1. Gather Both Sides

If ~~erp or ~~data warehouse is connected:
- Pull GL balance for the specified account(s) as of period end
- Pull subledger, bank statement, or third-party balance for comparison
- Pull prior period reconciliation for outstanding item carryforward

If no data source: prompt user for GL balance, other-side balance, and prior period outstanding items.

### 2. Compare Balances

```
GL Balance:                        $XX,XXX.XX
Subledger/Bank/Other Balance:      $XX,XXX.XX
                                   ----------
Difference:                        $XX,XXX.XX
```

### 3. Identify Reconciling Items

**Timing Differences** (will clear in subsequent periods): Outstanding checks, deposits in transit, pending invoices, accruals awaiting reversal

**Permanent Differences** (require adjustment): Recording errors, missing entries, bank fees not recorded, FX translation differences

**Prior Period Items**: Items cleared vs. still outstanding (carry forward with aging)

### 4. Generate Reconciliation Workpaper

```
ACCOUNT RECONCILIATION
Account: [Code] — [Name]
Period End: [Date]
Prepared by: [User]    Date Prepared: [Today]

Balance per General Ledger:              $XX,XXX.XX
  Add: [Reconciling items]                $X,XXX.XX
  Less: [Reconciling items]             ($X,XXX.XX)
Adjusted GL Balance:                     $XX,XXX.XX

Balance per [Subledger/Bank/Other]:      $XX,XXX.XX
  Add: [Reconciling items]                $X,XXX.XX
  Less: [Reconciling items]             ($X,XXX.XX)
Adjusted [Other] Balance:                $XX,XXX.XX

DIFFERENCE:                                   $0.00
```

### 5. Reconciling Items Detail

| # | Description | Amount | Category | Age (Days) | Status | Action Required |
|---|-------------|--------|----------|------------|--------|-----------------|
| 1 | [Detail]    | $X,XXX | Timing   | 5          | Expected to clear | Monitor |
| 2 | [Detail]    | $X,XXX | Error    | N/A        | Requires correction | Post adjusting JE |

### 6. Review and Escalation

Flag items requiring attention:
- Aged items outstanding more than 30/60/90 days
- Large items exceeding materiality thresholds
- Growing reconciling item totals period over period
- Unresolved prior period items
- Unexplained differences

### 7. Output

1. Formatted reconciliation workpaper
2. Reconciling items with categorization and aging
3. Required adjusting entries (if permanent differences identified)
4. Action items for follow-up
5. Comparison to prior period reconciliation (if available)
6. Sign-off section for preparer and reviewer
