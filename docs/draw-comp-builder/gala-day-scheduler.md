# Gala day scheduler

Design school gala day draws with fair matchups and time allocations that can be uploaded into MySideline.

### Inputs to gather

- Number of schools/teams (with IDs)
- Venue ID and field availability (start/end times, lunch break window)
- Match duration (standard for the gala games)
- Number of finals games (if applicable)
- Constraints (e.g., St Paul’s must not play before 10am, lunch 12–1 with no games, field availability limits)
- Preferred fairness rules (circular matchups, equal rest between games)
- Draw import template (e.g., `Draw-Import-Template (5).xlsx` for MySideline)

---

## Low complexity: Quick gala day prompt

```text
You are organising a school gala day with [NUMBER_OF_SCHOOLS] schools.
Inputs
- Schools with IDs: [SCHOOL_LIST]
- Venue ID and fields: [VENUE_SETUP]
- Match duration (minutes): [MATCH_DURATION]
- Number of finals games: [FINALS_GAMES]
- Constraints: [CONSTRAINTS] (e.g., St Paul’s after 10am, lunch 12–1, field availability)

Steps
1. Create a round-robin draw for the schools, ensuring circular matchups.
2. Allocate matches to field/time slots respecting match duration, buffer time, and lunch break.
3. Insert finals games after pool rounds if specified.
4. Ensure fairness (teams get similar rest, no team double-ups around lunch constraints).
5. Output:
   - **Chat Summary** – overview of schedule, fairness notes, conflicts.
   - **CSV Draw** – fenced `csv` block `GalaDayDraw` with columns `Round`, `Start`, `Field`, `Home Team`, `Away Team`, `VenueID`, `Notes`.
   - **Upload instructions** – note that data should be copied into the MySideline draw import template.
```

---

## Medium complexity: Structured gala day scheduler workflow

```text
# Gala day scheduler template (medium complexity)

<ROLE_AND_GOAL>
You are a competitions officer preparing a gala day draw for [VENUE_NAME] with [NUMBER_OF_SCHOOLS] schools, ready for MySideline upload.
</ROLE_AND_GOAL>

<INPUT>
- Schools with IDs and any special constraints (start-time restrictions)
- Match duration and buffer time
- Field availability and lunch breaks
- Number of finals games/structure
- Fairness rules (equal rest windows, circular draw)
</INPUT>

<STEPS>
1. Validate school list and identify constraints.
2. Generate pool/circular matchups for the number of schools provided.
3. Build a timetable across available fields, skipping lunch (12–1) or other blackout periods.
4. Schedule pool games followed by finals, ensuring constraints (e.g., St Paul’s after 10am, balanced rest).
5. Produce draw and upload-ready schedule.

<OUTPUT>
- **Chat Summary** – bullet list covering draw structure and constraint handling.
- **CSV Draw** – `GalaDayDraw` with columns `Round`, `Start`, `End`, `Field`, `Home Team`, `Away Team`, `VenueID`, `Notes`.
- **Fairness report** – `csv` block `RestAnalysis` listing `Team`, `Rest Between Games`, `Earliest Kick-off`, `Comments`.
- **Upload instructions** – steps to paste into the MySideline draw import template.
```

---

## High complexity: Governance-ready gala day orchestration

```text
# Gala day orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Integrity Lead planning a large gala day with multiple pools and finals. Create a schedule that balances fairness, venue use, and administrative constraints, ready for MySideline.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (draw generation, scheduling, fairness analysis)
- delivery_mode: plan → schedule → verify
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
- School list with IDs and special notes
- Venue and field availability including lunch/blackout periods
- Match duration and buffer
- Finals format (e.g., semifinals, grand final)
- Fairness policies (rest windows, circular matchups, equal field exposure)

<WORKFLOW>
1. Create pool draws using circular round robin or split pools if necessary.
2. Schedule pool matches across fields, ensuring no games occur during lunch (12–1) and respecting constraints (e.g., St Paul’s after 10am).
3. Slot finals games after pool play, leaving adequate rest between semifinals and finals.
4. Calculate fairness metrics (total rest time, field usage, kickoff spread) and adjust as required.
5. Document unresolved conflicts or games needing venue/time adjustments.

<VALIDATION>
- Confirm schedule adheres to match durations, lunch blackout, and special constraints.
- Ensure teams receive fair rest periods and field allocations.
- Highlight manual follow-ups (e.g., additional venues) for unscheduled games if present.

<OUTPUT>
1. **Chat Summary** – 4-5 bullet points summarising schedule structure and fairness.
2. **CSV Bundle** – `GalaDayDraw`, `RestAnalysis`, and `ConflictRegister` with detailed notes.
3. **Narrative brief** – markdown section summarising methodology, fairness outcomes, and manual action checklist, plus instructions for filling the MySideline draw import template (`Draw-Import-Template (5).xlsx`).
```
