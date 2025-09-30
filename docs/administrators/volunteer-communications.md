# Volunteer recruitment and onboarding communications

**Category:** Administrators  
**Template type:** Template filling and personalisation

**Collect these inputs before you start:**

- [NRL_CLUB_NAME]
- [MISSION_STATEMENT - e.g., grow participation, support young players, strengthen community spirit]
- [VOLUNTEER_ROLE - e.g., coach, team manager, game day helper, canteen support]
- [TARGET_VOLUNTEER_DEMOGRAPHIC - e.g., parents, young adults, retirees, local businesses]
- [KEY_BENEFITS - e.g., accredited training, community connection, skill development, being part of the club family]
- [RECIPIENT_BACKGROUND - e.g., parent of a junior player, retired player, local business owner]
- [CLUB_SPECIFIC_NEEDS - e.g., Caloundra Sharks priorities, upcoming events to plug, values tone]
- [MISSION_STATEMENT]


Craft targeted volunteer outreach that speaks to different roles and audiences. The low-complexity prompt delivers a quick personalised message, while the medium-complexity workflow guides you through adapting templates for specific individuals or volunteer groups.

---

## Low complexity: volunteer outreach prompt

```text
Act as a community sport volunteer communications specialist and create personalised volunteer recruitment and onboarding messages for [NRL_CLUB_NAME], a grassroots rugby league organisation. Highlight our mission to [MISSION_STATEMENT - e.g., grow participation, support young players, strengthen community spirit] and the specific [VOLUNTEER_ROLE - e.g., coach, team manager, game day helper, canteen support] opportunities available. Adapt the tone to appeal to our [TARGET_VOLUNTEER_DEMOGRAPHIC - e.g., parents, young adults, retirees, local businesses] while emphasising both the impact volunteers make on the rugby league community and the benefits they receive, including [KEY_BENEFITS - e.g., accredited training, community connection, skill development, being part of the club family]. Make the message warm, welcoming, and clear about next steps for getting involved.
```

---

## Medium complexity: personalised volunteer journey workflow

```text
# NRL club volunteer recruitment and onboarding communications template (medium complexity)

<ROLE_AND_GOAL>
You are a volunteer coordinator and communications specialist for [NRL_CLUB_NAME], skilled at creating engaging, personalised communications that inspire action and make volunteers feel valued. Your task is to tailor our standard volunteer recruitment and onboarding templates to match specific rugby league volunteer opportunities, individual backgrounds, and club needs.
</ROLE_AND_GOAL>

<INPUT>
Provide:
- The volunteer role ([VOLUNTEER_ROLE - e.g., game day support, coaching, canteen, first aid, mentoring])
- Recipient background ([RECIPIENT_BACKGROUND - e.g., parent of a junior player, retired player, local business owner])
- Club-specific needs or tone preferences ([CLUB_SPECIFIC_NEEDS - e.g., Caloundra Sharks’ current priorities, upcoming events, values to highlight])
- Any additional logistical details (onboarding steps, contact person, start date)
</INPUT>

<STEPS>
Using our standard template content and the specific variables I provide, create personalised communications that:
1. Clearly explain the volunteer role, requirements, and impact on the club (e.g., supporting game day, coaching, mentoring juniors, running the canteen).
2. Address the recipient's specific skills, interests, or background ([RECIPIENT_BACKGROUND]) so the message feels tailored.
3. Weave in club-specific needs or tone preferences ([CLUB_SPECIFIC_NEEDS]) while conveying our mission and values.
4. Include clear next steps and calls to action (e.g., how to sign up, who to contact, what to bring on their first day).
5. Maintain a warm, appreciative, and community-minded tone throughout and reiterate why this role matters to [NRL_CLUB_NAME].
</STEPS>

<OUTPUT>
Provide the personalised communication with:
1. An attention-grabbing subject line (for emails or SMS).
2. A personalised greeting using the recipient's name.
3. Body content that integrates all provided variables naturally.
4. A clear call-to-action with specific next steps.
5. An appropriate closing that reinforces connection to the club's mission and rugby league community.
</OUTPUT>
```

---

## High complexity: volunteer lifecycle journey builder

Use this to design segmented nurture paths, automated follow-ups, and experimentation hooks for diverse volunteer personas.

```text
# Volunteer journey orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Volunteer Experience Lead for [NRL_CLUB_NAME]. Build a full lifecycle communications plan covering recruitment, onboarding, engagement, and retention for multiple persona groups (e.g., parents, alumni players, corporate teams). Keep the messaging aligned with our mission of [MISSION_STATEMENT] and NRL values.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (persona synthesis, content experiments, automation design)
- experimentation_mode: propose A/B tests with validation checkpoints every 30 days.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand persona motivations, availability, and barriers.
- Review volunteer data summaries provided (hours, roles, retention) and extract key insights.
- Summarise prior communications performance (open rates, sign-ups) and identify what worked.
- Capture volunteer role pipelines (e.g., game day support, coaching, canteen, first aid, mentoring) and note which backgrounds each role targets (parents, retired players, local business owners).
- Gather club-specific needs or tone preferences (current priorities, key events, values that must be highlighted) to inform messaging.
- Stop intake once you have at least two hypotheses per persona on messaging or channel approach.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Define 3-4 core personas with needs, motivators, preferred channels, role alignment, recipient backgrounds, and risk factors.
2. Map a 90-day communication journey for each persona, covering recruitment outreach, onboarding packets, role-specific tips, appreciation touchpoints, and re-engagement triggers.
3. Generate message templates (email, SMS, social DM) with dynamic fields for volunteer role, recipient background, availability, and benefits, plus placeholders for club-specific priorities.
4. Outline automation logic: segmentation rules, branching conditions, escalation paths for no-response scenarios.
5. Provide measurement framework (KPIs, dashboards, review cadence) and recommend prompt snippets for future analytics reviews.
</WORKFLOW>

<VALIDATION>
- Ensure messaging across steps stays consistent with mission and avoids conflicting instructions.
- Confirm accessibility (reading level, alt-text guidance for linked assets) and cultural inclusivity.
- Highlight dependencies on other systems (CRM, rostering) and provide fallback manual steps.
</VALIDATION>

<OUTPUT>
Deliver a markdown playbook featuring:
### Persona profiles
- Detailed descriptions covering motivators, barriers, tone guidance, recipient backgrounds, and aligned volunteer roles.

### Journey maps
- Ordered touchpoint lists per persona outlining channel, timing, and template references.

### Message templates
- Collection of drafts grouped by channel and lifecycle stage, ready for personalisation with volunteer role, recipient background, and club-specific notes.

### Automation plan
- Narrative describing trigger events, tooling notes, KPIs, and experimentation ideas.
</OUTPUT>
```

---
