# Field allocation scheduler

**Prerequisite:** Have the MySideline Matches Detail export ready with fixtures set to `TBD` times. Filter the report to the specific weekend(s) you want to schedule.

This workflow assigns kick-off times and fields across venues while respecting official game durations, field sharing rules, and administrator sequencing preferences.

### Inputs to gather

- Filtered Matches Detail report (e.g., `Weekend's games.xlsx`) including competition, teams, age group, venue, date, and `TBD` time placeholders
- Field inventory per venue (field count, operating hours, lighting limits)
- Official game duration/field share rules (fixed table provided below)
- Sequencing preferences (e.g., juniors before seniors, first grade last, minimum rest between games)
- Venue allocation rules (e.g., U18 always on Field 1, minis limited to certain fields)
- Buffer time between games (default 5 minutes unless specified)

**Official duration and field share rules (fixed):**
- Mini League (U6–U7): 40 mins, 25% of field (4 games per field slot)
- Mod League (U8–U9): 40 mins, 50% of field (2 games per field slot)
- Junior League (U10–U12): 50 mins, 100% of field
- Youth League (U13–U15): 60 mins, 100% of field
- Senior Youth (U16–U18): 70 mins, 100% of field
- Open Age (Seniors/Women’s): 90 mins, 100% of field

---

## Low complexity: Quick field allocation prompt

```text
You have filtered the MySideline Matches Detail report to the upcoming weekend and need to set times/fields.
Inputs
- Matches Detail report: [MATCHES_REPORT]
- Field inventory per venue: [FIELD_SETUP]
- Sequencing preferences: [SEQUENCING_RULES]
- Venue allocation exceptions: [VENUE_RULES]
- Buffer between games (default 5 minutes): [BUFFER]

Steps
1. For each fixture, determine required duration and field share using the official game duration table.
2. Build a scheduling matrix per venue and field, respecting operating hours and lighting limits.
3. Apply sequencing rules (e.g., junior grades earlier, seniors later) and venue allocation requirements (e.g., U18 on Field 1).
4. Assign start times and fields, filling from earliest available slot and grouping club games where possible.
5. Output:
   - **Chat Summary** – key scheduling decisions and any games needing manual intervention.
   - **CSV Schedule** – fenced `csv` block `FieldSchedule` with columns `Venue`, `Field`, `Start`, `End`, `Competition`, `Division`, `Home Team`, `Away Team`, `Field Share`, `Notes`.
   - **Anomaly list** – bullet list of fixtures that do not fit or require alternate venues/times.
```

---

## Medium complexity: Structured field allocation workflow

```text
# Field allocation scheduler template (medium complexity)

<ROLE_AND_GOAL>
You are a competitions officer assigning kick-off times to [WEEKEND_DATE] fixtures using filtered Matches Detail data and venue capacity rules.
</ROLE_AND_GOAL>

<INPUT>
- Filtered Matches Detail report (CSV/table)
- Official duration/field share table (provided)
- Field inventory with operating windows, lighting limits, maintenance breaks
- Sequencing and venue allocation rules (admin priorities)
- Buffer time between games
</INPUT>

<STEPS>
1. Validate inputs and note missing venue or field details.
2. Map each fixture to its duration and field share requirement.
3. Build a time-slot planner per venue, inserting buffer times and accounting for fields that can operate late.
4. Allocate fixtures according to sequencing rules (e.g., minis first, seniors last) and venue allocation requirements (e.g., U18 Field 1).
5. Balance field usage by shuffling fixtures if a field becomes overloaded; ensure clubs have reasonable gaps between games if requested.
6. Record games that cannot be placed due to capacity or rule conflicts and propose alternative slots/venues.

<OUTPUT>
- **Chat Summary** – bullet list of schedule highlights and unresolved issues.
- **CSV Export** – `FieldSchedule` with columns `Venue`, `Field`, `Start`, `End`, `Competition`, `Division`, `Home Team`, `Away Team`, `Field Share`, `Notes`.
- **Anomalies report** – `csv` block `SchedulingAnomalies` listing `Game`, `Issue`, `Suggested Action`.
- **Manual upload reminder** – note that times must be entered manually into MySideline.
```

---

## High complexity: Governance-ready field allocation orchestrator

```text
# Field allocation orchestrator template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Integrity Lead generating venue schedules across multiple days/venues using matches set to TBD times. Ensure efficiency, fairness, and clear escalation triggers.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (slot optimisation, fairness scoring, conflict resolution)
- scheduling_mode: plan → simulate → verify
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
- Filtered Matches Detail report(s) for the scheduling window
- Field inventory with operating hours, lighting, and shared-surface constraints
- Official duration/field share rules (fixed table)
- Sequencing/venue policies (juniors first, field locks, broadcast slots)
- Buffer times and any mandated washout slots

<WORKFLOW>
1. Categorise fixtures by venue, age group, and duration.
2. Create slot grids for each venue/field, respecting operating windows and lighting limits.
3. Optimise scheduling to minimise idle time, respect sequencing priorities, and balance club logistics.
4. Calculate fairness metrics (e.g., rest gaps between games for clubs with multiple teams, distribution of prime-time slots).
5. Flag unscheduled fixtures or conflicts (e.g., insufficient field capacity, late-night restrictions) and propose mitigation.
6. Prepare documentation for administrator approval.

<VALIDATION>
- Verify every scheduled game adheres to duration/field share rules.
- Confirm sequencing and venue allocation policies are met or note exceptions.
- List outstanding items (e.g., games needing new venue/day) for manual follow-up.

<OUTPUT>
1. **Chat Summary** – 4-5 bullet points outlining scheduling efficiency, fairness notes, and conflicts.
2. **CSV Bundle** – `FieldSchedule` plus `SchedulingAnomalies` for unresolved games.
3. **Narrative brief** – markdown section summarising approach, utilisation stats per venue/field, fairness observations, and manual action checklist.
```
