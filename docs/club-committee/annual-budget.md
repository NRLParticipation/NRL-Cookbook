# Annual club budget planner

**Category:** Club Committee  
**Template type:** Financial planning and governance

**Collect these inputs before you start:**

- [NRL_CLUB/ORGANISATION_NAME]
- [FINANCIAL_YEAR]
- [REVENUE_SOURCES]
- [EXPENSE_CATEGORIES]
- [MISSION_STATEMENT]


Use these prompts to prepare an annual rugby league club budget that balances participation goals with financial sustainability.

---

## Low complexity: Quick Budget Outline Prompt

Use this when you need a fast draft for committee review.

```text
Act as a community sport finance advisor. Build an annual budget outline for [NRL_CLUB/ORGANISATION_NAME] covering [FINANCIAL_YEAR]. Use the following revenue streams: [REVENUE_SOURCES], and expenses: [EXPENSE_CATEGORIES]. Provide:
- Summary table of projected income versus expenditure
- Notes on cashflow pinch points across the season
- Two cost-saving or fundraising ideas aligned with club culture
Keep figures in Australian dollars and highlight any assumptions.
```

---

## Medium complexity: Structured Annual Budget Workflow

Pick this template when you have detailed inputs and want a committee-ready workbook.

```text
# Annual club budget template (medium complexity)

<ROLE_AND_GOAL>
You are the Treasurer for [NRL_CLUB/ORGANISATION_NAME]. Develop a detailed budget for [FINANCIAL_YEAR] that supports participation growth, complies with governance obligations, and maintains cash reserves.
</ROLE_AND_GOAL>

<INPUT>
I will provide:
- Last year's actuals (revenue and expenses)
- Projected participation numbers or program changes
- Planned capital projects or major events
- Funding commitments (grants, sponsorships) with timing
- Cost drivers (venue hire, equipment, travel, insurance)
</INPUT>

<STEPS>
1. Summarise baseline assumptions and variances versus last year.
2. Build income projections by stream (registrations, sponsorship, fundraising, grants, canteen, merchandise).
3. Itemise expenditure by program and operations (coaching, referees, travel, facilities, administration, marketing).
4. Identify seasonal cashflow peaks and troughs, suggesting buffer levels or short-term financing if needed.
5. Recommend allocation of surplus (reserves, facility upgrades, contingency funds) and risk mitigation plans.
6. Prepare commentary for committee presentation, including key changes, risks, and decision points.
</STEPS>

<CONSTRAINTS>
- Use Australian dollars and note GST assumptions if relevant.
- Flag any figures requiring confirmation or quotes.
- Align recommendations with club policies and safeguarding commitments.
</CONSTRAINTS>

<OUTPUT>
- Budget summary table (income, expense, net position)
- Month-by-month cashflow projection
- Narrative commentary highlighting drivers and risks
- Action list for approvals, grant applications, or cost reviews
</OUTPUT>
```

---

## High complexity: Financial Strategy Orchestrator

Deploy this workflow when you need multi-scenario forecasts, sensitivity testing, and governance artefacts.

```text
# Comprehensive club budgeting template (high complexity)

<ROLE_AND_GOAL>
You are the Chief Financial Steward for [NRL_CLUB/ORGANISATION_NAME], preparing a three-year financial strategy centred on [MISSION_STATEMENT]. Deliver a compliant budget pack that supports strategic initiatives, risk management, and stakeholder transparency.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (scenario modelling, sensitivity analysis, risk scanning)
- decision_mode: baseline -> scenario -> recommendation
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: gather the financial and strategic data required for robust forecasting.
- Compile historical financials, participation trends, grant cycles, sponsorship agreements, and facility commitments.
- Capture strategic priorities (pathway expansion, women and girls programs, facility upgrades, community outreach).
- Note compliance requirements (audits, NRL reporting, insurance, safeguarding budgets).
- Record risk factors (volunteer capacity, weather impacts, cost escalation) and available contingencies.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build baseline projections for revenue and expenditure using historical averages adjusted for confirmed changes.
2. Create at least three scenarios (optimistic, expected, conservative) covering participation, sponsorship, and grant outcomes.
3. Run sensitivity checks on major cost drivers (venue hire, travel, insurance) and revenue dependencies.
4. Develop funding and investment recommendations (reserve targets, capital projects, grant priorities) aligned with strategic goals.
5. Produce governance artefacts: budget summary, scenario comparison charts, risk register, and board briefing notes.
6. Outline implementation steps, including monitoring cadence, trigger alerts for reforecasting, and stakeholder communication plan.

<VALIDATION>
- Confirm assumptions with provided data or flag for follow up.
- Ensure each scenario meets safeguarding, compliance, and reserve policies.
- Highlight exposure areas requiring mitigation or contingency planning.

<OUTPUT>
Deliver a financial strategy pack containing:
### Budget overview
- Tables summarising baseline and scenario projections with variances.

### Scenario dashboard
- Charts comparing revenue, expenditure, and cash position under each scenario.

### Risk and mitigation register
- List of financial risks, likelihood, impact, owner, and mitigation actions.

### Implementation roadmap
- Timeline for approvals, reporting, and reforecast checkpoints.
```

---
