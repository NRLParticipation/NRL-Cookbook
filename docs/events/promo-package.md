# Event promotional materials

**Category:** Events  
**Template type:** Content generation from scratch

**Collect these inputs before you start:**

- [EVENT_NAME]
- [NRL_CLUB/ORGANISATION_NAME]
- [EVENT_DATE]
- [TARGET_AUDIENCE - e.g., families, players, sponsors, local community]
- [EVENT_DATE_TIME]
- [EVENT_LOCATION]
- [EVENT_PURPOSE - e.g., season launch, junior registrations, sponsor day, fundraiser]
- [TARGET_AUDIENCE]
- [KEY_ACTIVITIES - e.g., games, clinics, awards, guest speakers]
- [REGISTRATION_DETAILS]
- [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, strengthening community spirit]
- [Headline]
- [Tagline 1]
- [Tagline 2]
- [Tagline 3]
- [Benefit/Feature 1]
- [Benefit/Feature 2]
- [Benefit/Feature 3]
- [Benefit/Feature 4]
- [Benefit/Feature 5]
- [Additional features as needed]
- [Facebook post with event details and emotional appeal]
- [Instagram post with visual description elements and hashtags]
- [Concise Twitter post with essential details and hashtags]
- [Compelling CTA with registration information]
- [EVENT_PURPOSE]
- [MISSION_STATEMENT]


Launch events with cohesive messaging across channels. The low-complexity prompt produces a full promotional bundle, while the medium-complexity workflow structures targeted content for multiple platforms.

---

## Low complexity: Promotional package prompt

```text
Act as a community sport event marketing specialist and create compelling promotional materials for [EVENT_NAME] hosted by [NRL_CLUB/ORGANISATION_NAME] on [EVENT_DATE]. Search the web for effective community sport and grassroots rugby league event promotion strategies and generate a complete promotional package including: a press release, five social media posts with relevant rugby league hashtags, an email announcement, and a one-page event flyer - all maintaining our club's authentic voice while emphasising our mission impact (e.g., growing participation, celebrating volunteers, strengthening community spirit) and clear calls to action (e.g., register, attend, support).
```

---

## Medium complexity: Structured promotional workflow

```text
# NRL club event promotional materials template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced community sport event marketing specialist who creates compelling promotional materials that drive attendance and engagement while reflecting club values. Your task is to generate promotional content for [EVENT_NAME] hosted by [NRL_CLUB/ORGANISATION_NAME] that will resonate with [TARGET_AUDIENCE - e.g., families, players, sponsors, local community] and effectively communicate the event's purpose, benefits, and key details.
</ROLE_AND_GOAL>

<STEPS>
Create a comprehensive promotional package for the event that includes:
1. A compelling event headline and two or three taglines that capture the essence of the event.
2. A 150-200 word event description for the website and email announcements.
3. Five to seven key bullet points highlighting event benefits or features.
4. Three social media posts (50-75 words each) tailored for different platforms.
5. A call-to-action statement encouraging registration or attendance.

Use the following information to customise the content:
- Event name: [EVENT_NAME]
- Date and time: [EVENT_DATE_TIME]
- Location: [EVENT_LOCATION]
- Purpose: [EVENT_PURPOSE - e.g., season launch, junior registrations, sponsor day, fundraiser]
- Target audience: [TARGET_AUDIENCE]
- Key speakers/activities: [KEY_ACTIVITIES - e.g., games, clinics, awards, guest speakers]
- Registration information: [REGISTRATION_DETAILS]
- Club mission: [NRL_CLUB/ORGANISATION_NAME]'s mission of [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, strengthening community spirit].
</STEPS>

<OUTPUT>
## Event headline and taglines
[Headline]
- [Tagline 1]
- [Tagline 2]
- [Tagline 3]

Event description
[150-200 word compelling description]

Key event highlights
- [Benefit/Feature 1]
- [Benefit/Feature 2]
- [Benefit/Feature 3]
- [Benefit/Feature 4]
- [Benefit/Feature 5]
- [Additional features as needed]

Social media posts
Facebook:
[Facebook post with event details and emotional appeal]

Instagram:
[Instagram post with visual description elements and hashtags]

Twitter/X:
[Concise Twitter post with essential details and hashtags]

Call-to-action
[Compelling CTA with registration information]
</OUTPUT>
```

---

## High complexity: Multi-channel event launch studio

Use this when you require a strategic event campaign across owned, earned, and paid channels with experimentation hooks and measurement plans.

```text
# NRL event campaign orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Event Marketing Director for [NRL_CLUB/ORGANISATION_NAME], launching [EVENT_NAME] on [EVENT_DATE_TIME] at [EVENT_LOCATION]. Create a full-funnel campaign to engage [TARGET_AUDIENCE], emphasise [EVENT_PURPOSE], and reinforce [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (audience segmentation, channel playbooks, asset prompts, experimentation, KPI planning)
- campaign_span: pre-event buzz, conversion push, last-call, onsite amplification, post-event recap.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand audience segments, key activities, stakeholder expectations, and past performance.
- Summarise event highlights, speakers, and partner requirements provided.
- Note previous campaign learnings (open rates, attendance drivers, social reach).
- Stop when each campaign stage has clear objectives and content pillars or list gaps.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build a strategy canvas with audience segments, motivations, and key messages.
2. Develop channel playbooks (email, social, PR, paid, website, SMS) detailing cadence, creative angle, and CTA.
3. Produce content assets: long-form narrative, talking points, social copy, ad headlines, SMS prompts, press sound bites.
4. Outline experimentation plan (e.g., subject line tests, creative variants) with metrics and decision rules.
5. Define measurement framework (KPIs, dashboards, reporting cadence) and post-event amplification steps.
</WORKFLOW>

<VALIDATION>
- Ensure all materials accurately reflect event details and logistics.
- Confirm CTAs, ticketing links, and tracking parameters are consistent across channels.
- Check accessibility: alt-text guidance, caption suggestions, inclusive language.
</VALIDATION>

<OUTPUT>
Deliver a markdown campaign dossier containing:
### Strategy canvas
- Table summarising segments, needs, and messaging focus.

### Channel playbooks
- Sections for each channel with objectives, cadence, content angles, and CTAs.

### Content library
- Ready-to-use copy blocks (email, social, SMS, press) with placeholders.

### Experiment plan
- List of tests with hypotheses, measurement plans, and success thresholds.

### Measurement and amplification plan
- KPIs, dashboard notes, reporting cadence, and post-event content suggestions.
</OUTPUT>
```

---
