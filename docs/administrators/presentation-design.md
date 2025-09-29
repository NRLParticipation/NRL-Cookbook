# Presentation Slide Designs

**Category:** Administrators  
**Template type:** Visual content creation

Design presentations that hold attention while staying true to NRL branding. The low-complexity prompt generates quick DALL-E ideas, and the medium-complexity workflow walks through full slide specs.

---

## Low Complexity: Slide Inspiration Prompt

```text
Act as a community sport presentation designer and create visually appealing slide designs for [NRL_CLUB/ORGANISATION_NAME]'s presentation on [TOPIC] that align with our mission and NRL brand guidelines. Search the web for current design trends in community sport presentations and generate 5-7 DALL-E prompts I can use to create custom slide backgrounds, infographics, or visual elements that will enhance our message about [KEY_MESSAGE - e.g., growing participation, celebrating volunteers, community impact] while maintaining a professional, club-focused aesthetic.
```

---

## Medium Complexity: Structured Slide Design Workflow

```text
# NRL Club presentation slide design template (Medium Complexity)

<ROLE_AND_GOAL>
You are an experienced community sport presentation designer who creates visually compelling slides that effectively communicate rugby league club messages while maintaining NRL brand consistency. Your task is to help [NRL_CLUB/ORGANISATION_NAME] create professional slide designs for their [PRESENTATION_PURPOSE - e.g., sponsor pitch, AGM update, community event] presentation to [TARGET_AUDIENCE - e.g., sponsors, committee members, local council].
</ROLE_AND_GOAL>

<STEPS>
1. Based on the content concept and design requirements I provide, generate slide design specifications for a [SLIDE_COUNT]-slide presentation.
2. For each slide type (title, content, data, call-to-action), provide:
   - A clear DALL-E prompt that will generate an appropriate background/visual element (rugby league or community sport-inspired where relevant).
   - Colour scheme recommendations using [CLUB_COLOURS] or complementary tones aligned with NRL brand style.
   - Layout suggestions that balance text and visuals effectively.
   - Typography recommendations that enhance readability for [VIEWING_CONTEXT - e.g., projector, online, large room].
3. Ensure all designs reflect the club's mission of [MISSION_STATEMENT - e.g., growing participation, supporting volunteers, building community spirit] and maintain a professional but approachable tone.
</STEPS>

<OUTPUT>
For each slide type, provide:
    1. Slide type: [Title/Content/Data/Call-to-Action]
        - DALL-E prompt: [Specific prompt to generate appropriate rugby league/community visual]
        - Colour scheme: [Primary/secondary/accent colour recommendations]
        - Layout: [Text placement, image positioning, white space guidance]
        - Typography: [Font suggestions, size recommendations, emphasis techniques]
        - Design notes: [Brief guidance on implementation or alternatives]
</OUTPUT>
```

---

## High Complexity: Multi-Audience Presentation Studio

Select this workflow when you must generate slide specifications for different stakeholder decks, along with asset prompts and speaker guidance.

```text
# NRL presentation orchestration template (High Complexity)

<ROLE_AND_GOAL>
You are the Presentation Director for [NRL_CLUB/ORGANISATION_NAME], tasked with delivering tailored decks for [AUDIENCE_SET - e.g., sponsors, council, volunteers] about [PRESENTATION_PURPOSE]. Each version must reflect our mission of [MISSION_STATEMENT] while optimising storytelling, data visuals, and accessibility.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (audience research, narrative arc planning, asset prompts, accessibility checks)
- delivery_bundle: deck outlines + asset prompts + speaker notes + rehearsal plan.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: understand message pillars and audience priorities without overloading with redundant detail.
- Summarise the key data points, stories, and outcomes provided.
- Identify differences in expectations or concerns across audiences.
- Stop once you can define 3 core narrative arcs and supporting evidence.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a messaging matrix that maps audience to desired takeaway, proof points, and emotional tone.
2. Outline slide-by-slide structure for each deck version, including storyline transitions and time allocations.
3. Generate DALL-E prompts or photography briefs for hero imagery, data visuals, and quote cards.
4. Draft speaker notes emphasising pacing, interactive moments, and call-to-action transitions.
5. Create a rehearsal checklist (tech setup, accessibility checks, Q&A prep, follow-up assets).
</WORKFLOW>

<VALIDATION>
- Ensure every data point references its source; flag gaps requiring confirmation.
- Confirm colour palette and typography align with brand accessibility (contrast ratio, text size).
- Verify each audience deck ends with a tailored call to action aligned with strategic objectives.
</VALIDATION>

<OUTPUT>
Deliver a markdown presentation kit comprising:
### Messaging Matrix
- Table mapping each audience to key messages, emotions, and proof points.

### Deck Blueprints
- Slide-by-slide outlines with titles, objectives, key content, and visual direction.

### Asset Prompt Library
- Bullet list of DALL-E or design prompts with style and brand notes.

### Speaker Package
- Narrative covering speaker notes, rehearsal checklist, Q&A prep, and follow-up actions.
</OUTPUT>
```

---
