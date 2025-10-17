# Event registrations and follow-ups

**Category:** Events  
**Template type:** Automated communications

**Collect these inputs before you start:**

- [NRL_CLUB/ORGANISATION_NAME]
- [EVENT_NAME]
- [EVENT_DATE]
- [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, building community spirit]
- [REMINDER_TIMEFRAME]
- [FINAL_DETAILS_TIMEFRAME]
- [FOLLOW_UP_ACTION - e.g., feedback survey, membership renewal, volunteer sign-up]
- [EVENT_LOCATION]
- [EVENT_TIME]
- [PARKING_INFO]
- [WHAT_TO_BRING]
- [DRESS_CODE]
- [MISSION_STATEMENT]
- [FOLLOW_UP_ACTION]


Keep attendees informed from sign-up to post-event. The low-complexity prompt generates a full email series, while the medium-complexity workflow offers customisable templates with timing guidance.

---

## Low complexity: Registration follow-up prompt

```text
Act as an event communications coordinator for [NRL_CLUB/ORGANISATION_NAME] and generate a set of follow-up emails for our [EVENT_NAME] on [EVENT_DATE], including: a registration confirmation, a one-week reminder with event details, a day-before reminder with last-minute instructions, and a post-event thank you message that requests feedback. Use a warm, welcoming tone that reflects our mission of [MISSION_STATEMENT - e.g., growing participation, celebrating volunteers, building community spirit], and include our club logo and contact information in each message.
```

---

## Medium complexity: Structured registration workflow

```text
NRL club event registration follow-up and confirmation template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced Event Coordinator for [NRL_CLUB/ORGANISATION_NAME], responsible for managing all communication with registrants for our [EVENT_NAME]. Your task is to create personalised, timely follow-up messages and confirmations that maintain engagement, provide necessary information, and reduce no-shows.
</ROLE_AND_GOAL>

<STEPS> Generate a complete set of event communication templates based on the following information: 1. Create a **confirmation email** to be sent immediately after registration. 2. Design a **reminder email** for [REMINDER_TIMEFRAME] before the event. 3. Develop a **final details email** for [FINAL_DETAILS_TIMEFRAME] before the event. 4. Create a **post-event thank-you email** with [FOLLOW_UP_ACTION – e.g., feedback survey, membership renewal, volunteer sign-up] request.

For each template:

Include a clear, engaging subject line.

Incorporate [NRL_CLUB/ORGANISATION_NAME] branding elements and tone (e.g., warm, community-focused, professional).

Include all critical information ([EVENT_LOCATION], [EVENT_DATE], [EVENT_TIME]).

Add any special instructions ([PARKING_INFO], [WHAT_TO_BRING], [DRESS_CODE]).

</STEPS>
<OUTPUT> For each communication template, provide: 1. **Subject line** – Brief, clear subject line. 2. **Email body** – Complete email text with all placeholders properly positioned. 3. **Send timing** – Recommended timing for sending this communication. 4. **Customisation notes** – Brief notes on how to adapt this template for different event types (e.g., game days, awards nights, fundraisers, sponsor luncheons). </OUTPUT>
```

