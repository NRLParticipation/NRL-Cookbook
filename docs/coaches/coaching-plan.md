# Coaching plan templates

**Category:** Coaches  
**Template type:** Program design and development

**Collect these inputs before you start:**

- [AGE_RANGE]
- [SESSIONS_PER_WEEK]
- [CLUB_NAME]


Use these prompts to build age-appropriate rugby league coaching plans that incorporate guidance from the NRL's official coaching resources (https://www.playrugbyleague.com/coach/coaching-resources/).

---

## Low complexity: Quick coaching plan prompt

Ideal when you need a fast session outline tailored to a specific age group and weekly schedule.

```text
"Act as an NRL community coach. Using the age range [AGE_RANGE] and [SESSIONS_PER_WEEK] training sessions per week, create a basic four-week coaching plan. All drills, safety points, and references should be drawn or adapted from the PlayRugbyLeague coaching resources (found at playrugbyleague.com/coach/coaching-resources). Provide:
• Weekly focus areas (skills, conditioning, game sense)
• Two or three recommended drills per session, with brief instructions
• Key coaching cues and safety checks
• A simple equipment list"
```

---

## Medium complexity: Structured coaching plan workflow

Choose this template when you want a richer, multi-week program that can be shared with assistant coaches and volunteers.

```text
# NRL coaching planner template (medium complexity)

<ROLE_AND_GOAL>
You are the Head Coach for a community rugby league squad. Design a training program that aligns with official NRL coaching resources, keeps players safe, and develops core skills for [AGE_RANGE] athletes across [SESSIONS_PER_WEEK] sessions per week.
</ROLE_AND_GOAL>

<INPUT>
I will provide:
- Age range ([AGE_RANGE])
- Number of sessions per week ([SESSIONS_PER_WEEK])
- Season phase (e.g., pre-season, in-season, finals)
- Squad priorities or constraints (e.g., tackle technique, fitness, limited equipment)
</INPUT>

<STEPS>
1. Review guidance from https://www.playrugbyleague.com/coach/coaching-resources/ relevant to the age range and season phase.
2. Define program goals: skill development, physical conditioning, game understanding, wellbeing.
3. Build a multi-week outline (4-6 weeks) with session themes, objectives, and progression notes.
4. Detail each session with warm-up, core drills, game application, and cool-down elements.
5. Add coaching cues, player safety considerations, and inclusivity adjustments (mixed abilities, genders, or experience).
6. Provide evaluation checkpoints for coaches to track progress and gather feedback.
</STEPS>

<CONSTRAINTS>
- Align activities with age-appropriate contact rules and NRL coaching guidance.
- Keep instructions concise so volunteers can follow them quickly.
- Highlight where additional resources or videos from the linked site can support delivery.
</CONSTRAINTS>

<OUTPUT>
- Program overview table (weeks, themes, goals)
- Session-by-session breakdown with drills and timing
- Coaching cues and safety reminders
- Equipment checklist per session
- Progress review checklist
</OUTPUT>
```

---

## High complexity: Coaching strategy orchestrator

Use this workflow when you must integrate athlete monitoring, long-term skill progression, and resource planning for a full season.

```text
# Comprehensive coaching strategy template (high complexity)

<ROLE_AND_GOAL>
You are the Director of Coaching for [CLUB_NAME], responsible for delivering a season-long development plan for [AGE_RANGE] players, running [SESSIONS_PER_WEEK] sessions per week. Leverage official NRL coaching resources to ensure alignment with best practice, welfare standards, and pathway goals.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (resource curation, skill progression mapping, load management checks)
- decision_mode: plan -> validate -> refine
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: compile only the data needed for an evidence-backed plan.
- Summarise key themes from the NRL coaching resources relevant to the squad (skill focus, safety modules, season planning guides).
- Capture squad details: player numbers, positions, experience mix, injury considerations.
- Record facility and equipment constraints, plus support staff availability.
- Note competition calendar milestones (trial games, season start, finals window).
</CONTEXT_GATHERING>

<WORKFLOW>
1. Map season phases (pre-season, in-season blocks, finals preparation) with objectives, workloads, and skill emphases.
2. Design microcycles covering each week: session goals, load management notes, recovery protocols.
3. Integrate individualisation strategies (position groups, emerging talent, return-to-play plans).
4. Curate resource links, videos, or worksheets from the official NRL site for each key skill or drill.
5. Create communication assets: briefing notes for assistant coaches, parent updates, and player goal sheets.
6. Develop monitoring tools (session review template, player feedback form, injury and attendance tracker).

<VALIDATION>
- Check workload balance against age-appropriate guidelines (contact limits, rest days).
- Ensure each phase references at least one resource from the official site.
- Highlight gaps requiring manual confirmation (facility bookings, medical approvals).

<OUTPUT>
Produce a coaching strategy pack with:
### Season roadmap
- Timeline of phases, objectives, and key events.

### Weekly microcycles
- Tables outlining sessions, focus areas, intensity notes, and recovery actions.

### Resource index
- List of linked drills, videos, and documents sourced from the NRL coaching resources site.

### Support materials
- Templates for coach briefings, player goal tracking, and parent communications.
```

---
