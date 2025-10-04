# Strategic planning and scenario planning

**Category:** Administrators  
**Template type:** Strategic planning and forecasting

**Collect these inputs before you start:**

- [NRL_CLUB/ORGANISATION_NAME]
- [COMMUNITY_SPORT_FOCUS - e.g., rugby league participation, women and girls in sport, volunteerism, grassroots funding]
- [CLUB_METRICS/CHALLENGES - e.g., registrations and retention, volunteer hours/roles, sponsorship revenue, facilities capacity, compliance/safeguarding, game-day attendance]
- [MISSION_STATEMENT]
- [PLANNING_TIMEFRAME]


Develop long-range plans grounded in community rugby league realities. The low-complexity prompt guides a full three-year strategy with scenarios, while the medium-complexity workflow provides a structured framework for deeper analysis.

---

## Low complexity: Three-Year Plan With Scenarios

```text
Act as a community sport strategic planning consultant for [NRL_CLUB/ORGANISATION_NAME] and help develop a three-year strategic plan with scenario planning. Search the web for current trends in [COMMUNITY_SPORT_FOCUS - e.g., rugby league participation, women and girls in sport, volunteerism, grassroots funding], analyse our current state data including [CLUB_METRICS/CHALLENGES - e.g., registrations and retention, volunteer hours/roles, sponsorship revenue, facilities capacity, compliance/safeguarding, game-day attendance], and create three future scenarios (optimistic, realistic, pessimistic) with corresponding strategic recommendations, resource requirements (budget ranges, volunteer/FTE equivalents, partnerships, facilities), and impact measurements/KPIs (e.g., participation growth, volunteer retention, inclusion targets, financial sustainability). Deliver: (1) Executive summary, (2) Current state snapshot (baseline metrics), (3) Trends summary (implications for the club), (4) Scenario matrix (assumptions, priorities, initiatives, resources, KPIs), (5) Year-by-year roadmap with milestones, (6) Risks and mitigations by scenario, and (7) Measurement and reporting cadence (dashboard metrics and review rhythm). Align advice with safeguarding expectations and community sport best practice, using clear, actionable language suitable for committee decision-making.
```

---

## Medium complexity: Structured Strategic Planning Workflow

```text
# NRL strategic planning and scenario development template (medium complexity)

<ROLE_AND_GOAL>
You are a community sport strategic planning consultant with expertise in scenario planning and long-term club development. Your task is to help [NRL_CLUB/ORGANISATION_NAME] develop a comprehensive strategic plan and scenario analysis that aligns with our mission of [MISSION_STATEMENT] while addressing current challenges (e.g., volunteer capacity, facilities, compliance) and future opportunities (e.g., participation growth, women and girls pathways, sponsorship).
</ROLE_AND_GOAL>

<STEPS>
Analyse the provided information and develop a strategic plan with scenario planning by:
1. Analysing [NRL_CLUB/ORGANISATION_NAME]'s current state, including strengths, weaknesses, opportunities, and threats (SWOT) across participation, volunteers, finance/sponsorship, facilities, and governance/safeguarding.
2. Identifying 3-5 strategic priorities based on [PLANNING_TIMEFRAME] (typically 3-5 years) that advance community impact and on-field pathways.
3. Developing three distinct future scenarios (optimistic, realistic, and challenging) with clear assumptions relevant to community rugby league.
4. Creating actionable recommendations for each strategic priority (initiatives, resources, partners, timing).
5. Suggesting key performance indicators to track progress (e.g., registrations, volunteer retention, inclusion targets, sponsorship revenue, game-day attendance).
</STEPS>

<OUTPUT>
Provide a strategic planning document with:
1. Executive summary (3-5 bullet points)
2. Current state analysis (SWOT)
3. Strategic priorities (3-5)
4. Future scenarios (Optimistic, Realistic, Challenging)
5. Implementation recommendations
6. Key performance indicators
7. Next steps
</OUTPUT>
```

---

## High complexity: Scenario Planning Command Suite

Use this when you need GPT-5 to orchestrate multi-scenario modelling, stakeholder heatmaps, and implementation governance.

```text
# NRL strategic foresight automation (high complexity)

<ROLE_AND_GOAL>
You are the Strategic Planning Director for [NRL_CLUB/ORGANISATION_NAME]. Build a five-year strategy incorporating scenario modelling (optimistic, realistic, challenging), resource planning, and stakeholder alignment aligned with [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 9 (trend scanning, data triangulation, scenario stress-testing, KPI design, risk mapping)
- foresight_mode: allow uncertainty but document assumptions and confidence levels.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: assemble evidence for participation, finance, volunteerism, facilities, and compliance trends.
- Summarise internal metrics, league benchmarks, and community insights provided.
- Identify emerging trends (limit to two quick scans if external context is required) and note uncertainty.
- Stop once every strategic pillar has baseline data and at least one future signal or is marked as gap.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a strategic insights brief (SWOT + trend impact assessment) per pillar.
2. Define scenario narratives with triggers, leading indicators, resource implications, and decision guardrails.
3. Create priority portfolio: objectives, initiatives, owners, dependencies, and budget ranges.
4. Develop KPI architecture (lagging/leading metrics, targets, data sources, review cadence).
5. Generate stakeholder engagement map (influence, interest, messaging, cadence) and risk mitigation plan.
</WORKFLOW>

<VALIDATION>
- Check coherence between scenarios and initiative portfolio; highlight conflicts or overcommitments.
- Ensure resource projections align with financial constraints; mark funding gaps.
- Confirm KPIs are measurable with existing data systems or list required upgrades.
</VALIDATION>

<OUTPUT>
Deliver a markdown strategy dossier containing:
### Strategic insights
- Key findings per pillar with confidence scores.

### Scenario playbook
- Descriptions of each scenario including triggers, indicators, and implications.

### Initiative portfolio
- Table of initiatives with priority, cost band, owner, and timeline.

### KPI framework
- Metrics with calculation method, targets, frequency, and data owner.

### Stakeholder plan
- Map of stakeholder segments alongside engagement tactics and narrative focus.
</OUTPUT>
```

---
