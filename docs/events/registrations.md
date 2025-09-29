# Event Registrations and Follow-ups

**Category:** Events  
**Template type:** Automated communications

Keep attendees informed from sign-up to post-event. The low-complexity prompt generates a full email series, while the medium-complexity workflow offers customisable templates with timing guidance.

---

## Low Complexity: Registration Follow-up Prompt

```text
Act as an event communications coordinator for [NRL_CLUB/ORGANISATION_NAME] and generate a set of follow-up emails for our [EVENT_NAME] on [EVENT_DATE], including: a registration confirmation, a one-week reminder with event details, a day-before reminder with last-minute instructions, and a post-event thank you message that requests feedback. Use a warm, welcoming tone that reflects our mission of [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, building community spirit], and include our club logo and contact information in each message.
```

---

## Medium Complexity: Structured Registration Workflow

```text
# NRL Club Event Registration Follow-up and Confirmation Template (Medium Complexity)

<ROLE_AND_GOAL>
You are an experienced Event Coordinator for [NRL_CLUB/ORGANISATION_NAME], responsible for managing all communication with registrants for our [EVENT_NAME]. Your task is to create personalised, timely follow-up messages and confirmations that maintain engagement, provide necessary information, and reduce no-shows.
</ROLE_AND_GOAL>

<STEPS>
Generate a complete set of event communication templates based on the following information:
1. Create a **confirmation email** to be sent immediately after registration.
2. Design a **reminder email** for [REMINDER_TIMEFRAME] before the event.
3. Develop a **final details email** for [FINAL_DETAILS_TIMEFRAME] before the event.
4. Create a **post-event thank you email** with [FOLLOW_UP_ACTION - e.g., feedback survey, membership renewal, volunteer sign-up] request.

For each template:
- Include a clear, engaging subject line.
- Personalise with [ATTENDEE_NAME] and specific event details.
- Incorporate [NRL_CLUB/ORGANISATION_NAME] branding elements and tone (e.g., warm, community-focused, professional).
- Include all critical information ([EVENT_LOCATION], [EVENT_DATE], [EVENT_TIME]).
- Add any special instructions ([PARKING_INFO], [WHAT_TO_BRING], [DRESS_CODE]).
- Include contact information for questions ([CONTACT_NAME], [CONTACT_EMAIL], [CONTACT_PHONE]).
</STEPS>

<OUTPUT>
For each communication template, provide:
1. **Subject line** - Brief, clear subject line.
2. **Email body** - Complete email text with all placeholders properly positioned.
3. **Send timing** - Recommended timing for sending this communication.
4. **Customisation notes** - Brief notes on how to adapt this template for different event types (e.g., game days, awards nights, fundraisers, sponsor luncheons).
</OUTPUT>
```

---

## High Complexity: Registration Engagement Control Tower

Deploy this when handling multi-stage communications, segmentation, and analytics for event registrants.

```text
# NRL registration lifecycle orchestration template (High Complexity)

<ROLE_AND_GOAL>
You are the Registration Experience Lead for [NRL_CLUB/ORGANISATION_NAME], managing communications for [EVENT_NAME] on [EVENT_DATE]. Deliver personalised confirmation, reminder, final details, and post-event follow-up sequences that reflect [MISSION_STATEMENT] and drive [FOLLOW_UP_ACTION].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (audience segmentation, copy variants, automation design, analytics planning, accessibility QA)
- cadence_scope: confirmation, T-1 week, T-24 hours, on-the-day, post-event.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: gather registrant personas, event logistics, and compliance requirements.
- Summarise registration form fields, ticket types, and special accommodations.
- Note key event highlights, partners, and post-event objectives (e.g., membership sign-up, feedback).
- Stop when each communication touchpoint has clear objectives or gaps are noted for follow-up.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Segment registrants (e.g., VIP, general attendee, volunteer) with tailored messaging cues.
2. Draft templates for confirmation, pre-event reminders, final instructions, and post-event thank-you/feedback requests (email + SMS microcopy).
3. Create automation flow outlining triggers, timing, fallback channels, and escalation paths.
4. Provide personalisation tokens, merge tags, and dynamic content blocks for logistics (parking, accessibility, weather contingencies).
5. Outline analytics dashboard metrics (open/click rates, attendance conversion, feedback response) and follow-up prompt suggestions.
</WORKFLOW>

<VALIDATION>
- Verify all logistical details (time zones, venue, contact info) are accurate across templates.
- Ensure tone and CTAs align with mission and audience expectations.
- Confirm accessibility steps (plain language, alternative formats, contact options) are included.
</VALIDATION>

<OUTPUT>
Produce a markdown communications playbook with:
### Segment Overview
- Table or list describing each audience group with key messaging notes.

### Message Templates
- Full email content and SMS snippets for each touchpoint and segment.

### Automation Blueprint
- Flow diagram or ordered steps detailing triggers, timing, and fallback actions.

### Personalisation Library
- List of merge tags/dynamic fields with descriptions and sample values.

### Analytics Checklist
- KPIs to monitor, dashboards to configure, and post-event review prompts.
</OUTPUT>
```

---
