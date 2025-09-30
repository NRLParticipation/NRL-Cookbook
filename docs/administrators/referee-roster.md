# Referee roster templates

**Category:** Administrators  
**Template type:** Scheduling and logistics

**Collect these inputs before you start:**

- [LEAGUE_NAME]
- [NUMBER_OF_VENUES]
- [MAX_GAMES_PER_DAY]
- [TOTAL_GAMES]
- [LEAGUE_POLICY_REFERENCE]


Assign accredited referees to busy match schedules while respecting availability, travel, and workload limits.

---

## Low complexity: referee assignment prompt

Use this when you have a single weekend draw and need a quick referee allocation.

```text
Act as a community rugby league referee coordinator. I will provide referee availability (names and dates) plus the fixture list with dates, kick-off times, divisions, and venues. Allocate referees to each game by:
- Matching availability and travel feasibility
- Balancing workloads (no more than two consecutive games without a break)
- Flagging fixtures that need backup coverage
Return a table grouped by venue and date with assigned referee names, start times, and rest breaks.
```

---

## Medium complexity: structured referee roster workflow

Choose this template when you are working across multiple venues and need a clear operating plan for volunteers.

```text
# Referee roster planner template (medium complexity)

<ROLE_AND_GOAL>
You are the Referee Allocations Manager for [LEAGUE_NAME]. Build the weekly roster across [NUMBER_OF_VENUES] venues, ensuring fair workloads, adequate rest, and alignment with referee accreditation levels.
</ROLE_AND_GOAL>

<INPUT>
I will provide:
- Referee availability list (name, accreditation level, preferred divisions, available dates and times, travel constraints)
- Fixture list (game ID, division, date, time, venue, field, duration)
- Venue notes (changeover times, travel distance, parking or access limits)
</INPUT>

<STEPS>
1. Organise fixtures by venue and date, ordering by kick-off time.
2. Match referees to suitable games based on availability, accreditation level, and division preference.
3. Ensure each referee has appropriate rest windows (e.g., minimum 30 minutes between games) and avoid more than [MAX_GAMES_PER_DAY] games per referee.
4. Assign backup referees for high-priority or knockout fixtures.
5. Generate travel-friendly schedules when a referee covers multiple venues in a day, flagging required travel time.
6. Produce a communication-ready roster plus notes on gaps, clashes, or approvals needed.
</STEPS>

<CONSTRAINTS>
- Honour referee accreditation requirements for each division.
- Keep allocations within availability and travel limits provided.
- Highlight any unfilled fixtures or workload risks that require manual intervention.
</CONSTRAINTS>

<OUTPUT>
- Venue-by-venue roster table (game, referee, backup, arrival time, rest breaks)
- Referee summary (assignments per day, total games, required travel)
- List of outstanding issues or approvals needed
- Suggested follow-up messages for referees and venue managers
</OUTPUT>
```

---

## High complexity: referee scheduling orchestrator

Deploy this workflow when you must manage large rounds (50+ games per venue) and integrate referee development, travel budgets, and compliance tracking.

```text
# Comprehensive referee scheduling template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Operations Lead overseeing referee allocations across [NUMBER_OF_VENUES] venues and [TOTAL_GAMES] games this round. Create a defensible roster that balances experience, development needs, welfare, and travel costs while maintaining compliance with [LEAGUE_POLICY_REFERENCE].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (availability parsing, load balancing, travel matrix checks, compliance validation)
- decision_mode: assess -> allocate -> verify
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: assemble the data required for equitable, compliant allocations.
- Compile referee profiles (experience tier, accreditation, recent assignments, development goals).
- Summarise fixture clusters by venue, date, field, and time including game length and buffer requirements.
- Gather travel matrices or indicative travel times between venues if referees may rotate.
- Log policy constraints (maximum games per day, mandatory rest periods, development pairings, cost caps).
- Record stakeholder notes (requests from clubs, referee coach availability, special events).
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build workload baselines per referee (recent assignments, fatigue indicators) and set target ranges for this round.
2. Allocate referees to fixtures prioritising accreditation fit, development goals (e.g., pairing junior referees with mentors), and travel efficiency.
3. Schedule breaks and rotation patterns, ensuring compliance with rest and welfare rules.
4. Identify high-risk fixtures (finals, rivalry matches) and assign senior or dual referees with support staff.
5. Generate logistics outputs: arrival times, field allocations, travel instructions, and expense estimates.
6. Create contingency plans (standby list, escalation contacts) for late withdrawals or weather disruptions.

<VALIDATION>
- Verify allocations meet accreditation and welfare policies.
- Check for travel or timing conflicts across venues.
- Flag referees exceeding workload thresholds or lacking mentor coverage.
- Highlight uncovered fixtures or policy exceptions needing approval.

<OUTPUT>
Deliver a scheduling dossier containing:
### Master roster
- Comprehensive table of games, primary referee, assistant or touch judges (if provided), backup, arrival time, and venue notes.

### Referee workload summary
- Dashboard of assignments per referee, consecutive games, travel requirements, and rest periods.

### Logistics checklist
- Tasks for venue coordinators, referee coaches, and administration (briefings, equipment, expense forms).

### Contingency plan
- Standby allocations, communication tree, and risk mitigation steps.
```

---
