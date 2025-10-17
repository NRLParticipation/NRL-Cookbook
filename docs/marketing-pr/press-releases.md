# Press releases and media announcements

**Category:** Marketing and PR  
**Template type:** Content generation from scratch

**Collect these inputs before you start:**

- [Rugby_League_Club/ORGANISATION_NAME]
- [ANNOUNCEMENT_TOPIC - e.g., new sponsor partnership, junior program launch, women's team expansion]
- [SPOKESPERSON_NAME/TITLE - e.g., Club President, Head Coach]
- [ANNOUNCEMENT_TYPE - e.g., new sponsorship, program launch, milestone achievement, community initiative]
- [SPOKESPERSON_NAME]
- [Rugby_League_Club_NAME]
- [CONTACT_NAME]
- [CONTACT_TITLE]
- [CONTACT_EMAIL]
- [CONTACT_PHONE]
- [ANNOUNCEMENT_TYPE]
- [ANNOUNCEMENT_DATE]
- [MISSION_STATEMENT]


Secure media coverage with professional, newsworthy announcements. The low-complexity prompt delivers a ready-to-send release, while the medium-complexity workflow supports more nuanced storytelling and media targeting.

---

## Low complexity: Press release prompt

```text
Act as a community sport PR specialist and create a compelling press release for [Rugby_League_Club/ORGANISATION_NAME] about [ANNOUNCEMENT_TOPIC - e.g., new sponsor partnership, junior program launch, women's team expansion]. Search the web for recent developments in grassroots rugby league and community sport to include relevant context, and structure it with a catchy headline, impactful quotes from [SPOKESPERSON_NAME/TITLE - e.g., Club President, Head Coach], key details about the announcement (who, what, when, where, why), and standard boilerplate information about the club's mission to grow rugby league and strengthen community spirit.
```

---

## Medium complexity: Structured press release workflow

```text
# NRL club press release generator template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced sport communications specialist who crafts compelling press releases and media announcements that generate positive coverage for rugby league organisations. Your task is to create a professional, newsworthy press release for [Rugby_League_Club/ORGANISATION_NAME] that effectively communicates their [ANNOUNCEMENT_TYPE - e.g., new sponsorship, program launch, milestone achievement, community initiative] while maintaining the club's authentic voice and mission focus.
</ROLE_AND_GOAL>

<STEPS>
1. Create a complete press release that includes: a strong headline, dateline, lead paragraph summarising the news, supporting paragraphs with details, quotes from [SPOKESPERSON_NAME] (with title, e.g., Club President, Head Coach), boilerplate about the club, and contact information.
2. Focus on the news angle that would most interest journalists covering community sport, rugby league, and local news.
3. Use the inverted pyramid structure with the most important information first.
4. Include at least two compelling quotes that balance factual detail with emotional impact, showing how the announcement strengthens rugby league and benefits the community.
5. Maintain a professional, third-person perspective throughout except in quotes.
</STEPS>

<OUTPUT>
Provide a complete, publication-ready press release with:
- **Attention-grabbing headline in bold**
- **Dateline** (City, State - Date)
- Four to five paragraphs of content (300-500 words total)
- Two or three quotes from club leadership or key spokespeople
- Standard "About [Rugby_League_Club_NAME]" boilerplate paragraph
- **Contact information section** with [CONTACT_NAME], [CONTACT_TITLE], [CONTACT_EMAIL], and [CONTACT_PHONE]
</OUTPUT>
```

---

## High complexity: Media campaign control room

Use this when the announcement requires multi-outlet targeting, asset coordination, and stakeholder follow-up.

```text
# NRL integrated press campaign template (high complexity)

<ROLE_AND_GOAL>
You are the Communications Director for [Rugby_League_Club/ORGANISATION_NAME], preparing a media campaign around [ANNOUNCEMENT_TYPE] on [ANNOUNCEMENT_DATE]. Produce a flagship press release, segmented media briefs, talking points, and follow-up plan that reinforce [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (story framing, media segmentation, quote crafting, risk review, follow-up planning)
- outreach_mode: generate assets for traditional media, digital outlets, and owned channels.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: capture announcement facts, stakeholder priorities, and media angles without redundant detail.
- Summarise the key facts, stats, and human-interest stories provided (cite sources).
- Identify target journalist segments and outlets with interests in community sport/rugby league.
- Stop when the core narrative arc and proof points are clear or gaps are documented.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Craft a narrative arc with headline themes, proof points, and emotional hooks.
2. Draft the main press release (headline, subhead, body, quotes, boilerplate, contact info).
3. Produce tailored media briefs (e.g., local news, sports, community) highlighting the most relevant angles.
4. Create talking points and Q and A for spokespeople, including suggested sound bites.
5. Outline distribution and follow-up plan with timeline, channel, owner, and success metrics.
</WORKFLOW>

<VALIDATION>
- Fact-check all stats and quotes; mark any needing approval.
- Ensure tone stays professional and mission-aligned across assets.
- Verify follow-up plan covers post-announcement amplification and monitoring.
</VALIDATION>

<OUTPUT>
Deliver a markdown media kit containing:
### Flagship press release
- Fully formatted release ready for distribution.

### Segmented media briefs
- Bullet summaries tailored to each outlet segment with suggested angles.

### Spokesperson toolkit
- Talking points, Q and A, and quote cards for spokespeople.

### Distribution and follow-up plan
- Timeline outlining channels, owners, metrics, and monitoring tasks.
</OUTPUT>
```

---
