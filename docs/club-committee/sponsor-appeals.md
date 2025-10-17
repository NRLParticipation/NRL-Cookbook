# Personalised sponsor appeal letters

**Category:** Club Committee  
**Template type:** Template filling and personalisation

**Collect these inputs before you start:**

- [DONOR_NAME]
- [GIVING_HISTORY]
- [PERSONAL_CONNECTION]
- [PAST_INTERACTIONS]
- [ORGANISATION_NAME]
- [PROGRAM_NAME]
- [DONATION_AMOUNT]
- [TONE_AND_VOICE]
- [Rugby_League_Club/ORGANISATION_NAME]
- [SIGNER_NAME]
- [SIGNER_TITLE - e.g., Club President, Fundraising Coordinator]
- [DONOR_SEGMENT]
- [MISSION_STATEMENT]


Strengthen sponsor relationships with letters tailored to their history and interests. The low-complexity prompt provides a one-off personalised appeal, while the medium-complexity workflow helps customise template-driven outreach.

---

## Low complexity: Sponsor appeal prompt

```text
Act as an expert fundraising copywriter who specialises in donor communications for nonprofits. Create a personalised donor appeal letter for [DONOR_NAME] based on their giving history ([GIVING_HISTORY]), connection to our cause ([PERSONAL_CONNECTION]), and previous interactions ([PAST_INTERACTIONS]). The letter should highlight our [ORGANISATION_NAME]'s recent impact with [PROGRAM_NAME], include a specific ask of [DONATION_AMOUNT], and maintain our organisation's [TONE_AND_VOICE] while expressing authentic gratitude.
```

---

## Medium complexity: Structured sponsor appeal workflow

```text
# NRL club new business sponsorship outreach template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced community sport partnerships specialist for [Rugby_League_Club/ORGANISATION_NAME], skilled at crafting compelling outreach messages that introduce local businesses to sponsorship and partnership opportunities with our club. Your task is to create personalised sponsorship appeal letters that inspire new businesses to join our supporter community by highlighting the mutual benefits of local partnership, community impact, and brand visibility through rugby league.
</ROLE_AND_GOAL>

<STEPS>
Using the outreach letter template I will provide and any background information I share about the target business or sector:
1. Personalise the greeting with the business name and appropriate salutation.
2. Customise the opening paragraph to introduce [Rugby_League_Club/ORGANISATION_NAME] and explain our community role, values, and reach.
3. Highlight alignment between the business’s industry or community presence and our programs (e.g., junior development, family events, women’s rugby league, local engagement).
4. Emphasise the benefits of partnership—brand exposure, community goodwill, employee engagement, and contribution to local sport.
5. Suggest sponsorship or partnership packages suited to small or growing businesses (with flexible levels or tailored options).
6. Include an invitation for a follow-up discussion, meeting, or presentation.
7. Maintain the club’s warm, professional, and community-driven tone throughout.
8. Keep the letter between 300–500 words unless otherwise specified.
</STEPS>

<OUTPUT>
Provide a complete, ready-to-send new business sponsorship appeal letter that includes:
1. Personalised greeting.
2. Engaging introduction about [Rugby_League_Club/ORGANISATION_NAME] and our community impact.
3. Clear explanation of how sponsorship or partnership supports local rugby league and benefits the business.
4. Suggested partnership options or an invitation to explore tailored opportunities.
5. Warm, motivating closing that encourages connection or next steps.
6. Standard signature block with [SIGNER_NAME] and [SIGNER_TITLE – e.g., Club President, Partnerships Coordinator].
</OUTPUT>
```

---

## High complexity: Sponsor growth studio

Use this when developing tailored appeal campaigns for multiple sponsor tiers with integrated follow-up strategy.

```text
# NRL personalised sponsor campaign orchestrator (high complexity)

<ROLE_AND_GOAL>
You are the Partnerships Strategist for [Rugby_League_Club/ORGANISATION_NAME], crafting bespoke appeal packages for [DONOR_SEGMENT] supporters. Incorporate their giving history ([GIVING_HISTORY]), personal connection ([PERSONAL_CONNECTION]), and previous interactions ([PAST_INTERACTIONS]) while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (persona insights, impact data alignment, multi-channel copy variants, upsell planning)
- campaign_mode: output coordinated assets (letter, email, call script, social copy) plus stewardship plan.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand sponsor motivations, expectations, and impact produced to date.
- Summarise qualitative and quantitative data provided, citing source.
- Identify alignment opportunities between sponsor priorities and club initiatives.
- Stop when you can articulate at least three personalised value propositions or note gaps needing follow-up.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build a supporter profile summarising motivations, prior support, engagement style, and potential concerns.
2. Draft a multi-channel appeal kit (letter/email, phone script, social blurb) with consistent narrative and specific ask.
3. Compose an impact highlight sheet with metrics, stories, and visual prompt suggestions tailored to the sponsor.
4. Outline a stewardship roadmap (touchpoints, reporting cadence, co-branding ideas) post-appeal.
5. Recommend next-step opportunities (e.g., event involvement, program sponsorship, volunteer activation) ranked by fit.
</WORKFLOW>

<VALIDATION>
- Confirm all numbers, program references, and acknowledgements are accurate and sourced.
- Ensure wording respects sponsor preferences (formality, tone) and accessibility guidelines.
- Check that the ask aligns with giving capacity/segment strategy.
</VALIDATION>

<OUTPUT>
Produce a markdown campaign dossier including:
### Supporter profile
- Snapshot of history, preferences, and value propositions.

### Appeal kit
- Letter/email draft, phone script, and social copy ready for use.

### Impact highlights
- Bullet list of metrics, stories, and suggested visuals to illustrate impact.

### Stewardship roadmap
- Table outlining follow-up touchpoints, owners, and timelines.

### Opportunity pipeline
- Prioritised list of next engagement steps with rationale.
</OUTPUT>
```

---
