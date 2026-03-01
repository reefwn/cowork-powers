# Reconciliation

Methodology and best practices for account reconciliation, including GL-to-subledger, bank reconciliations, and intercompany. Covers reconciling item categorization, aging analysis, and escalation.

> **Important**: All reconciliations should be reviewed by qualified financial professionals before sign-off.

## Reconciliation Types

### GL to Subledger
Compare GL control account to subledger detail (AR, AP, FA, inventory, prepaids, accrued liabilities). Common causes of differences: manual JEs not in subledger, interface timing, batch posting delays, reclassifications.

### Bank Reconciliation
```
Balance per bank statement:     $XX,XXX
  Add: Deposits in transit       $X,XXX
  Less: Outstanding checks     ($X,XXX)
Adjusted bank balance:          $XX,XXX

Balance per general ledger:     $XX,XXX
  Add: Interest/credits          $X,XXX
  Less: Bank fees              ($X,XXX)
Adjusted GL balance:            $XX,XXX

Difference:                          $0
```

### Intercompany
Reconcile receivable/payable between entities. Common causes: timing, different FX rates, misclassification, disputed amounts, different cut-off practices.

## Reconciling Item Categories

| Category | Description | Action |
|----------|-------------|--------|
| **Timing** | Outstanding checks, deposits in transit, pending interfaces | Monitor — clears within normal cycle |
| **Adjustments Required** | Unrecorded fees, errors, missing entries, classification errors | Prepare adjusting JE |
| **Requires Investigation** | Unidentified differences, disputed items, aged items, recurring unexplained | Investigate root cause, escalate |

## Aging Analysis

| Age Bucket | Status | Action |
|-----------|--------|--------|
| 0-30 days | Current | Monitor |
| 31-60 days | Aging | Investigate |
| 61-90 days | Overdue | Escalate to supervisor |
| 90+ days | Stale | Escalate to management — potential write-off |

## Escalation Thresholds (Illustrative)

| Trigger | Threshold | Escalation |
|---------|-----------|------------|
| Individual item | > $10K | Supervisor review |
| Individual item | > $50K | Controller review |
| Total reconciling items | > $100K | Controller review |
| Item age | > 60 days | Supervisor follow-up |
| Unreconciled difference | Any | Cannot close — must resolve |

## Best Practices

1. Complete within close calendar deadline (T+3 to T+5)
2. Reconcile all balance sheet accounts on defined frequency
3. Include preparer, reviewer, date, and clear explanations
4. Segregation: reconciler ≠ transaction processor
5. Track open items to resolution
6. Root cause analysis for recurring items
7. Standardized templates across all accounts
