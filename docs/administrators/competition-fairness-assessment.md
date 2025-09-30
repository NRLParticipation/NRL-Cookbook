# Competition fairness assessment templates

**Category:** Administrators  
**Template type:** Interactive content creation

**Collect these inputs before you start:**

- [LEAGUE_NAME]
- [NUMBER_OF_DIVISIONS]
- [POLICY_REFERENCE]
- [MISSION_STATEMENT]


Review season draws to confirm every club receives a fair balance of home fixtures, travel, byes, and divisional matchups before the competition begins.

---

## Low complexity: competition fairness prompt

Use this when you have a single draw export and need a fast fairness check with ready-to-share recommendations.

```text
You are a competition administrator reviewing a rugby league draw to see if it is fair. Using the dataset with rounds, teams, venues, dates, times, byes, and divisions, count how many home and away games each team has, check how many byes each team has and whether they are fairly shared, and make sure each team is playing all the other teams in their division and note how often. Finally, provide a short summary for each team and division, highlight any imbalances, and give simple recommendations to make the competition more even.
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
- **Competition draw dataset** including round number, round type, home team and ID, away team and ID, venue name and ID, field number, date, time, BYE/TBA flags, and division or age group.
</INPUT>

<STEPS>
1. Break the draw down by division.
2. For each team, calculate:
   - Number of home games.
   - Number of away games.
   - Number of byes.
3. Assess whether byes are evenly distributed across the teams and season.
4. Check whether each team is scheduled to play all other teams in their division, and record how many times they meet.
5. Provide an overall fairness assessment across divisions.
6. Recommend practical changes (e.g., rebalancing venues, adjusting fixtures, reassigning byes) to make the competition fairer and more equitable.
</STEPS>

<CONSTRAINTS>
- Use only the data provided in the draw.
- Keep recommendations realistic (small fixture adjustments rather than rewriting the whole season).
- Ensure analysis is clear and actionable for administrators.
</CONSTRAINTS>

<OUTPUT>
- A fairness report for each team (home games, away games, byes).
- Division-level summary of matchups (who plays whom, and how often).
- Assessment of whether the competition is fair.
- Recommendations for changes to improve fairness.
</OUTPUT>
```

---

## High complexity: competition equity orchestrator

Use this option when you must audit multiple draws, integrate venue or travel constraints, and produce a governance-ready change log.

```text
# Competition equity audit template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Integrity Lead for [LEAGUE_NAME], reviewing the full-season draw across [NUMBER_OF_DIVISIONS] divisions to confirm fairness, compliance with [POLICY_REFERENCE], and operational feasibility. Your goal is to surface imbalances, propose targeted adjustments, and brief leadership on required actions while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (fixture clustering, venue capacity checks, travel time estimation, fairness scoring)
- decision_mode: analyse -> recommend -> validate
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: compile only the evidence necessary to make defensible recommendations.
- Catalogue each draw source with version, date range, and completeness notes.
- Extract per-team fixture details (home, away, venue type, travel distance if provided, bye placement) with source citations.
- Record policy constraints such as maximum consecutive away games, venue blackout dates, or development round requirements.
- Log stakeholder notes (club availability, venue maintenance, broadcast commitments) and flag conflicts.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build fairness scorecards per division covering home or away balance, bye spacing, opponent frequency, rest days, and travel load where data allows.
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
Generate a markdown briefing containing:
### Division fairness scorecards
- Tables summarising fairness indicators and anomalies by team.

### Recommendation tracker
- List of proposed changes with priority, owner, timeline, and decision status.

### Policy compliance notes
- Summary of how the draw aligns with relevant competition rules, plus any exceptions that need sign-off.

### Communication checklist
- Sequenced tasks and message prompts for notifying stakeholders about approved adjustments.
</OUTPUT>
```

---
