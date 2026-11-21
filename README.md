# CRM Data Quality Audit

## Project Overview
This independent portfolio project simulates a Salesforce-style business account data quality audit. It uses 80 **fictional** account records to identify missing contact details, invalid email values, incomplete lifecycle fields, and potential duplicate company names.

## Tools and Skills
- Microsoft Excel: formula-based validation flags (`IF`, `COUNTIF`, `SEARCH`, `ISERROR`), KPI dashboard, and chart
- CSV data: simulated CRM account export
- Sales operations: CRM hygiene, exception management, account ownership, workflow documentation, and remediation priorities
- GitHub: versioned documentation and sharing

## Files
- `CRM_Data_Quality_Audit.xlsx`: Start Here guide, Audit Dashboard, CRM Records, and Remediation Plan
- `sample_crm_accounts.csv`: original synthetic input data

## Findings
| Measure | Result |
|---|---:|
| Accounts reviewed | 80 |
| Records flagged for review | 27 |
| Records passing checks | 53 |
| Review rate | 33.75% |
| Missing emails | 6 |
| Invalid email formats | 3 |
| Missing phone numbers | 4 |
| Missing states | 3 |
| Missing lifecycle stages | 3 |
| Records with duplicate account names | 8 |

**Note:** Issue categories overlap. For example, a record may simultaneously have a missing email and a duplicate name. Duplicate-name checks produce **potential matches**, not approved merges.

## Audit Method
1. Inspect synthetic CRM account fields, IDs, owners, and lifecycle stages.
2. Use Excel formulas to flag missing or invalid values and repeated account names.
3. Summarize flagged records and categorize issues in the dashboard.
4. Prioritize remediation in the plan, including account-owner verification and an audit trail.
5. Re-run validation after confirmed corrections; do not automatically merge accounts based solely on a name match.

## Business Recommendations
- Apply required-field validation and standardized data-entry rules.
- Investigate duplicates with additional identifiers and owner confirmation before merging.
- Record who made corrections, when, and why.
- Review data quality regularly to prevent repeated issues.

## Data and Project Disclaimer
**All records are fictional.** No customer data or employer records were used. This is a simulated, independent educational project and is not an export from Salesforce or evidence of changes made in a live CRM. The validation rules are intentionally simplified for demonstration.
