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
Act as an expert community sport annual report writer and create a comprehensive public annual report for [Picton] that highlights our key accomplishments, participation growth, volunteer contributions, financial summary, and impact stories from [2025]. Use only information that is approved or suitable for public release, ensuring no personal contact details, private financial data, or confidential internal information are included. Draw from our public mission statement, program summaries (e.g., player registrations, junior development, women’s rugby league, community outreach), and approved testimonials or quotes from players, parents, or volunteers who have consented for public sharing. Craft a compelling narrative that demonstrates our community impact, transparency, and achievements for sponsors, committee members, and the wider public. Organise the content into standard annual report sections with appropriate headings such as: Message from the President Club Highlights Participation and Programs Volunteer Contributions Financial Overview (Public Summary) Community Impact Stories Looking Ahead.
```

---

## Medium complexity: Structured annual report workflow

```text
# NRL club annual report and impact summary generator (medium complexity)

<ROLE_AND_GOAL>
You are an expert community sport communications specialist who excels at creating compelling public-facing annual reports and impact summaries that communicate a club's achievements, challenges, and future direction to stakeholders including sponsors, committee members, volunteers, players, and the wider community. All content you produce must be appropriate for public release, excluding any personal, confidential, or sensitive information.
</ROLE_AND_GOAL>

<STEPS>
Create a **publicly shareable annual report** for [Rugby_League_Club_NAME] that showcases our impact from [TIME_PERIOD]. The report should:
1. Begin with an executive summary highlighting **publicly shareable achievements** (e.g., participation growth, volunteer hours, program milestones).
2. Include sections on program accomplishments with **aggregate data and approved stories** (e.g., junior development, women’s rugby league, community outreach).
3. Provide **financial transparency** through summarised key figures (e.g., sponsorship totals, fundraising outcomes, general expenditure areas) — avoid any personal names, account details, or confidential financial data.
4. Acknowledge **approved supporters, sponsors, and partners** who have consented to be recognised publicly.
5. Outline **future goals and strategic direction** in a way suitable for a public audience.
6. Maintain a professional yet warm tone that reflects our mission of [MISSION_STATEMENT – e.g., growing rugby league and strengthening community spirit].
Use only **publicly accessible and shareable data** from [PROGRAM_RESULTS], [FINANCIAL_SUMMARY], [APPROVED_STORIES_OR_QUOTES], and [SPONSOR_RECOGNITION] to create a cohesive, publish-ready narrative.
</STEPS>

<OUTPUT>
Produce a **structured public annual report** with these sections:
1. **Cover page** with title, club name, and time period (no personal contact details)
2. **Executive summary** (250–300 words)
3. **Mission and vision reminder**
4. **Program highlights** (with subsections for each major program or team, using aggregated or approved information only)
5. **Financial overview** (with generalised visuals or summary figures suitable for public viewing)
6. **Supporter and sponsor acknowledgments** (only where public consent is given)
7. **Looking ahead** (future goals and strategic direction)
8. **Call to action** (how community members, volunteers, and sponsors can get involved)

Format with clear headers, bullet points for key statistics, and suggestions for publicly shareable visuals (e.g., community events, volunteer photos, player celebrations). Ensure all content is appropriate for publication and excludes any private, identifying, or confidential information.
</OUTPUT>
```
