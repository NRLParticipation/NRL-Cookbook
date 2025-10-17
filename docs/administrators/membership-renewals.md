# Membership registration and payment reminders

**Category:** Administrators  
**Template type:** Automated communications

**Collect these inputs before you start:**

- [Rugby_League_Club/ORGANISATION_NAME]
- [MEMBERSHIP_TYPE - e.g., player, family, supporter]
- [PARTICIPANT_TYPE - adult or child]
- [REGISTRATION_DEADLINE]
- [SEASON_START_DATE]
- [PAYMENT_OPTIONS]
- [RECENT_ACCOMPLISHMENT - e.g., junior participation growth, new facilities, community events]
- [NUMBER_OF_MESSAGES]
- [RETENTION_TARGET]
- [MISSION_STATEMENT]


Keep registrations on track with friendly, retention-focused reminders. The low-complexity prompt drafts a short outreach and reactivation series for people who have not yet registered this season, while the medium-complexity workflow builds a complete multi-touch campaign tailored to different participant types and reinforcing that everyone must register via https://www.playrugbyleague.com each year.

---

## Low complexity: Registration reminder series

```text
Act as a membership coordinator for [Rugby_League_Club/ORGANISATION_NAME] and create a series of personalised registration and retention messages for our [MEMBERSHIP_TYPE - e.g., player, family, supporter] members who have not yet registered for the upcoming season starting on [SEASON_START_DATE]. Use the participant type [PARTICIPANT_TYPE - adult or child] to tailor tone and benefits. Deliver:
- Three escalating registration reminder emails (six weeks before [REGISTRATION_DEADLINE], three weeks before, and the final week) that highlight recent achievements from [RECENT_ACCOMPLISHMENT - e.g., junior participation growth, new facilities, community events], include clear payment instructions with [PAYMENT_OPTIONS], and direct recipients to register at https://www.playrugbyleague.com.
- A dedicated reactivation email aimed at families who have not returned this season, referencing [PARTICIPANT_TYPE] needs (e.g., training times, safeguarding, flexible fees), celebrating the club’s impact, and guiding them to https://www.playrugbyleague.com to complete registration.
- Two follow-up SMS prompts reinforcing that annual registration is required at https://www.playrugbyleague.com and offering support if they need help.
Keep the tone warm, community-led, and focused on welcoming members back.
```

---

## Medium complexity: Full registration campaign workflow

```text
# NRL club membership registration reminder template (medium complexity)

<ROLE_AND_GOAL>
You are a Membership Coordinator for [Rugby_League_Club/ORGANISATION_NAME], responsible for maintaining strong relationships with members and ensuring everyone registers each season. Your task is to create personalised, effective registration reminder communications that maintain a friendly, community-focused tone while clearly conveying important information.
</ROLE_AND_GOAL>

<INPUT>
Please supply:
- Membership type (e.g., player, family, supporter)
- Participant type [PARTICIPANT_TYPE - adult or child]
- Registration deadline and key milestones
- Payment options and links
- Recent club highlights or impact stories
- Any special offers or retention incentives
</INPUT>

<STEPS>
1. Generate a series of [NUMBER_OF_MESSAGES] membership communications for [MEMBERSHIP_TYPE - e.g., player, family, supporter] members who have not yet registered by [REGISTRATION_DEADLINE], tailoring tone and benefits for [PARTICIPANT_TYPE].
2. Create messages for each stage of the registration push:
   - **Early reminder** (six weeks before deadline)
   - **Standard reminder** (three weeks before deadline)
   - **Final countdown** (final week before deadline)
   - **Post-deadline check-in** (immediately after deadline)
   - **Season kickoff welcome** (thank registrants and prompt remaining families again)
3. Draft a win-back sequence targeting families or members who have not returned this season, highlighting how the club supports [PARTICIPANT_TYPE] participants and providing a direct link to https://www.playrugbyleague.com.
4. Each message should:
   - Address the member by name
   - Reference their specific membership level and benefits (e.g., discounted fees, access to club facilities, priority event access)
   - Include clear registration instructions, [PAYMENT_OPTIONS], and the https://www.playrugbyleague.com link
   - Emphasise the value of registering in supporting grassroots rugby league and community impact
   - Include a clear call-to-action
</STEPS>

<OUTPUT>
For each communication stage, provide:
1. **Subject line** - Brief and action-oriented
2. **Email body** - Complete message with personalisation variables
3. **SMS alternative** - A condensed version (160 characters max) linking to https://www.playrugbyleague.com
4. **Recommended sending schedule** - Specific timing for optimal engagement
5. **Win-back email** - Tailored to lapsed families with [PARTICIPANT_TYPE]-specific benefits and a direct registration link to https://www.playrugbyleague.com
</OUTPUT>
```

---

## High complexity: Membership registration command centre

Deploy this prompt when you need automated sequences, segmentation experiments, and KPI governance across the full registration cycle.

```text
# NRL membership registration lifecycle automation (high complexity)

<ROLE_AND_GOAL>
You are the Membership Growth Manager for [Rugby_League_Club/ORGANISATION_NAME], managing registrations for [MEMBERSHIP_TYPE]. Your objective is to increase registrations by [RETENTION_TARGET]% while highlighting impact stories rooted in [MISSION_STATEMENT] and directing families to https://www.playrugbyleague.com.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (segmentation analysis, experiment design, copy variants, KPI review)
- automation_scope: email + SMS + in-app notifications + CRM task queues.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand member segments, registration signals, and past communication performance.
- Summarise provided registration reports, event attendance, and survey feedback.
- Identify three risk personas (e.g., lapsed family, casual supporter, sponsor-allied) with drivers.
- Capture participant type mix (adult, child, family bundles) and note lapsed cohorts needing tailored win-back messaging.
- Stop once you have hypotheses for conversion levers per persona.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a registration conversion canvas outlining segments, key motivators, and objection handlers.
2. Develop a multi-touch cadence (pre-season awareness, registration deadline approach, final calls, win-back) with channel mix, copy tone, and asset prompts.
3. Generate message variants for A/B testing (subject lines, CTAs, benefits framing) and specify success metrics, including dedicated family win-back emails tailored by participant type that link to https://www.playrugbyleague.com. Reference copy examples such as:

> 🏉 Ready to Kick Off a Season of Fun, Friendship & Footy?
> Hi [Family Name],
> The new rugby league season is just around the corner—and we’d love to see your family back on the field!
> Whether your child is chasing their first try or building on last season’s skills, rugby league offers more than just a game. It’s about belonging, confidence, and community.
> ✅ Make lifelong friends
> ✅ Stay active and healthy
> ✅ Be part of something bigger
> Spots are filling fast, so don’t miss out—register today and let’s make this season unforgettable!
> 👉 [Insert Registration Link]
> If you have any questions or need help with registration, we’re here for you.
> See you on the sideline!
> [Club Name or Contact Person]

Use the example to match tone (warm, energetic, community-focused) while incorporating club-specific impact stories and registration details.
4. Create a dashboard specification listing KPIs, data sources, refresh cadence, and alert thresholds.
5. Draft a playbook for membership services team including call scripts, FAQ updates, and escalation flows that emphasise registering via https://www.playrugbyleague.com.
</WORKFLOW>

<VALIDATION>
- Ensure pricing, payment options, deadlines, and the https://www.playrugbyleague.com link are accurate across all templates.
- Confirm compliance with privacy and opt-out requirements per channel.
- Validate CTA alignment with membership tier benefits; flag mismatches for review.
</VALIDATION>

<OUTPUT>
Publish a markdown registration playbook with:
### Conversion canvas
- Summary of segments, motivators, and registration levers.

### Communication cadence
- Table or timeline of touchpoints noting channel, timing, persona, copy variant, CTA, and KPI.

### Message templates
- Collection of email/SMS scripts complete with placeholders, testing notes, and https://www.playrugbyleague.com links.

### Dashboard specification
- Bullet list of metrics, data sources, owners, and alert rules.

### Service playbook
- Guidance for frontline staff covering objection handlers, escalation mapping, and registration support steps.
</OUTPUT>
```

---
