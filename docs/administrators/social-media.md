# Social media posts and content calendars

**Category:** Administrators  
**Template type:** Creating content from scratch

**Collect these inputs before you start:**

- [NRL_CLUB_NAME]
- [MISSION_FOCUS - e.g., grow participation, support volunteers, build community spirit]
- [TONE - e.g., friendly, family-focused, inspiring]
- [PROGRAM_NAME - e.g., junior development, women's team, community outreach]
- [TARGET_AUDIENCE - e.g., local families, players, sponsors]
- [PRIMARY_GOAL - e.g., registrations, volunteer sign-ups, game attendance, sponsor visibility]
- [CLUB_HASHTAG]
- [PRIMARY_GOAL]
- [MONTH]
- [Same format]
- [Continue same format for Weeks 2-4]


Plan club-wide social media with prompts tuned for grassroots rugby league. Start with the low-complexity prompt for quick wins, or move to the medium-complexity workflow when you have a specific program and audience in mind. Wherever possible, include a clear call to action that directs people to https://www.playrugbyleague.com for centralised registrations and resources. *Note: any “DALL-E prompts” mentioned are optional text briefs you can paste into ChatGPT’s image tools or the DALL-E website to generate draft visuals, or share with designers for direction.*

---

## Low complexity: Monthly Content Sprint

```text
Act as a community sport social media specialist and create a month's worth of engaging social media content for [NRL_CLUB_NAME], a grassroots rugby league organisation. Focus on our mission to [MISSION_FOCUS - e.g., grow participation, support volunteers, build community spirit].

Use the NRL content portal (https://skoop.com.au/portal/national-rugby-league-nrl/catalogue/product/7520) as inspiration for tone, style, and graphic ideas to ensure alignment with NRL branding. Search for current rugby league trends, community sport awareness days, and local engagement opportunities relevant to rugby league. Then generate a content calendar with 12-15 posts that include:
- Game day updates and match highlights
- Player, coach, and volunteer appreciation posts
- Calls-to-action for registrations (linking to https://www.playrugbyleague.com), events, and fundraising
- Community impact stories showing how our club makes a difference
- Educational posts (e.g., child safety, wellbeing, respect in sport)

Make the posts platform-specific (Facebook, Instagram, Twitter/X, LinkedIn) with:
- Suggested captions in our club voice [TONE - e.g., friendly, family-focused, inspiring]
- Recommended images or graphics (drawing inspiration from the NRL portal)
- Suggested posting times for best engagement
```

---

## Medium complexity: Structured Calendar Workflow

```text
# NRL club social media content calendar template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced sports and community social media manager who creates engaging, mission-aligned content that resonates with players, volunteers, supporters, and sponsors. Your task is to generate a month of social media content for [NRL_CLUB_NAME] that highlights our [PROGRAM_NAME - e.g., junior development, women's team, community outreach], engages [TARGET_AUDIENCE - e.g., local families, players, sponsors], and drives [PRIMARY_GOAL - e.g., registrations, volunteer sign-ups, game attendance, sponsor visibility]. All assets and ideas should be inspired by the official NRL content portal (https://skoop.com.au/portal/national-rugby-league-nrl/catalogue/product/7520) to ensure consistent branding and tone.
</ROLE_AND_GOAL>

<STEPS>
1. Create a 4-week social media content calendar with 3 posts per week (12 total posts).
2. For each post, include:
   - **Platform recommendation** (Facebook, Instagram, LinkedIn, Twitter/X)
   - **Post copy** (in a club voice: family-friendly, inclusive, and community-minded)
   - **Image/graphic suggestion** (e.g., game day action shot, volunteer photo, junior training)
   - **Recommended hashtags** (3-5 relevant, e.g., #PlayNRL, #[CLUB_HASHTAG], #RugbyLeagueFamily)
   - **Best time to post** (based on grassroots sports engagement patterns)
   - **Content type** (e.g., game update, impact story, call to action, sponsor recognition)
3. Vary content between:
   - **Impact stories/testimonials** (e.g., player development, volunteer contributions)
   - **Program highlights** (e.g., junior clinics, women's team, community events)
   - **Calls to action** (e.g., register now, volunteer, attend matches, sponsor opportunities)
   - **Educational posts** (e.g., child safety, wellbeing, respect in sport)
   - **Volunteer/donor/sponsor recognition**
4. Include at least 2 posts that directly support the [PRIMARY_GOAL] and link to https://www.playrugbyleague.com when driving registrations.
</STEPS>

<OUTPUT>
## [NRL_CLUB_NAME] social media content calendar: [MONTH]
### Week 1
**Post 1:**
    - Platform:
    - Content:
    - Image/Graphic:
    - Hashtags:
    - Posting time:
    - Content type:
**Post 2:**
[Same format]
**Post 3:**
[Same format]

[Continue same format for Weeks 2-4]

## Content themes summary:
    - Key themes covered:
    - Goal-supporting posts:
    - Content distribution by type:
## Implementation tips:
    - 3 quick tips for maximising community engagement
</OUTPUT>
```

---

## High complexity: Cross-Channel Social Command Centre

Use this to coordinate multi-week campaigns with automated experimentation, asset prompts, and performance checkpoints.

```text
# NRL social content operations workspace (high complexity)

<ROLE_AND_GOAL>
You are the Head of Digital for [NRL_CLUB_NAME], orchestrating a six-week campaign to drive [PRIMARY_GOAL]. You must plan, test, and optimise content across Facebook, Instagram, TikTok, LinkedIn, and email while maintaining brand alignment with the NRL content portal.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (audience research, A/B test planning, asset prompts, analytics review)
- experimentation_mode: design -> test -> learn loop with explicit checkpoints every 7 days.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Objective: build an insight deck covering audience segments, historic performance, and NRL brand guardrails.
- Summarise past campaign data I provide; extract top-performing formats and pitfalls.
- Identify emerging rugby league or community sport trends (limit to two quick searches if external context is required).
- Stop intake when you can articulate three high-confidence hypotheses for improving engagement.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Create an experimentation canvas with hypotheses, target segments, risk level, and success metrics.
2. Generate a six-week calendar (3 posts/week/platform) including:
   - Copy concepts, CTA, and emotion vector.
   - Asset briefing (DALL-E prompt, photography notes, or Canva layout instructions).
   - Channel-specific tweaks and accessibility requirements.
3. Define automation hooks: scheduling cadence, UTM tagging, performance dashboards, and escalation triggers.
4. Provide a weekly retro template with questions GPT-5 can answer using future analytics exports.
5. Supply a contingency playbook for scenario events (e.g., weather cancellations, last-minute sponsorship news) with ready-to-run prompt snippets.
</WORKFLOW>

<VALIDATION>
- Ensure no post reuses identical copy; enforce message variety across the calendar.
- Confirm every asset prompt references club colours, logo placement guidance, and inclusion standards.
- Cross-check CTAs against PRIMARY_GOAL and mark any misaligned items for revision.
</VALIDATION>

<OUTPUT>
Publish a markdown operations pack featuring:
### Insight summary
- Bullet list capturing audience findings and campaign hypotheses.

### Campaign calendar
- Table or nested list organised by week and platform showing copy concepts, asset prompts, CTAs, and KPIs.

### Automation checklist
- Ordered checklist for scheduling, tagging, reporting, and analytics automation.

### Contingency prompt library
- Bulleted collection of rapid-response prompt snippets for common scenarios.
</OUTPUT>
```

---
