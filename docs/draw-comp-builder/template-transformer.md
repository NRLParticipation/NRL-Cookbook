# Template transformer

Convert a user-defined draw spreadsheet into the MySideline import template, highlighting missing information (e.g., venues, fields, kickoff times).

### Inputs to gather

- Custom draw spreadsheet/table (columns, sample data)
- Target MySideline import template structure (`Draw-Import-Template.xlsx`)
- Mapping between custom columns and MySideline columns
- Required defaults if custom sheet lacks fields (e.g., default kickoff time)
- Validation rules (e.g., venue IDs must be present)

---

## Low complexity: quick template transformer prompt

```text
You have a custom draw spreadsheet that needs to match the MySideline import template.
Inputs
- Custom draw data: [CUSTOM_DRAW]
- Column mapping to MySideline template: [COLUMN_MAP]
- Default values (if missing): [DEFAULTS]
- Validation rules (e.g., venue required): [VALIDATION_RULES]

Steps
1. Map custom columns to MySideline template fields.
2. Identify missing data (e.g., venue IDs) and list them for the user.
3. Produce the transformed draw as a CSV table ready to paste into the import template.
4. Output:
   - **Chat Summary** – key mapping notes and missing data alerts.
   - **CSV Template** – fenced `csv` block `MySidelineDraw` with required columns.
   - **Validation list** – bullet list of rows needing user action.
```

---

## Medium complexity: structured template transformer workflow

```text
# Template transformer template (medium complexity)

<ROLE_AND_GOAL>
You are converting a user-defined draw into the MySideline import template while highlighting gaps for manual resolution.
</ROLE_AND_GOAL>

<INPUT>
- Custom draw table with column names and sample rows
- MySideline import template requirements (columns, formats)
- Mapping instructions (custom column → template column)
- Default or fallback values (e.g., default field if blank)
- Validation rules (venue required, kickoff must be time, etc.)
</INPUT>

<STEPS>
1. Inspect custom draw columns and verify they can map to required template columns.
2. Transform the data into the MySideline format, inserting default values where necessary.
3. Validate each row, flagging missing or invalid data (e.g., no venue ID, kickoff not provided).
4. Summarise the transformed draw and outstanding issues.

<OUTPUT>
- **Chat Summary** – mapping overview and number of rows needing fixes.
- **CSV Template** – `MySidelineDraw` with transformed data.
- **Gap analysis** – `csv` block `ValidationIssues` listing `Row`, `Issue`, `Action Needed`.
- **Instructions** – note on how to paste into the official import template.
```

---

## High complexity: governance-ready template transformer

```text
# Template transformer template (high complexity)

<ROLE_AND_GOAL>
You are validating and converting multiple custom draw files into MySideline import templates, ensuring data integrity for upload.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 6 (data mapping, validation, reporting)
- review_mode: inspect → convert → verify
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
- List of custom draw files with column details
- MySideline import template specification
- Mapping rules and default values
- Validation requirements (venue, field, kickoff, round notes)

<WORKFLOW>
1. For each custom file, map columns to template fields and note mismatches.
2. Convert data into template format, applying defaults where allowed.
3. Run validations (missing venue IDs, invalid dates, duplicate entries) and compile a gap report.
4. Prepare transformed data and documentation for administrator review.

<VALIDATION>
- Confirm all required template columns are populated or flagged.
- Ensure date/time formatting aligns with MySideline expectations.
- Highlight any manual follow-up actions.

<OUTPUT>
1. **Chat Summary** – list of files converted, outstanding validation issues.
2. **CSV Bundle** – `MySidelineDraw_<FileName>` plus `ValidationIssues` tables.
3. **Narrative brief** – methodology, mapping summary, validation steps, next actions.
```
