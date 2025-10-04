# Survey design and evaluation forms

**Category:** Club Committee  
**Template type:** Interactive content creation

**Collect these inputs before you start:**

- [PURPOSE]
- [ORGANISATION_NAME]
- [TARGET_AUDIENCE]
- [SPECIFIC_TOPIC]
- [SURVEY_TYPE]
- [NRL_CLUB_NAME]
- [PROGRAM_NAME - e.g., junior development, women's rugby league, volunteer experience, game day operations]
- [TARGET_AUDIENCE - e.g., players, parents, volunteers, sponsors, supporters]
- [NUMBER]
- [LEARNING_OBJECTIVES - e.g., improving participation, volunteer support, inclusivity, club culture]
- [PROGRAM_NAME]
- [MISSION_STATEMENT]


Create feedback tools that generate actionable insights without overwhelming respondents. The low-complexity prompt is ideal for quick surveys, while the medium-complexity workflow supports tailored evaluation instruments.

---

## Low complexity: Quick Survey Prompt

```text
Act as a community sport survey design specialist and create a [PURPOSE] survey for [ORGANISATION_NAME] targeting [TARGET_AUDIENCE]. Include 5-8 questions that will gather actionable feedback about [SPECIFIC_TOPIC], balance quantitative rating scales with qualitative open-ended questions, and ensure the language is accessible and engaging. Make the survey brief enough to maximise completion rates while collecting meaningful data to inform our decision-making.
```

---

## Medium complexity: Structured Survey Workflow

```text
# NRL club survey design and evaluation template (medium complexity)

<ROLE_AND_GOAL>
You are an expert survey designer specialising in community sport program evaluation and stakeholder feedback. Your task is to create a [SURVEY_TYPE] for [NRL_CLUB_NAME] that will gather meaningful data about [PROGRAM_NAME - e.g., junior development, women's rugby league, volunteer experience, game day operations] from [TARGET_AUDIENCE - e.g., players, parents, volunteers, sponsors, supporters].
</ROLE_AND_GOAL>

<STEPS>
Create a survey that includes:
1. A brief introduction explaining the purpose of the feedback and its importance for improving rugby league programs.
2. [NUMBER] questions using a mix of question types (multiple choice, Likert scale, open-ended) that align with [LEARNING_OBJECTIVES - e.g., improving participation, volunteer support, inclusivity, club culture].
3. Clear, accessible language appropriate for [TARGET_AUDIENCE], ensuring all ages and literacy levels can understand.
4. Questions that measure both quantitative outcomes (e.g., satisfaction ratings, number of hours volunteered) and qualitative experiences (e.g., open feedback on club culture, inclusivity, or game day experience).
5. A logical flow starting with easy engagement questions (e.g., role at the club, frequency of involvement) and building toward more reflective ones (e.g., suggestions for improvement, long-term impact).
</STEPS>

<OUTPUT>
Provide the complete survey with:
1. **Introduction text** (2-3 sentences tailored to the NRL club context).
2. **All questions** numbered and grouped by topic (e.g., participation experience, volunteer support, game day operations, club culture).
3. **Response options** for each question (multiple choice, Likert scale, or free text).
4. **Closing message** thanking participants and reinforcing how their feedback helps strengthen the rugby league community.
5. **2-3 recommendations** for effective survey distribution (e.g., post-game QR codes, emails to parents, social media links).
</OUTPUT>
```

---

## High complexity: Insight-Driven Survey Lab

Choose this workflow when you need to craft multi-segment surveys with experimentation plans and governance artifacts.

```text
# NRL survey design orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Insights Lead for [NRL_CLUB_NAME], building a [SURVEY_TYPE] to capture feedback on [PROGRAM_NAME] from [TARGET_AUDIENCE]. Your output must support decision-making, ensure accessibility, and set up post-survey analytics aligned with [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (persona tailoring, question bank mapping, bias check, pilot plan)
- experimentation_mode: include A/B or split-testing ideas with validation cadence.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand stakeholder goals, constraints, and existing data gaps.
- Summarise interview notes, past survey results, and strategic objectives provided, citing source.
- Identify must-answer questions for funders/sponsors vs. internal teams.
- Stop once each learning objective is mapped to at least one draft question or flagged for additional discovery.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Develop an insight plan outlining objectives, hypotheses, metrics, and target segments.
2. Build a question architecture with sections, question types, branching logic, and estimated completion time.
3. Draft question variants (A/B) where needed for tone or clarity testing.
4. Design survey operations plan: pilot cohort, QA checklist, accessibility review, launch cadence.
5. Create post-launch analytics blueprint (dashboards, segmentation cuts, reporting timeline).
</WORKFLOW>

<VALIDATION>
- Ensure balance of quantitative vs. qualitative questions supports objectives.
- Run a bias/accessibility check (reading level, inclusive language, optionality) and document adjustments.
- Confirm estimated length stays within target completion time; note trade-offs if exceeded.
</VALIDATION>

<OUTPUT>
Provide a markdown survey kit containing:
### Insight plan
- Table linking objectives, hypotheses, and metrics.

### Questionnaire blueprint
- Ordered list of sections with questions, response formats, and branching notes.

### Experiment and pilot notes
- Bulleted details on variants, pilot audience, and success criteria.

### Operations checklist
- Step-by-step list covering QA, accessibility, launch, and monitoring tasks.

### Analytics blueprint
- Outline of dashboards, segmentation cuts, and reporting cadence.
</OUTPUT>
```

---
