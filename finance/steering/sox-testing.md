# /sox-testing

Generate sample selections, create testing workpapers, document control assessments, and provide testing templates for SOX 404 internal controls over financial reporting.

> **Important**: This command assists with SOX compliance workflows but does not provide audit or legal advice. All testing workpapers and assessments should be reviewed by qualified financial professionals.

## Usage

```
/sox-testing [control-area] [period]
```

### Arguments
- `control-area` — `revenue-recognition`, `procure-to-pay`/`p2p`, `payroll`, `financial-close`, `treasury`, `fixed-assets`, `inventory`, `itgc`, `entity-level`, `journal-entries`, or any specific control ID
- `period` — Testing period (e.g., `2024-Q4`, `2024`, `2024-H2`)

## Workflow

### 1. Identify Controls to Test

Present the control matrix:

| Control # | Control Description | Type | Frequency | Key/Non-Key | Risk | Assertion |
|-----------|-------------------|------|-----------|-------------|------|-----------|

**Types**: Manual, Automated, IT-Dependent Manual
**Assertions (CEAVOP)**: Completeness, Existence, Accuracy, Valuation, Obligations/Rights, Presentation

### 2. Determine Sample Size

| Control Frequency | Population | Low Risk | Moderate Risk | High Risk |
|------------------|-----------|----------|---------------|-----------|
| Annual           | 1         | 1        | 1             | 1         |
| Quarterly        | 4         | 2        | 2             | 3         |
| Monthly          | 12        | 2-4      | 3             | 4         |
| Weekly           | 52        | 5        | 8             | 15        |
| Daily            | ~250      | 20       | 30            | 40        |
| Per-transaction  | 250+      | 25       | 40            | 60        |

### 3. Generate Sample Selection

```
SAMPLE SELECTION
Control: [ID] — [Description]
Period: [Testing period]
Population: [Count] items, $[Total value]
Sample size: [N] items
Selection method: [Random/Systematic/Targeted]

| Sample # | Transaction Date | Reference/ID | Amount | Selection Basis |
|----------|-----------------|--------------|--------|-----------------|
```

### 4. Create Testing Workpaper

Generate template with: Control identification, test objective, test procedures, expected evidence, results table, exceptions table, and conclusion section (Effective / Deficiency / Significant Deficiency / Material Weakness).

### 5. Common Control Templates by Area

- **Revenue Recognition**: Sales order approval, delivery evidence, recognition timing, pricing accuracy, credit memo approval
- **Procure to Pay**: PO approval, three-way match, vendor master changes, payment approval, duplicate prevention
- **Financial Close**: Reconciliation completeness, JE approval, management review, consolidation, disclosure checklist
- **ITGC**: Access provisioning/de-provisioning, privileged access reviews, change management, batch monitoring, backup/recovery

### 6. Document Control Assessment

Classify deficiencies: Deficiency → Significant Deficiency → Material Weakness. Consider likelihood, magnitude, and compensating controls.

### 7. Output

1. Control matrix for the selected area
2. Sample selections with methodology documentation
3. Testing workpaper templates with pre-populated test steps
4. Results documentation template
5. Deficiency evaluation framework
6. Suggested remediation actions for noted deficiencies
