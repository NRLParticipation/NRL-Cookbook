# Converting written content to video scripts

**Category:** Marketing and PR  
**Template type:** Content adaptation and reformatting

**Collect these inputs before you start:**

- [Rugby_League_Club/ORGANISATION_NAME]
- [TOPIC]
- [TARGET_AUDIENCE]
- [Suggested title]
- [Estimated length in minutes]
- [SCENE 1 DESCRIPTION]
- [Text to be spoken]
- [Description of what should appear on screen]
- [SCENE 2 DESCRIPTION]
- [Continue with additional scenes as needed]
- [Clear next step for viewers - e.g., register, volunteer, attend a match, support the club]
- [MISSION_STATEMENT]


Turn articles and updates into engaging video narratives. The low-complexity prompt adapts content quickly, while the medium-complexity workflow provides scene-by-scene scripting with visuals and timing. *Note: if a workflow suggests “DALL-E prompts”, they are optional text briefs you can paste into ChatGPT’s image tools or the DALL-E website to create supporting imagery, or hand to designers for reference.*

---

## Low complexity: Video script prompt

```text
As a community sport video script expert, transform [Rugby_League_Club/ORGANISATION_NAME]'s written content about [TOPIC] into an engaging video script that captures our mission while being visually compelling. Maintain our key messages and impact stories, but adapt the language to be more conversational, include visual scene descriptions (e.g., game day action, volunteer highlights, junior players), and structure it with clear segments that will resonate with our [TARGET_AUDIENCE].
```

---

## Medium complexity: Structured video script workflow

```text
# NRL club video script conversion template (medium complexity)

<ROLE_AND_GOAL>
You are a community sport video script specialist who excels at transforming written content into engaging, concise video scripts that highlight grassroots rugby league impact. Your task is to convert [Rugby_League_Club/ORGANISATION_NAME]'s written content about [TOPIC] into a compelling video script that will resonate with [TARGET_AUDIENCE] while showcasing the club's mission, values, and community spirit.
</ROLE_AND_GOAL>

<STEPS>
1. Review the provided written content and identify the three to five most important messages that must be included in the video.
2. Transform the content into a conversational script with clear scene descriptions, narration text, and visual cues (e.g., match day action, training, volunteers, community events).
3. Adapt the language to be concise and engaging for video format (aim for 150-200 words per minute of video).
4. Organise the script into a logical flow with a strong introduction, key messages, and an inspiring call-to-action.
5. Highlight [Rugby_League_Club/ORGANISATION_NAME]'s impact through visual examples of players, coaches, and community involvement.
</STEPS>

<OUTPUT>
Provide the video script in the following format:
VIDEO TITLE: [Suggested title]
DURATION: [Estimated length in minutes]
SCRIPT:
[SCENE 1 DESCRIPTION]
NARRATION: [Text to be spoken]
VISUAL: [Description of what should appear on screen]
[SCENE 2 DESCRIPTION]
NARRATION: [Text to be spoken]
VISUAL: [Description of what should appear on screen]
[Continue with additional scenes as needed]
CALL TO ACTION: [Clear next step for viewers - e.g., register, volunteer, attend a match, support the club]
</OUTPUT>
```

---

## High complexity: Video story production studio

Use this when transforming large content sets into multi-segment video scripts with storyboard cues and optimisation notes.

```text
# NRL video storytelling orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Video Content Director for [Rugby_League_Club/ORGANISATION_NAME], adapting written materials about [TOPIC] into an engaging video series targeting [TARGET_AUDIENCE]. Produce primary script, teaser versions, shot list, and post-launch analytics plan while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (content distillation, scene planning, accessibility, optimisation strategy)
- delivery_bundle: script, shot plan, asset prompts, repurposing ideas.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: capture key messages, visuals, and emotional beats without duplicating effort.
- Summarise essential points from the written content, noting quotes, stats, and stories.
- Understand distribution goals (platforms, duration targets, CTAs) and compliance needs.
- Stop when you can outline a narrative spine and supporting visuals or list gaps requiring approval.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Create a narrative outline (hook, proof, impact, CTA) and map scenes to key messages.
2. Draft the full script including narrator lines, on-screen text, and audio cues, sized for target duration.
3. Develop a shot list/storyboard notes: visuals, camera moves, b-roll ideas, DALL-E prompts if required.
4. Generate derivative assets: 30-second teaser script, social cutlines, and caption copy.
5. Outline accessibility and optimisation plan (captions, audio description, aspect ratios, analytics to monitor).
</WORKFLOW>

<VALIDATION>
- Ensure timing estimates align with platform guidelines (150-200 words/minute baseline).
- Confirm CTAs and mission references appear consistently across versions.
- Check accessibility requirements (captions, contrast for text overlays) and highlight any pending approvals.
</VALIDATION>

<OUTPUT>
Deliver a markdown video kit with:
### Full script
- Scene-by-scene layout pairing narration, visuals, and on-screen text.

### Shot and asset plan
- Table listing scene, visual direction, audio cues, and asset prompts.

### Derivative content
- Teaser script, social captions, and thumbnail ideas.

### Accessibility and optimisation checklist
- Items covering captions, audio description, aspect ratios, and analytics tracking.
</OUTPUT>
```

---
