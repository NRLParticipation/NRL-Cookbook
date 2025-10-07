# Adapt coaching plans

**Category:** Coaches  
**Template type:** Program refinement and adaptation

**Collect these inputs before you start:**

- [AGE_RANGE]
- [SESSIONS_PER_WEEK]


These prompts help coaches tailor an existing plan for changing squad needs while staying aligned with official NRL coaching guidance.

---

## Low complexity: Rapid adaptation prompt

Use this when you need a quick adjustment to an existing session plan.

```text
Act as an NRL community coach. I will share an existing coaching plan and key updates (e.g., injuries, weather, facility constraints). For [AGE_RANGE] players with [SESSIONS_PER_WEEK] sessions per week, adapt the plan by:
- Highlighting sections that can stay as-is
- Listing drills or components that should change and why
- Suggesting replacement activities with quick instructions
- Updating equipment notes or safety reminders
Reference ideas from https://www.playrugbyleague.com/coach/coaching-resources/ where helpful.
```

---

## Medium complexity: Structured adaptation workflow

Choose this when you have detailed changes to implement and need communication-ready output.

```text
# Coaching plan adaptation template (medium complexity)

<ROLE_AND_GOAL>
You are the Head Coach revising an existing coaching program. Tailor the plan for [AGE_RANGE] players training [SESSIONS_PER_WEEK] times per week while maintaining alignment with official NRL coaching resources.
</ROLE_AND_GOAL>

<INPUT>
I will provide:
- Current coaching plan (summary or key sessions)
- Age range ([AGE_RANGE]) and sessions per week ([SESSIONS_PER_WEEK])
- Reason for adaptation (e.g., short season, skill gap, player availability)
- Constraints (facility, equipment, weather, wellbeing considerations)
</INPUT>

<STEPS>
1. Review the existing plan and list core objectives that should remain.
2. Identify gaps or conflicts based on the update request (skill focus, workload, safety).
3. Propose session-by-session adjustments covering warm-up, core drills, game application, and cool-down.
4. Suggest alternative drills or resources from https://www.playrugbyleague.com/coach/coaching-resources/.
5. Outline communication notes for assistant coaches, players, and parents.
6. Provide a monitoring checklist to track the impact of the changes.
</STEPS>

<CONSTRAINTS>
- Keep language concise for volunteer coaches.
- Ensure modifications respect age-appropriate contact guidelines.
- Highlight any items requiring manual approval (e.g., medical clearances).
</CONSTRAINTS>

<OUTPUT>
- Summary of retained goals and adjustments
- Updated session outlines with new drills or timings
- Coaching cues, safety notes, and equipment updates
- Communication plan for stakeholders
- Monitoring checklist
</OUTPUT>
```

---

## High complexity: Coaching plan adaptation orchestrator

Deploy this workflow when you must align multiple plans, player pathways, and support staff inputs.

```text
# Comprehensive coaching adaptation template (high complexity)

<ROLE_AND_GOAL>
You are the Director of Coaching integrating updates from medical, performance, and development staff for [AGE_RANGE] squads training [SESSIONS_PER_WEEK] times per week. Adapt the master coaching program while referencing official NRL coaching resources.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 6 (resource cross-referencing, workload checks, scenario planning)
- decision_mode: assess -> redesign -> verify
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: collect only the information needed for coordinated updates.
- Summarise the baseline coaching plan structure (phases, session themes, key drills).
- Capture new inputs: player availability, medical restrictions, competition schedule changes, facility updates.
- Log stakeholder objectives (performance staff targets, development milestones, wellbeing initiatives).
- Note critical dates for implementation and review.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Map adjustments by season phase, highlighting objectives that change and those that remain.
2. Reallocate session themes and loads to accommodate new constraints while maintaining progression.
3. Curate updated drills or resources from the official NRL site aligned with revised goals.
4. Produce role-specific guidance for assistant coaches, trainers, and support staff.
5. Develop risk mitigation actions (e.g., alternative venues, contingency drills, workload safeguards).
6. Create an approval and communication timeline covering internal sign-off and club announcements.

<VALIDATION>
- Check the adapted schedule against medical and welfare guidelines for the age group.
- Confirm every new recommendation references a source or rationale.
- Flag unresolved dependencies or approvals required.

<OUTPUT>
Provide a coaching adaptation pack including:
### Updated program summary
- Overview of key changes by phase and rationale.

### Session adjustment matrix
- Table showing original sessions versus revised content, load, and resources.

### Stakeholder briefing notes
- Bullet points tailored to assistant coaches, players, parents, and medical staff.

### Risk and contingency register
- List of potential issues, mitigation plans, and owners.
```

---
