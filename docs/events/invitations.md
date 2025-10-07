# Event invitations and confirmations

**Category:** Events  
**Template type:** Template filling and personalisation

**Collect these inputs before you start:**

- [NRL_CLUB/ORGANISATION_NAME]
- [EVENT_TYPE - e.g., season launch invitation, awards night confirmation, sponsor luncheon invite]
- [RECIPIENT_NAME]
- [EVENT_NAME]
- [EVENT_DATE]
- [EVENT_LOCATION]
- [EVENT_PURPOSE - e.g., celebrating volunteers, launching the season, thanking sponsors]
- [SPECIAL_STEPS - e.g., RSVP link, dress code, parking details]
- [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, strengthening community spirit]
- [INVITATION_TYPE - e.g., invitation, reminder, confirmation, or thank you]
- [AUDIENCE_SEGMENTS - e.g., sponsors, volunteers, families]
- [MISSION_STATEMENT]


Deliver personalised invites and confirmations that feel warm and mission-aligned. The low-complexity prompt covers quick customisation, while the medium-complexity workflow supports deeper tailoring by audience segment.

---

## Low complexity: Invitation prompt

```text
Act as an event communications specialist for [NRL_CLUB/ORGANISATION_NAME] and create a personalised [EVENT_TYPE - e.g., season launch invitation, awards night confirmation, sponsor luncheon invite] for [RECIPIENT_NAME] that includes key details about our [EVENT_NAME] on [EVENT_DATE] at [EVENT_LOCATION]. Maintain our club's warm and professional tone while highlighting the [EVENT_PURPOSE - e.g., celebrating volunteers, launching the season, thanking sponsors] and include any special instructions like [SPECIAL_STEPS - e.g., RSVP link, dress code, parking details].
```

---

## Medium complexity: Structured invitation workflow

```text
# NRL club event invitation and confirmation template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced community sport communications specialist who creates engaging, personalised event invitations and confirmation messages that drive attendance and participation for [NRL_CLUB/ORGANISATION_NAME]'s events while reflecting our mission of [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, strengthening community spirit].
</ROLE_AND_GOAL>

<STEPS>
Create a personalised [INVITATION_TYPE - e.g., invitation, reminder, confirmation, or thank you] for our upcoming [EVENT_NAME] on [EVENT_DATE] at [EVENT_LOCATION]. The message should:
1. Address the recipient by name and reference their relationship to the club (e.g., player, parent, volunteer, sponsor, community member).
2. Clearly communicate the event purpose, timing, location, and any special instructions (e.g., RSVP link, dress code, parking).
3. Include a compelling reason to attend that connects to our club's mission and community impact.
4. Specify any required actions (RSVP, registration, payment, etc.) with clear deadlines.
5. Match [NRL_CLUB/ORGANISATION_NAME]'s tone (e.g., warm, family-friendly, professional, celebratory) and incorporate our key messaging.
</STEPS>

<OUTPUT>
Provide the following:
1. **Email subject line** - compelling and specific
2. **Personalised greeting** - addressing the recipient by name
3. **Main message body** - 250-350 words, including event details and mission connection
4. **Clear call-to-action** - with deadline if applicable
5. **Professional closing** - with club representative's name and role (e.g., Club President, Events Coordinator)
</OUTPUT>
```

---

## High complexity: Audience-segmented invitation studio

Use this when you need tailored invitations, reminders, and confirmations across multiple attendee types with automation cues.

```text
# NRL event invitation orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Events Communications Manager for [NRL_CLUB/ORGANISATION_NAME], managing outreach for [EVENT_NAME] on [EVENT_DATE]. Deliver segmented invitations, confirmations, and reminders for [AUDIENCE_SEGMENTS - e.g., sponsors, volunteers, families], each reflecting [MISSION_STATEMENT] and specific value propositions.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 6 (audience profiling, message tailoring, automation mapping, accessibility review)
- output_bundle: invitation variants, reminder scripts, RSVP logic, escalation notes.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: collect attendee personas, event highlights, and logistical requirements.
- Summarise key agenda items, speakers, and unique experiences for each audience.
- Record special instructions (dress code, parking, accessibility accommodations).
- Stop when you can articulate personalised value and logistics for each segment or note follow-up gaps.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build persona cards for each audience segment with motivations, tone, and channels.
2. Draft invitation, reminder, and confirmation templates per persona, including dynamic fields and CTAs.
3. Provide SMS/WhatsApp short-form variants and phone script snippets for follow-up.
4. Outline automation logic (RSVP tracking, reminder cadence, escalation triggers for VIPs).
5. Compile post-event thank-you and survey prompts tailored to attendance outcome.
</WORKFLOW>

<VALIDATION>
- Ensure all messages include correct event details and deadlines.
- Confirm tone and benefits align with each persona's motivations.
- Check accessibility (plain language, alternative contact options) and add disclaimers as required.
</VALIDATION>

<OUTPUT>
Deliver a markdown communication kit featuring:
### Persona cards
- Profiles outlining motivations, tone, and preferred channels.

### Message templates
- Invitation, reminder, confirmation, and post-event notes for each segment.

### Short-form scripts
- SMS/WhatsApp copy and phone call talking points.

### Automation and escalation plan
- Flow description for triggers, reminders, and VIP handling.
</OUTPUT>
```

---
