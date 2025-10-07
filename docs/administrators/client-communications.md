# Client service communication follow-up

**Category:** Administrators  
**Template type:** Template filling and personalisation

**Collect these inputs before you start:**

- [TEMPLATE_TYPE - e.g., welcome email, follow-up message, thank-you note]
- [RECIPIENT_FIRST_NAME]
- [RECIPIENT_CONTEXT - e.g., new player registration, parent of junior, volunteer role, sponsor involvement]
- [RECENT_INTERACTION - e.g., registration assistance, training session, sponsor package]
- [NEXT_STEPS - e.g., upcoming games, orientation session, volunteer briefing, payment confirmation]
- [NRL_CLUB/ORGANISATION_NAME]
- [CLUB_VALUES - e.g., teamwork, respect, inclusivity, community spirit]
- [AUDIENCE_SET - e.g., new members, volunteers, sponsors]
- [CLUB_TONE]


Personalise member, volunteer, and sponsor follow-ups with ease. Use the low-complexity prompt for quick adaptations, or the medium-complexity workflow when you need structured guidance across multiple touchpoints.

---

## Low complexity: Personalised follow-up prompt

```text
Act as a community sport member communications specialist and personalise this [TEMPLATE_TYPE - e.g., welcome email, follow-up message, thank-you note] for [RECIPIENT_FIRST_NAME] based on their [RECIPIENT_CONTEXT - e.g., new player registration, parent of junior, volunteer role, sponsor involvement] and our recent [RECENT_INTERACTION - e.g., registration assistance, training session, sponsor package]. Include relevant follow-up information about [NEXT_STEPS - e.g., upcoming games, orientation session, volunteer briefing, payment confirmation], maintain [NRL_CLUB/ORGANISATION_NAME]'s warm and community-focused tone, and ensure all information stays generic enough that no personal contact details or sensitive data are included.
```

---

## Medium complexity: Structured communication workflow

```text
# Member and volunteer communications template (medium complexity)

<ROLE_AND_GOAL>
You are a community sport communications specialist for [NRL_CLUB/ORGANISATION_NAME], responsible for creating personalised follow-up communications that strengthen our relationship with members, volunteers, players, and sponsors while efficiently delivering important information.
</ROLE_AND_GOAL>

<STEPS>
1. Use the context I provide to personalise our standard communication template without repeating personal contact details or sensitive data.
2. Adapt the tone and level of detail to match their specific situation and communication preferences.
3. Include all required information from our template while making it feel personal and community-focused.
4. Reference specific details about their role, registration, or recent involvement where appropriate.
5. Maintain a warm, supportive tone that reflects [NRL_CLUB/ORGANISATION_NAME]'s values of [CLUB_VALUES - e.g., teamwork, respect, inclusivity, community spirit].
</STEPS>

<OUTPUT>
Provide a personalised communication that includes:
1. **Warm, personalised greeting** using the recipient's preferred name.
2. **Specific references** to their situation, role, or last interaction with the club (keep details high level; avoid personal contact information).
3. **Clear next steps or action items** (if applicable).
4. **Relevant resource information** tailored to their needs (e.g., training times, event details, sponsor benefits).
5. **Standard closing** with appropriate club contact information.
</OUTPUT>
```

---

## High complexity: Relationship communications control tower

Use this when you must coordinate multi-touch, multi-channel follow-ups across members, volunteers, and partners while integrating data-driven insights.

```text
# Member and volunteer communications orchestrator (high complexity)

<ROLE_AND_GOAL>
You are the Community Engagement Manager for [NRL_CLUB/ORGANISATION_NAME]. Build a communications plan covering follow-ups for [AUDIENCE_SET - e.g., new members, volunteers, sponsors] about [SERVICE_PROVIDED]. Ensure each message reinforces [CLUB_VALUES] and advances strategic goals (retention, participation, revenue).
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (persona analysis, sentiment tailoring, journey mapping, QA)
- delivery_mode: produce templates, journey maps, and analytics hooks.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand recipient history, preferences, and outstanding needs.
- Summarise CRM notes, survey responses, and engagement metrics provided.
- Identify risk indicators (e.g., low attendance, overdue payment) and motivators.
- Stop when each persona has clear goals, pain points, and preferred channels documented.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Create persona vault entries capturing motivations, concerns, and tone preferences.
2. Map a communications journey (initial follow-up, nurture, escalation, celebration) for each persona across email, SMS, and social.
3. Draft message templates with dynamic fields and personalisation tokens, including optional branches for positive/negative sentiment.
4. Define analytics plan: KPIs, data collection methods, experimentation ideas.
5. Provide quality assurance checklist (accessibility, compliance, data privacy) and escalation guidance for complex queries.
</WORKFLOW>

<VALIDATION>
- Ensure all templates embed accurate next steps, deadlines, and contact info.
- Check for consistency in tone with [CLUB_TONE] and highlight any adjustments needed.
- Confirm CTA alignment with strategic objectives; note conflicts for review.
</VALIDATION>

<OUTPUT>
Deliver a markdown communications guide featuring:
### Persona library
- Profiles with tone guidance, motivations, and concerns.

### Journey sequences
- Channel-by-channel timelines outlining timing and goals for each persona.

### Message templates
- Full drafts tagged by persona, channel, and lifecycle stage.

### Analytics plan
- KPIs, measurement methods, and review cadence.

### QA checklist
- Compliance and accessibility checks to complete before sending.
</OUTPUT>
```

---
