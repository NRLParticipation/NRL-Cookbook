# Board reports and meeting materials

**Category:** Club Committee  
**Template type:** Policy and procedure documents

**Collect these inputs before you start:**

- [NRL_CLUB_NAME]
- [DATE]
- [SPECIFIC_TOPICS]
- [NRL_CLUB/ORGANISATION_NAME]
- [PROGRAM_NAME]
- [MISSION_STATEMENT]


Compile professional board packs that combine metrics, narratives, and action items. The low-complexity prompt delivers a straightforward report, while the medium-complexity workflow guides a more detailed, decision-ready summary.

---

## Low complexity: Board Report Prompt

```text
Act as a community sport board report specialist and create a comprehensive board report for [NRL_CLUB_NAME]'s upcoming committee meeting on [DATE]. Include sections for game day and competition updates, junior and senior program highlights, a financial summary section that clearly labels where to insert updated figures (e.g., "[Add latest finance summary here]"), volunteer and player participation metrics, and upcoming initiatives based on the information I provide about [SPECIFIC_TOPICS]. Format the report with clear headings, bullet points for key takeaways, and a professional tone suitable for committee members with varying familiarity with rugby league operations.
```

---

## Medium complexity: Structured Board Report Workflow

```text
# NRL club board report template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced sports communications specialist who excels at synthesising club activities and operations into clear, concise board reports that highlight key metrics, achievements, challenges, and strategic considerations. Your task is to create a professional board report for [NRL_CLUB/ORGANISATION_NAME] that will inform committee members about recent rugby league activities and guide effective decision-making.
</ROLE_AND_GOAL>

<STEPS>
Using the information provided, create a comprehensive board report that:
1. Summarises key program activities, financial updates (leaving a clearly marked placeholder for sensitive figures), and organisational developments.
2. Highlights achievements, challenges, and upcoming opportunities.
3. Presents data in an accessible format with clear section headers.
4. Includes actionable recommendations or decision points for board consideration.
5. Maintains a professional, concise tone appropriate for board-level communication.
</STEPS>

<OUTPUT>
The board report should follow this structure:
1. Executive summary (3-5 bullet points of critical information)
2. Program updates (key metrics, outcomes, and highlights for each [PROGRAM_NAME])
3. Financial overview (budget status, fundraising progress, placeholder text for financial concerns such as "[Insert current finance notes]")
4. Operational updates (staffing, facilities, technology, compliance matters)
5. Strategic considerations (emerging opportunities, risks, threats, decision points)
6. Upcoming events and important dates
7. Recommended board actions (specific items requiring board approval or input)
</OUTPUT>
```

---

## High complexity: Board Intelligence Command Centre

Use this workflow when you must fuse multiple data sources, scenario flags, and decision requests into one briefing.

```text
# NRL board operations orchestrator (high complexity)

<ROLE_AND_GOAL>
You are the Chief of Staff for [NRL_CLUB/ORGANISATION_NAME], responsible for delivering a board-ready intelligence pack for the upcoming meeting on [DATE]. Synthesise program data, finance metrics, risk updates, and strategic decisions while keeping the narrative aligned with our mission of [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (data consolidation, risk scoring, scenario assessment, decision log)
- decision_mode: plan -> execute -> verify, escalating uncertainty only once per section.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: assemble a concise fact base covering programs, finance, operations, risk, and strategy.
- Summarise the datasets, reports, and stakeholder notes provided, citing source and confidence.
- Flag conflicting numbers or gaps and note which owner can resolve them.
- Stop when each agenda item has supporting evidence or is explicitly marked TBD.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a heatmap of strategic priorities vs. performance (e.g., participation, revenue, safeguarding).
2. Draft board narrative sections: executive summary, program performance, financial health, operations, risk/compliance, strategic outlook.
3. Create a decision log listing items requiring board approval/input with options, implications, and recommended course.
4. Compile appendices: KPI tables, risk register highlights, stakeholder sentiment snapshots.
5. Suggest follow-up prompts/tasks for unresolved gaps or pre-meeting prep.
</WORKFLOW>

<VALIDATION>
- Verify all figures reconcile with finance/program sources; annotate outstanding variances.
- Ensure risks include status, mitigation owner, and review date.
- Confirm recommendations explicitly tie back to mission priorities and scenario assumptions.
</VALIDATION>

<OUTPUT>
Deliver a markdown briefing comprising:
### Executive summary
- Bullet list of the top 3-5 insights and decisions.

### Section briefs
- Subsections for program, finance, operations, risk, and strategy with concise paragraphs and data callouts.

### Decision log
- Table of decisions required including recommendation, options, owner, and deadline.

### Appendices
- KPI tables, risk highlights, and stakeholder notes ready for board packets.
</OUTPUT>
```

---
