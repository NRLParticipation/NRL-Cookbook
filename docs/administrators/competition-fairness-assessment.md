# Competition fairness assessment templates

**Category:** Administrators  
**Template type:** Interactive content creation

**Collect these inputs before you start:**

- [LEAGUE_NAME]
- [NUMBER_OF_DIVISIONS]
- [AUDIT_FOCUS_ITEMS - e.g., home/away balance, bye spacing, travel load, rest days, finals positioning]
- [MISSION_STATEMENT]


Review season draws to confirm every club receives a fair balance of home fixtures, travel, byes, and divisional matchups before the competition begins.

---

## Low complexity: competition fairness prompt

Use this when you have a single draw export and need a fast fairness check with ready-to-share recommendations.

```text
You are a competition administrator reviewing the latest MySideline "Matches Detail" export (columns include `Competition Season`, `Competition Name`, `Pool Name`, `Round Type`, `Round Number`, `Venue`, `Date & Time`, `Home Team`, `Away Team`, plus `Bye` and `Tba` flags) to check whether divisions are fair. Start by acknowledging the administrator's [AUDIT_FOCUS_ITEMS] so your assessment targets the areas they care about (e.g., home/away balance, bye spacing, travel load, finals preparation). Treat each row as a scheduled fixture and ignore entries flagged as byes (`Bye = 'BYE'` or `Home Team`/`Away Team` missing) or placeholders (`Tba = 'TBA'`). Using the remaining data, count how many home and away games each team has, check how many byes each team has and whether they are fairly shared, and make sure each team is playing all the other teams in their `Pool Name` (division) and note how often. When discussing travel, state that detailed distance analysis may be limited because the export only contains venue names, not full addresses, and note any data gaps that prevent deeper review. Respond with two outputs:
1. **Chat Summary** – 3-4 sentences highlighting the biggest fairness issues, data gaps, and the recommended next action for administrators.
2. **CSV Export Set** – Provide a short instruction line telling the user they can copy each CSV block into its own `.csv` file (or paste into Excel using Data → From Text/CSV), then supply three CSV code blocks labelled `TeamBreakdown`, `DivisionSummary`, and `Recommendations`. Each block should include column headers and rows formatted as comma-separated values.
```

---

## Medium complexity: competition fairness workflow

Pick this workflow when you can supply a structured draw file and want division-level diagnostics that can be handed to scheduling staff.

```text
# Competition fairness review template (medium complexity)

<ROLE_AND_GOAL>
You are a competition administrator tasked with reviewing the fairness of a rugby league draw to ensure teams are treated equitably across the season.
</ROLE_AND_GOAL>

<INPUT>
Provide the following information:
- **Matches Detail export** from MySideline (columns should include at minimum: Competition Season/Name, Pool Name, Round Type, Round Number, Date & Time, Venue, Home Team/ID, Away Team/ID, Bye, Tba). Note whether any columns are missing.
- **Optional travel context** such as preferred venue suburbs or home venue addresses if available (acknowledge if not supplied).
- **Audit focus items** administrators want reviewed (e.g., home/away balance, bye sequencing, travel load, rest days, finals positioning).
</INPUT>

<STEPS>
1. Confirm the **Audit focus items** and restate how the assessment will address each priority.
2. Clean the dataset by removing rows marked as byes (`Bye` column not blank or `Home Team`/`Away Team` missing) or `Tba` placeholders.
3. Break the draw down by `Pool Name` (division/age group) and confirm all fixtures are assigned.
4. For each team, calculate:
   - Number of home games.
   - Number of away games.
   - Number of byes.
5. Assess whether byes are evenly distributed across the teams and season.
6. Check whether each team is scheduled to play all other teams in their division, and record how many times they meet.
7. Comment on travel balance using available venue information; if detailed addresses are missing, explicitly note the limitation and what additional data would help.
8. Provide an overall fairness assessment across divisions, linking findings back to the **Audit focus items** and referencing the exact MySideline columns used.
9. Recommend practical changes (e.g., rebalancing venues, adjusting fixtures, reassigning byes) to make the competition fairer and more equitable.
</STEPS>

<CONSTRAINTS>
- Use only the data provided in the Matches Detail export.
- Highlight any missing columns (e.g., absent venue addresses) that limit travel fairness assessment.
- Keep recommendations realistic (small fixture adjustments rather than rewriting the whole season).
- Ensure analysis is clear and actionable for administrators.
</CONSTRAINTS>

- **Chat Summary** – 3-4 bullet points capturing key fairness findings, data gaps, and suggested next steps.
- **CSV Export Set** – Provide a brief instruction on how to save each CSV block into Excel, then output three fenced code blocks using the `csv` language identifier:
  1. `TeamBreakdown` – per-team counts with columns for `Competition Name`, `Pool Name`, `Team`, `Home Games`, `Away Games`, `Byes`, `Audit Notes`.
  2. `DivisionSummary` – who plays whom, frequency, and fairness metrics with columns such as `Competition Name`, `Pool Name`, `Metric`, `Value`, `Observation`.
  3. `Recommendations` – recommended changes with suggested owners/next steps and alignment to **Audit focus items**, including columns `Team/Division`, `Issue`, `Suggested Action`, `Owner`, `Audit Focus Alignment`.
  Include column headers in every CSV block and reference the MySideline columns that informed each metric where relevant.
</OUTPUT>
```

---

## High complexity: competition equity orchestrator

Use this option when you must audit multiple draws, integrate venue or travel constraints, and produce a governance-ready change log.

```text
# Competition equity audit template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Integrity Lead for [LEAGUE_NAME], reviewing the full-season draw across [NUMBER_OF_DIVISIONS] divisions to confirm fairness, align with the administrator's [AUDIT_FOCUS_ITEMS], and ensure operational feasibility while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (fixture clustering, venue capacity checks, travel time estimation, fairness scoring)
- decision_mode: analyse -> recommend -> validate
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: compile only the evidence necessary to make defensible recommendations.
- Catalogue each Matches Detail export with version, date range, and completeness notes (e.g., missing rounds or competitions).
- Extract per-team fixture details (home, away, venue type, travel distance if provided, bye placement) with source citations, noting when precise travel distances cannot be calculated because venue address data is missing.
- Record any supplied policy constraints (e.g., maximum consecutive away games, venue blackout dates, development round requirements) and use the [AUDIT_FOCUS_ITEMS] list to prioritise the review.
- Log stakeholder notes (club availability, venue maintenance, broadcast commitments) and flag conflicts.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build fairness scorecards per division covering home/away balance, bye spacing, opponent frequency, rest days, and travel load where data allows, explicitly filtering out rows flagged as byes or TBA placeholders and flagging where travel analysis is limited by missing address data.
2. Detect anomalies such as three or more consecutive away games, repeated byes, or missing divisional matchups; classify by risk level.
3. Draft narrative summaries for each division, highlighting competitive balance, operational issues, and policy compliance.
4. Recommend fixture adjustments (swaps, venue changes, rescheduling) with rationale, expected impact, and prerequisites.
5. Create an action register assigning owners, deadlines, and dependencies for each change.
6. Outline communication steps for clubs, referees, and venues, including template prompts for announcements or approvals.
</WORKFLOW>

<VALIDATION>
- Cross-check proposed changes against policy constraints and available venue slots.
- Confirm that every recommendation references evidence captured in the context log.
- Highlight residual risks or data gaps requiring manual review.
</VALIDATION>

<OUTPUT>
Generate outputs in two parts:
1. **Chat Summary** – 4-5 bullet points highlighting key fairness findings, urgent risks, data gaps (especially travel limitations), and decisions required.
2. **CSV Export Set** – Provide a one-line instruction explaining how to import the CSV blocks into Excel, then output four fenced code blocks using the `csv` language identifier with the following structures:
### DivisionScorecards
- Columns: `Competition Name`, `Pool Name`, `Team`, `Home Games`, `Away Games`, `Byes`, `Opponent Count`, `Issue/Observation`, `Audit Focus Alignment`.

### RecommendationTracker
- Columns: `Team/Division`, `Issue Identified`, `Evidence (MySideline column)`, `Recommendation`, `Owner`, `Timeline`, `Priority`, `Status`.

### PolicyGovernanceNotes
- Columns: `Competition Name`, `Policy/Guideline`, `Compliance Status`, `Notes`, `Follow-up Required`.

### CommunicationChecklist
- Columns: `Task`, `Stakeholder`, `Message Purpose`, `Channel`, `Due Date`, `Owner`.
Ensure each CSV block includes headers, references the relevant MySideline columns, and uses comma-separated values that paste cleanly into Excel.
</OUTPUT>
```

---
