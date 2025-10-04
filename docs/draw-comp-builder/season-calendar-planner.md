# Season calendar planner

Plan the overall rugby league calendar leading into finals and the grand final. Provide the inputs listed below so the assistant can offer multiple scheduling options, analyse impact for different team counts, and highlight engagement risks (e.g., Easter, school holidays).

### Inputs to gather

- Fixed grand final date (e.g., 05/09/2025)
- Required finals weeks (e.g., 3)
- Fixed season start date or earliest acceptable start date
- Target competition window (e.g., 1 March – 15 September)
- Weeks or weekend ranges with no games (holidays, representative rounds)
- Team counts to assess (e.g., 6, 8, 10, 12, 14)
- Notes about public holidays, school holidays, or major events
- Preferred game day(s), washout round preferences, and reserve weekends

---

## Low complexity: Quick Season Calendar Prompt

```text
You are planning the upcoming rugby league season and want suggested competition calendars. Inputs:
- Grand final date: [GRAND_FINAL_DATE]
- Finals weeks: [FINALS_WEEKS]
- Fixed/earliest start date: [START_DATE]
- Target competition window: [COMP_WINDOW]
- No-game weekends (holidays, representative rounds): [NO_GAME_WEEKS]
- Team counts to analyse (e.g., 6, 8, 10, 12, 14): [TEAM_COUNTS]
- Preferred game day and washout round preference: [PREFERENCES]

Steps:
1. Generate start-date options within the target window that leave enough weekends for regular season plus finals.
2. For each team-count scenario, build a regular-season calendar (single round robin) and note required weekends. Highlight if double rounds or midweek fixtures would be needed.
3. Insert finals weeks leading to the grand final date and ensure no finals land on no-game weekends.
4. Identify holiday or gap periods (e.g., Easter, school holidays) and note if multiple consecutive weekends lack games.
5. Suggest a washout/recovery round that fits between regular season and finals or within the target window.
6. Output:
   - **Chat Summary** – 3-4 sentences summarising recommended start dates and key risks.
   - **CSV Calendar** – fenced `csv` block `SeasonCalendar` with columns `Scenario`, `Start Option`, `Round`, `Weekend`, `Type`, `Notes`.
```

---

## Medium complexity: Structured Season-Planning Workflow

```text
# Season calendar planner template (medium complexity)

<ROLE_AND_GOAL>
You are a competition administrator building next season’s calendar, aiming to propose optimal start dates and season lengths before locking in finals on [GRAND_FINAL_DATE].
</ROLE_AND_GOAL>

<INPUT>
- Grand final date and number of finals weeks
- Fixed or earliest start date (if any)
- Target competition window (start/end months)
- No-game weekends (holidays, rep rounds, venue blackouts)
- Team counts to model (6, 8, 10, 12, 14)
- Preferred washout weekend(s) or reserve weeks
- Any mandatory themed rounds (e.g., ANZAC Day)
</INPUT>

<STEPS>
1. Convert all inputs into a calendar timeline, tagging blackout weekends and target window boundaries.
2. For each team-count scenario:
   a. Calculate the number of weekends required for single and double round robins.
   b. Generate candidate start dates within the target window; discard those that push finals past the grand final date.
   c. Create round-by-round schedules, skipping no-game weekends, and reserve a washout weekend if feasible.
3. Append finals weeks leading into the grand final, ensuring they respect the finals count and blackout dates.
4. Perform engagement analysis: flag long gaps without games, clash with Easter or school holidays, and note impact on fan engagement.
5. Summarise trade-offs for each start-date option (e.g., early start avoids school holidays, later start forces double rounds).

<OUTPUT>
- **Chat Summary** – bullet list with recommended start date(s), washout round suggestion, and critical risks.
- **CSV Exports** – instructions followed by two `csv` blocks:
  1. `SeasonCalendar` – `Scenario`, `Start Date Option`, `Round`, `Weekend`, `Type (Regular/Finals/Washout)`, `Notes`.
  2. `ImpactAnalysis` – `Scenario`, `Metric`, `Value`, `Risk/Benefit`, `Recommendation`.
- **Planning notes** – markdown paragraph describing engagement impacts and suggested mitigations.
```

---

## High complexity: Governance-Ready Season Orchestration

```text
# Season orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Integrity Lead producing start-date options and season calendars for board review, ensuring finals occur on [GRAND_FINAL_DATE] and the competition fits within [COMP_WINDOW].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 9 (calendar simulation, scenario comparison, risk scoring)
- decision_mode: explore → compare → recommend
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
- Grand final date, finals format, and venue availability
- Start date constraints and target competition window
- No-game weekends, public/school holidays, representative commitments
- Team-count scenarios to model (6, 8, 10, 12, 14)
- Preferred washout weekend and reserve dates
- Required themed rounds (e.g., Indigenous Round, ANZAC Day)

<WORKFLOW>
1. Build a master calendar covering the competition window, labelling blackout weekends and potential washout slots.
2. For each scenario, simulate regular-season schedules (single round robin and double round robin if needed), ensuring finals conclude on the grand final date.
3. Provide start-date options (e.g., early, mid, late) and quantify effects on season length, holiday clashes, and required double rounds.
4. Evaluate engagement impact: count holiday gaps, back-to-back interruptions, and note weeks without games.
5. Recommend washout/catch-up weekends and highlight scenarios that best balance duration, engagement, and blackout constraints.
6. Compile governance documentation summarising assumptions, trade-offs, and next decisions.

<VALIDATION>
- Confirm each option fits within the competition window and respects no-game weekends.
- Verify finals align with policy and the grand final date.
- Score scenarios on key metrics (duration, holiday conflicts, reserve weekends, fairness) and flag residual risks.

<OUTPUT>
1. **Chat Summary** – 4-5 bullet points comparing start-date options, engagement risks, and preferred scenario.
2. **CSV Bundle** – fenced `csv` blocks:
   - `SeasonCalendar` – `Scenario`, `Start Option`, `Round`, `Weekend`, `Stage`, `Notes`.
   - `ScenarioMetrics` – `Scenario`, `Start Option`, `Total Weekends`, `Holiday Clashes`, `Washout Availability`, `Notes`.
   - `DecisionLog` – `Decision`, `Rationale`, `Data Source`, `Approver`, `Status`.
3. **Narrative brief** – markdown section covering scenario comparison, engagement impact (e.g., Easter, school holidays), recommended washout round, and approval checklist.
```
