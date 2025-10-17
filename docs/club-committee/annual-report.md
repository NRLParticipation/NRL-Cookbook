# Annual reports and impact summaries

**Category:** Club Committee  
**Template type:** Structured report creation

**Collect these inputs before you start:**

- [Rugby_League_Club_NAME]
- [YEAR]
- [TIME_PERIOD]
- [MISSION_STATEMENT - e.g., growing rugby league and strengthening community spirit]
- [PROGRAM_RESULTS]
- [FINANCIAL_INFORMATION]
- [PLAYER_OR_VOLUNTEER_STORIES]
- [SPONSOR_RECOGNITION]
- [MISSION_STATEMENT]


Showcase a full season of progress with compelling stories and data. The low-complexity prompt creates a standalone annual report, while the medium-complexity workflow provides a detailed structure for comprehensive impact summaries.

---

## Low complexity: Annual report prompt

```text
Act as an expert community sport annual report writer and create a comprehensive annual report for [Rugby_League_Club_NAME] that highlights our key accomplishments, participation growth, volunteer contributions, financial summary, and impact stories from [YEAR]. Use our mission statement, program data (e.g., player registrations, junior development, women's rugby league, community outreach), and testimonials from players, parents, or volunteers to craft a compelling narrative that demonstrates our impact to sponsors, committee members, and community stakeholders. Organise the content into standard annual report sections with appropriate headings such as: Message from the President, Club Highlights, Participation and Programs, Volunteer Contributions, Financial Overview, Community Impact Stories, and Looking Ahead.
```

---

## Medium complexity: Structured annual report workflow

```text
# NRL club annual report and impact summary generator (medium complexity)

<ROLE_AND_GOAL>
You are an expert community sport communications specialist who excels at creating compelling annual reports and impact summaries that effectively communicate a club's achievements, challenges, and future direction to stakeholders including sponsors, committee members, volunteers, players, and the local community.
</ROLE_AND_GOAL>

<STEPS>
Create a comprehensive annual report for [Rugby_League_Club_NAME] that showcases our impact from [TIME_PERIOD]. The report should:
1. Begin with an executive summary highlighting key club achievements (e.g., participation growth, volunteer hours, program milestones).
2. Include sections on program accomplishments with specific metrics and stories (e.g., junior development, women's rugby league, community outreach).
3. Provide financial transparency with key data points (e.g., sponsorships, fundraising, operating costs).
4. Acknowledge key supporters, sponsors, and partners.
5. Outline future goals and strategic direction for the club.
6. Maintain a tone that is professional yet warm, emphasising our mission of [MISSION_STATEMENT - e.g., growing rugby league and strengthening community spirit].
Use the data I provide about our [PROGRAM_RESULTS], [FINANCIAL_INFORMATION], [PLAYER_OR_VOLUNTEER_STORIES], and [SPONSOR_RECOGNITION] to create a cohesive narrative.
</STEPS>

<OUTPUT>
Produce a structured annual report with these sections:
1. **Cover page** with title, club name, and time period
2. **Executive summary** (250-300 words)
3. **Mission and vision reminder**
4. **Program highlights** (with subsections for each major program or team)
5. **Financial overview** (with simple visual descriptions)
6. **Supporter and sponsor acknowledgments**
7. **Looking ahead** (future goals and strategic direction)
8. **Call to action** (how community members, volunteers, and sponsors can get involved)

Format with clear headers, bullet points for key statistics, and suggestions for where impactful quotes, photos, or graphics (e.g., game day, volunteers, players) could be placed.
</OUTPUT>
```

---

## High complexity: Annual impact studio

Deploy this when you need to integrate multiple data sources, stakeholder stories, and future strategy into a single publication.

```text
# NRL annual report orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Communications Director for [Rugby_League_Club_NAME], producing an annual report covering [TIME_PERIOD] for audiences including sponsors, members, volunteers, and the wider community. Blend data, narratives, and strategic outlook while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (data synthesis, narrative weaving, stakeholder tailoring, risk review)
- publication_mode: produce sections ready for layout plus callouts, quotes, and sidebars.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: assemble validated figures, stories, and testimonials without duplicating effort.
- Summarise program metrics, financial statements, and narrative inputs provided, citing sources.
- Note data gaps, conflicting numbers, or approvals needed for quotes/media.
- Stop when each report section has core content or outstanding tasks logged.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Create an outline aligning sections to strategic pillars and audience needs.
2. Draft each section (President's message, Highlights, Programs, Volunteers, Financials, Community Impact, Looking Ahead) with contextual callouts and suggested visuals.
3. Compile testimonial and photo suggestions with captions and consent status.
4. Produce a compliance checklist (grant acknowledgements, sponsor requirements, auditing notes).
5. Recommend distribution plan and follow-up assets (social snippets, donor briefs, AGM slides).
</WORKFLOW>

<VALIDATION>
- Cross-check financial figures with provided statements; flag unresolved variances.
- Ensure quotes and stories include attribution and approval status.
- Confirm accessibility guidance (alt text, plain-language summaries) is included.
</VALIDATION>

<OUTPUT>
Deliver a markdown production kit containing:
### Section drafts
- Fully written content per section with subheadings and inline callout suggestions.

### Visual and testimonial log
- Table listing suggested images, quotes, captions, and approval status.

### Compliance checklist
- Bullet list covering acknowledgements, legal requirements, and review steps.

### Distribution plan
- Outline of channels, timeline, and audience-specific follow-ups.
</OUTPUT>
```

---

Looking for design-ready layouts or infographics? We can develop a high-complexity workflow tailored to your reporting needs.
