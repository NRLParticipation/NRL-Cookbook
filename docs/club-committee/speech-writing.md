# Speech writing for events and presentations

**Category:** Club Committee  
**Template type:** Script and narrative writing

**Collect these inputs before you start:**

- [LENGTH]
- [NRL_CLUB/ORGANISATION_NAME]
- [TOPIC]
- [AUDIENCE - e.g., players, families, sponsors, community leaders]
- [EVENT_TYPE - e.g., season launch, awards night, fundraiser]
- [MISSION_STATEMENT - e.g., growing participation, supporting juniors, building community spirit]
- [KEY_MESSAGE - e.g., teamwork, inclusivity, resilience]
- [DESIRED_OUTCOME - e.g., new memberships, volunteer sign-ups, sponsorship support]
- [TONE - e.g., inspiring, celebratory, heartfelt]
- [LENGTH_IN_MINUTES]
- [SPEAKER_ROLE - e.g., Club President, Head Coach, Captain]
- [EVENT_NAME - e.g., season launch, presentation night, sponsor luncheon]
- [AUDIENCE_DESCRIPTION - e.g., players, families, sponsors, community leaders]
- [MISSION_STATEMENT - e.g., growing participation, supporting juniors, strengthening community spirit]
- [KEY_MESSAGE_1]
- [KEY_MESSAGE_2]
- [KEY_MESSAGE_3]
- [AUDIENCE_DESCRIPTION]
- [WORD_COUNT]
- [SPEAKER_ROLE]
- [EVENT_NAME]
- [MISSION_STATEMENT]


Craft memorable speeches that inspire action and celebrate your club. The low-complexity prompt delivers a ready-to-read script, while the medium-complexity workflow helps tailor speeches to different events and audiences.

---

## Low complexity: event speech prompt

```text
Act as an expert speechwriter for community sport organisations. Write a compelling [LENGTH]-minute speech for [NRL_CLUB/ORGANISATION_NAME] about [TOPIC] that will resonate with [AUDIENCE - e.g., players, families, sponsors, community leaders] at our upcoming [EVENT_TYPE - e.g., season launch, awards night, fundraiser]. Include our mission of [MISSION_STATEMENT - e.g., growing participation, supporting juniors, building community spirit], incorporate [KEY_MESSAGE - e.g., teamwork, inclusivity, resilience], and end with a clear call to action that inspires [DESIRED_OUTCOME - e.g., new memberships, volunteer sign-ups, sponsorship support]. Use a [TONE - e.g., inspiring, celebratory, heartfelt] tone throughout.
```

---

## Medium complexity: structured speech workflow

```text
# NRL club speech writing template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced speechwriter for community sport organisations who understands how to craft compelling narratives that inspire action, connect with diverse audiences, and effectively communicate mission-driven messages. Your task is to create a [LENGTH_IN_MINUTES]-minute speech for [NRL_CLUB/ORGANISATION_NAME] about [TOPIC] that will be delivered by [SPEAKER_ROLE - e.g., Club President, Head Coach, Captain] at [EVENT_NAME - e.g., season launch, presentation night, sponsor luncheon] to an audience of [AUDIENCE_DESCRIPTION - e.g., players, families, sponsors, community leaders].
</ROLE_AND_GOAL>

<STEPS>
1. Create a speech that aligns with [NRL_CLUB/ORGANISATION_NAME]'s mission of [MISSION_STATEMENT - e.g., growing participation, supporting juniors, strengthening community spirit] and incorporates these key messages: [KEY_MESSAGE_1], [KEY_MESSAGE_2], [KEY_MESSAGE_3].
2. Structure the speech with a compelling opening hook, clear main points with supporting evidence or stories, and a strong call-to-action conclusion.
3. Include at least one personal story or case example that illustrates the club's impact (e.g., a player's journey, a volunteer's contribution, a community achievement).
4. Adapt the language and tone to be appropriate for [AUDIENCE_DESCRIPTION] while maintaining the club's authentic voice and values.
5. Ensure the speech can be delivered within [LENGTH_IN_MINUTES] minutes (approximately [WORD_COUNT] words).
</STEPS>

<OUTPUT>
Provide the complete speech script with:
1. **Title**
2. **Full speech text** with paragraph breaks and natural speaking rhythm
3. **Approximate delivery time**
4. **Brief delivery notes** (pacing, emphasis points, pauses)
</OUTPUT>
```

---

## High complexity: speech campaign studio

Use this when you need multiple speech variants, rehearsal assets, and follow-up communications aligned with key objectives.

```text
# NRL event speech orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Communications Lead for [NRL_CLUB/ORGANISATION_NAME], supporting [SPEAKER_ROLE] to deliver a [LENGTH_IN_MINUTES]-minute speech on [TOPIC] at [EVENT_NAME]. Produce a primary script plus alternate excerpts, integrate audience interaction cues, and prepare post-event messaging while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 6 (audience insight, storytelling design, emotion mapping, CTA development, rehearsal planning)
- delivery_bundle: main script, highlight reel excerpt, Q and A prep, follow-up comms.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: gather audience demographics, event context, and desired outcomes.
- Summarise attendee makeup, past event themes, and organisational priorities provided.
- Capture key stories or data points that must appear; cite sources.
- Stop when you can outline a three-act structure and key emotional beats or list unresolved gaps.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Map the narrative arc (hook, proof, impact, call-to-action) with emotional tone shifts.
2. Draft the full speech, ensuring pacing suits [LENGTH_IN_MINUTES] minutes (approx. [WORD_COUNT] words) and includes at least one personal story.
3. Produce optional components: 2-minute highlight excerpt, quote cards, and social teaser copy.
4. Create a rehearsal plan with emphasis points, gesture cues, and audience interaction prompts.
5. Provide post-event follow-up messaging suggestions (email recap, media release summary, sponsor thank-you note).
</WORKFLOW>

<VALIDATION>
- Check for source attribution on data or quotes; mark any needing approval.
- Ensure tone matches audience expectations ([AUDIENCE_DESCRIPTION]) and maintains accessibility.
- Confirm CTA aligns with DESIRED_OUTCOME and includes a clear action.
</VALIDATION>

<OUTPUT>
Deliver a markdown speech pack comprising:
### Full script
- Paragraph-form speech ready for delivery with stage directions.

### Highlight assets
- Short excerpt, quote cards, and social teaser copy.

### Rehearsal guide
- Notes on pacing, emphasis, gestures, and audience engagement moments.

### Follow-up messaging
- Bulleted suggestions for post-event communications tied to the speech themes.
</OUTPUT>
```

---
