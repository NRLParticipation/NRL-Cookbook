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
5. Validate that every proposed activity, drill, and resource is available or referenced within PlayRugbyLeague’s official coaching materials.
6. Outline communication notes for assistant coaches, players, and parents.
7. Provide a monitoring checklist to track the impact of the changes.
</STEPS>

<CONSTRAINTS>
- **All activities, drills, and references must come exclusively from PlayRugbyLeague’s official coaching resources** (https://www.playrugbyleague.com/coach/coaching-resources/).
- Keep language concise for volunteer coaches.
- Ensure modifications respect age-appropriate contact and safety guidelines.
- Highlight any items requiring manual approval (e.g., medical clearances).
</CONSTRAINTS>

<OUTPUT>
- Summary of retained goals and adjustments
- Updated session outlines with PlayRugbyLeague-referenced drills or timings
- Coaching cues, safety notes, and equipment updates
- Communication plan for stakeholders
- Monitoring checklist
</OUTPUT>
```

---

