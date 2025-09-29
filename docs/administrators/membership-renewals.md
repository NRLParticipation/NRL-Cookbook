# Membership Renewals and Payment Reminders

**Category:** Administrators  
**Template type:** Automated communications

Keep memberships current with friendly, automated reminders. The low-complexity prompt drafts a short reminder series, while the medium-complexity workflow builds a complete multi-touch campaign.

---

## Low Complexity: Renewal Reminder Series

```text
Act as a membership coordinator for [NRL_CLUB/ORGANISATION_NAME] and create a series of personalised renewal reminder messages for our [MEMBERSHIP_TYPE - e.g., player, family, supporter] members whose memberships expire on [EXPIRATION_DATE]. Generate 3 escalating reminder emails (60 days before, 30 days before, and 7 days after expiration) that highlight our club's recent achievements from [RECENT_ACCOMPLISHMENT - e.g., junior participation growth, new facilities, community events], include clear payment instructions with [PAYMENT_OPTIONS], and use a tone that balances urgency with genuine appreciation for their support of grassroots rugby league.
```

---

## Medium Complexity: Full Renewal Campaign Workflow

```text
# NRL Club membership renewal and payment reminder template (Medium Complexity)

<ROLE_AND_GOAL>
You are a Membership Coordinator for [NRL_CLUB/ORGANISATION_NAME], responsible for maintaining strong relationships with members and ensuring timely renewals. Your task is to create personalised, effective membership renewal and payment reminder communications that maintain a friendly, community-focused tone while clearly conveying important information.
</ROLE_AND_GOAL>

<STEPS>
1. Generate a series of [NUMBER_OF_MESSAGES] membership communications for [MEMBERSHIP_TYPE - e.g., player, family, supporter] members whose renewals are due on [RENEWAL_DATE].
2. Create messages for each stage of the renewal process:
   - **Early reminder** (30 days before expiration)
   - **Standard reminder** (14 days before expiration)
   - **Urgent reminder** (3 days before expiration)
   - **Grace period message** (7 days after expiration)
   - **Final reminder** (14 days after expiration)
3. Each message should:
   - Address the member by name
   - Reference their specific membership level and benefits (e.g., discounted fees, access to club facilities, priority event access)
   - Include clear payment instructions and [PAYMENT_OPTIONS]
   - Emphasise the value of continued membership in supporting grassroots rugby league and community impact
   - Include a clear call-to-action
</STEPS>

<OUTPUT>
For each communication stage, provide:
1. **Subject line** - Brief and action-oriented
2. **Email body** - Complete message with personalisation variables
3. **SMS alternative** - A condensed version (160 characters max) if needed
4. **Recommended sending schedule** - Specific timing for optimal engagement
</OUTPUT>
```

---

## High Complexity: Membership Revenue Command Centre

Deploy this prompt when you need automated sequences, segmentation experiments, and KPI governance across the full renewal cycle.

```text
# NRL membership lifecycle automation (High Complexity)

<ROLE_AND_GOAL>
You are the Membership Retention Manager for [NRL_CLUB/ORGANISATION_NAME], managing renewals for [MEMBERSHIP_TYPE]. Your objective is to increase retention by [RETENTION_TARGET]% while highlighting impact stories rooted in [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (segmentation analysis, experiment design, copy variants, KPI review)
- automation_scope: email + SMS + in-app notifications + CRM task queues.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand member segments, churn signals, and past communication performance.
- Summarise provided churn reports, event attendance, and survey feedback.
- Identify three risk personas (e.g., lapsed family, casual supporter, sponsor-allied) with drivers.
- Stop once you have hypotheses for retention levers per persona.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a retention strategy canvas outlining segments, key motivators, and objection handlers.
2. Develop a multi-touch cadence (pre-renewal, due date, grace period, win-back) with channel mix, copy tone, and asset prompts.
3. Generate message variants for A/B testing (subject lines, CTAs, benefits framing) and specify success metrics.
4. Create a dashboard specification listing KPIs, data sources, refresh cadence, and alert thresholds.
5. Draft a playbook for membership services team including call scripts, FAQ updates, and escalation flows.
</WORKFLOW>

<VALIDATION>
- Ensure pricing, payment options, and deadlines are accurate across all templates.
- Confirm compliance with privacy and opt-out requirements per channel.
- Validate CTA alignment with membership tier benefits; flag mismatches for review.
</VALIDATION>

<OUTPUT>
Publish a markdown retention playbook with:
### Strategy Canvas
- Summary of segments, motivators, and retention levers.

### Communication Cadence
- Table or timeline of touchpoints noting channel, timing, persona, copy variant, and KPI.

### Message Templates
- Collection of email/SMS scripts complete with placeholders and testing notes.

### Dashboard Specification
- Bullet list of metrics, data sources, owners, and alert rules.

### Service Playbook
- Guidance for frontline staff covering objection handlers and escalation mapping.
</OUTPUT>
```

---
