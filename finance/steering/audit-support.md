# Audit Support

SOX 404 control testing methodology, sample selection approaches, testing documentation standards, control deficiency classification, and common control types.

> **Important**: This skill assists with SOX compliance workflows but does not provide audit or legal advice. All testing workpapers and assessments should be reviewed by qualified financial professionals.

## SOX 404 Methodology

1. **Scoping**: Identify significant accounts and relevant assertions
2. **Risk assessment**: Evaluate risk of material misstatement
3. **Control identification**: Document controls addressing each risk
4. **Testing**: Test design and operating effectiveness of key controls
5. **Evaluation**: Assess deficiencies and severity
6. **Reporting**: Document assessment and material weaknesses

### Significant Account Criteria
- Quantitative: Balance exceeds materiality (3-5% of benchmark), high transaction volume, significant estimates
- Qualitative: Complex accounting, fraud susceptibility, prior misstatements, significant judgment

### Assertions (CEAVOP)
Completeness, Existence/Occurrence, Accuracy, Valuation, Obligations/Rights, Presentation/Disclosure

## Sample Selection Approaches

| Method | When to Use | Pros | Cons |
|--------|------------|------|------|
| **Random** | Default for large populations | Statistically valid, no bias | May miss high-risk items |
| **Targeted** | Supplement for risk-based testing | Focuses on highest risk | Not statistically representative |
| **Haphazard** | When random is impractical | Simple | Not statistically valid |
| **Systematic** | Sequential populations, even coverage | Even period coverage | Periodic patterns could bias |

### Sample Size Guidance

| Frequency | Population | Low Risk | Moderate | High Risk |
|-----------|-----------|----------|----------|-----------|
| Annual | 1 | 1 | 1 | 1 |
| Quarterly | 4 | 2 | 2 | 3 |
| Monthly | 12 | 2 | 3 | 4 |
| Weekly | 52 | 5 | 8 | 15 |
| Daily | ~250 | 20 | 30 | 40 |
| Per-transaction | 250+ | 25 | 40 | 60 |

Increase for: higher risk, prior deficiencies, new controls, external auditor reliance.

## Deficiency Classification

- **Deficiency**: Control doesn't allow timely prevention/detection of misstatements
- **Significant Deficiency**: Important enough to merit governance attention; more than inconsequential but less than material
- **Material Weakness**: Reasonable possibility of material misstatement not prevented/detected

### Aggregation
Individual deficiencies may be significant in combination. Evaluate combined effect on same process/assertion.

## Common Control Types

### IT General Controls (ITGCs)
Access controls (provisioning, de-provisioning, privileged access, periodic reviews), Change management (approval, testing, separation of environments), IT operations (batch monitoring, backup/recovery, incident management)

### Manual Controls
Management review, supervisory approval, three-way match, reconciliation prep/review, physical inventory, vendor/customer master changes

### Automated Controls
System-enforced approvals, three-way match automation, duplicate detection, credit limit enforcement, automated calculations, SoD enforcement, input validation

### IT-Dependent Manual Controls
Manual controls relying on system-generated data. Must test both the manual control AND the completeness/accuracy of underlying data (IPE testing).

### Entity-Level Controls
Tone at the top, risk assessment, audit committee oversight, internal audit, fraud risk assessment, whistleblower programs, financial reporting competence

## Evidence Standards

**Sufficient**: Screenshots, signed approvals, email approvals with identifiable approver/date, system audit logs, re-performed calculations, observation notes

**Insufficient**: Verbal confirmations alone, undated documents, evidence without identifiable performer, generic reports without timestamps
