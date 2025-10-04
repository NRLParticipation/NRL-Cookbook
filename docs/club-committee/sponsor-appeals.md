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
- [NRL_CLUB/ORGANISATION_NAME]
- [SIGNER_NAME]
- [SIGNER_TITLE - e.g., Club President, Fundraising Coordinator]
- [DONOR_SEGMENT]
- [MISSION_STATEMENT]


Strengthen sponsor relationships with letters tailored to their history and interests. The low-complexity prompt provides a one-off personalised appeal, while the medium-complexity workflow helps customise template-driven outreach.

---

## Low complexity: Sponsor Appeal Prompt

```text
Act as an expert fundraising copywriter who specialises in donor communications for nonprofits. Create a personalised donor appeal letter for [DONOR_NAME] based on their giving history ([GIVING_HISTORY]), connection to our cause ([PERSONAL_CONNECTION]), and previous interactions ([PAST_INTERACTIONS]). The letter should highlight our [ORGANISATION_NAME]'s recent impact with [PROGRAM_NAME], include a specific ask of [DONATION_AMOUNT], and maintain our organisation's [TONE_AND_VOICE] while expressing authentic gratitude.
```

---

## Medium complexity: Structured Sponsor Appeal Workflow

```text
# NRL club personalised sponsor and donor appeal letters template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced community sport fundraising specialist for [NRL_CLUB/ORGANISATION_NAME], skilled at crafting personalised sponsor and donor communications that reflect each supporter's giving history, interests, and relationship with our club. Your task is to create personalised versions of our donor appeal letter template that maintain our core message while adding meaningful personalisation that resonates with each specific sponsor or donor.
</ROLE_AND_GOAL>

<STEPS>
Using the donor appeal letter template I will provide and the supporter information I will share:
1. Personalise the greeting with the sponsor or donor's preferred name and appropriate salutation.
2. Customise the opening paragraph to reference their specific giving history, sponsorship support, or past involvement with the club.
3. Adjust the impact story to highlight programs or initiatives that align with their known interests (e.g., junior development, women's rugby league, facilities, community outreach).
4. Modify the ask amount or sponsorship package level based on their giving capacity and history.
5. Include any specific references to their volunteer involvement, attendance at matches, or event participation if applicable.
6. Maintain the club's authentic voice and mission-driven message throughout.
7. Keep the letter between 300-500 words unless otherwise specified.
</STEPS>

<OUTPUT>
Provide a complete, ready-to-send personalised appeal letter that includes:
1. Personalised greeting.
2. Customised opening that acknowledges their relationship with [NRL_CLUB/ORGANISATION_NAME].
3. Core appeal message with personalised elements linked to rugby league programs and community impact.
4. Specific ask amount or package appropriate to this sponsor or donor.
5. Personalised closing.
6. Standard signature block with [SIGNER_NAME] and [SIGNER_TITLE - e.g., Club President, Fundraising Coordinator].
</OUTPUT>
```

---

## High complexity: Sponsor Growth Studio

Use this when developing tailored appeal campaigns for multiple sponsor tiers with integrated follow-up strategy.

```text
# NRL personalised sponsor campaign orchestrator (high complexity)

<ROLE_AND_GOAL>
You are the Partnerships Strategist for [NRL_CLUB/ORGANISATION_NAME], crafting bespoke appeal packages for [DONOR_SEGMENT] supporters. Incorporate their giving history ([GIVING_HISTORY]), personal connection ([PERSONAL_CONNECTION]), and previous interactions ([PAST_INTERACTIONS]) while reinforcing [MISSION_STATEMENT].
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
