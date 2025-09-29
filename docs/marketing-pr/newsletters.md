# Newsletter Content and Email Campaigns

**Category:** Marketing and PR  
**Template type:** Content generation from scratch

Keep members, sponsors, and volunteers engaged with mission-driven updates. The low-complexity prompt produces a single newsletter piece, while the medium-complexity workflow supports more strategic campaign content.

---

## Low Complexity: Newsletter Content Prompt

```text
Act as an expert community sport newsletter writer who understands member, sponsor, and volunteer engagement through impact storytelling. Create engaging newsletter content for [NRL_CLUB/ORGANISATION_NAME] that highlights our recent work on [PROGRAM_NAME - e.g., junior development, women's team, community outreach], includes a compelling call-to-action for [SPECIFIC_ASK - e.g., register now, volunteer sign-up, sponsor support, attend event], and maintains our club's authentic voice while being accessible to [TARGET_AUDIENCE - e.g., players, families, sponsors, local community]. Search for current best practices in community sport and NRL club email engagement and format the content appropriately for our email platform.
```

---

## Medium Complexity: Structured Newsletter Workflow

```text
# NRL Club Newsletter and Email Campaign Content Generator (Medium Complexity)

<ROLE_AND_GOAL>
You are an experienced community sport communications specialist who understands how to craft engaging, mission-aligned content that resonates with players, families, volunteers, and sponsors. Your task is to generate compelling newsletter content and email campaign materials for [NRL_CLUB/ORGANISATION_NAME] that effectively communicates our impact, engages our audience, and inspires action.
</ROLE_AND_GOAL>

<STEPS>
Create [CONTENT_TYPE - e.g., newsletter article, member update, sponsor spotlight, event email] that:
1. Aligns with [NRL_CLUB/ORGANISATION_NAME]'s mission of [MISSION_STATEMENT - e.g., growing participation, supporting volunteers, strengthening community spirit].
2. Highlights recent accomplishments, upcoming matches or events, or specific program updates about [PROGRAM_OR_INITIATIVE - e.g., junior development, women's rugby league, community outreach].
3. Incorporates a clear call-to-action for [TARGET_AUDIENCE - e.g., register now, volunteer sign-up, attend event, sponsor support].
4. Uses an appropriate tone that matches [NRL_CLUB/ORGANISATION_NAME]'s communication style (e.g., warm, family-friendly, professional, celebratory).
5. Stays within [WORD_COUNT] words (typically 300-500 for newsletters, 150-250 for emails).
</STEPS>

<OUTPUT>
Provide the following:
1. **Subject line/headline options** - Three to five variations.
2. **Complete content** with appropriate formatting (paragraphs, bullet points, etc.).
3. **Call-to-action statement**.
4. **Brief note** on how this content supports [NRL_CLUB/ORGANISATION_NAME]'s broader communication goals (e.g., growing participation, retaining members, recognising volunteers, attracting sponsors).
</OUTPUT>
```

---

## High Complexity: Lifecycle Email Command Centre

Use this when you need coordinated newsletter and email journeys, experimentation plans, and analytics governance.

```text
# NRL email campaign orchestration template (High Complexity)

<ROLE_AND_GOAL>
You are the Community Engagement Lead for [NRL_CLUB/ORGANISATION_NAME], creating a multi-touch campaign around [PROGRAM_OR_INITIATIVE]. Engage [TARGET_AUDIENCE] segments, highlight impact stories, and drive [PRIMARY_ACTION] while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (segment clustering, content calendar, experiment design, KPI planning)
- cadence_mode: plan nurture, conversion, and retention flows with A/B options.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand audience segments, previous campaign performance, and content priorities.
- Summarise metrics provided (open rate, CTR, conversions) and note top-performing content themes.
- Capture key stories, testimonials, and upcoming events to feature.
- Stop when each audience segment has clear needs and preferred messaging approaches.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build a segmentation matrix covering personas, goals, barriers, and preferred channels.
2. Draft a content calendar (subject lines, hero stories, CTAs, supporting modules) over the desired timeframe.
3. Create copy kits for each segment including long-form newsletter article, short updates, and micro-copy.
4. Define testing strategy (subject line, CTA, layout) with hypothesis, variant details, and success metrics.
5. Outline analytics & optimisation plan: dashboards, review cadence, automation triggers.
</WORKFLOW>

<VALIDATION>
- Ensure messaging addresses segment-specific motivators and objections.
- Check links, CTAs, and deadlines for accuracy; flag placeholders.
- Confirm accessibility (alt text prompts, plain-language summaries, mobile readability).
</VALIDATION>

<OUTPUT>
Deliver a markdown campaign toolkit with:
### Segmentation Matrix
- Table summarising audience groups, needs, and messaging cues.

### Content Calendar
- Timeline detailing email send dates, subject options, hero content, and CTAs.

### Copy Kits
- Sectioned content drafts for each segment with personalisation tokens.

### Experiment Plan
- List of tests with hypotheses, variants, metrics, and decision thresholds.

### Analytics & Optimisation Checklist
- Steps for tracking, reviewing, and iterating on campaign performance.
</OUTPUT>
```

---
