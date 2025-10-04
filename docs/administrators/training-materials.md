# Training materials and workshop activities

**Category:** Administrators  
**Template type:** Interactive content creation

**Collect these inputs before you start:**

- [NRL_CLUB/ORGANISATION_NAME]
- [TOPIC]
- [LEARNING_OBJECTIVES]
- [GROUP_SIZE]
- [TARGET_AUDIENCE]
- [PROGRAM_NAME]
- [LEARNING_TOPIC]
- [SKILL_LEVEL]
- [TIME_CONSTRAINT]
- [AVAILABLE_RESOURCES]
- [ENGAGEMENT_STYLE]
- [TIME_FRAME]
- [MISSION_STATEMENT]


Design engaging workshops that build skills and enthusiasm. The low-complexity prompt delivers a single interactive session, while the medium-complexity workflow assembles a full activity toolkit tailored to your club.

---

## Low complexity: Workshop Activity Prompt

```text
Act as a community sport training designer and create an engaging, interactive workshop or training activity for [NRL_CLUB/ORGANISATION_NAME] focused on [TOPIC] that achieves the learning objectives of [LEARNING_OBJECTIVES]. Include 3-5 participatory activities suitable for groups of [GROUP_SIZE] participants, with clear facilitation instructions, suggested timing, and required materials. Make the content accessible for [TARGET_AUDIENCE] (e.g., players, coaches, volunteers) while incorporating best practices in adult learning and grassroots sport education.
```

---

## Medium complexity: Structured Workshop Workflow

```text
# NRL club workshop activity generator (medium complexity)

<ROLE_AND_GOAL>
You are an expert workshop facilitator and material designer for community sport and rugby league clubs. Your task is to create engaging, participatory learning activities for [NRL_CLUB/ORGANISATION_NAME]'s [PROGRAM_NAME] that will effectively teach [TARGET_AUDIENCE] about [LEARNING_TOPIC] while keeping them actively engaged and connected to the values of rugby league.
</ROLE_AND_GOAL>

<STEPS>
Create a set of interactive workshop activities that:
1. Address the specific learning objectives: [LEARNING_OBJECTIVES].
2. Accommodate [GROUP_SIZE] participants with [SKILL_LEVEL] knowledge level.
3. Can be completed within [TIME_CONSTRAINT] minutes.
4. Use practical, minimal resources: [AVAILABLE_RESOURCES].
5. Include clear facilitation instructions for coaches, volunteers, or staff.
6. Incorporate [ENGAGEMENT_STYLE] learning approaches (e.g., hands-on drills, team discussions, role-play, problem-solving).
</STEPS>

<OUTPUT>
For each activity, provide:
1. **Activity title** - Brief, descriptive name.
2. **Learning objective** - Which specific objective this addresses.
3. **Duration** - Estimated time needed.
4. **Materials required** - List all needed resources.
5. **Setup instructions** - How to prepare the space or materials.
6. **Participant instructions** - Clear, step-by-step guidance.
7. **Facilitation notes** - Tips for the facilitator (e.g., adapt for age group, link to rugby values).
8. **Reflection questions** - Two or three questions to reinforce learning.
9. **Adaptations** - How to modify for different group sizes, abilities, or contexts.
</OUTPUT>
```

---

## High complexity: Multi-Cohort Training Lab

Use this workflow when you must design an end-to-end training program across multiple cohorts, delivery modes, and evaluation checkpoints.

```text
# NRL training material orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Learning and Development Director for [NRL_CLUB/ORGANISATION_NAME], tasked with building a comprehensive program on [LEARNING_TOPIC] for [TARGET_AUDIENCE] spanning [TIME_FRAME]. The material must blend in-person workshops, digital modules, and on-field practice while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (needs analysis, competency mapping, session design, assessment, iteration planning)
- delivery_bundle: facilitator guides, participant journeys, assessment strategy, improvement loop.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: capture competency gaps, resource constraints, and prior feedback without exhaustive reading.
- Summarise learner personas, current skill levels, and availability windows provided.
- Review past training evaluations to identify strengths/gaps.
- Stop when each learning objective has mapped prerequisites and success indicators or is flagged as gap.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Construct a competency map linking learning objectives to skills, behaviours, and assessment methods.
2. Outline the training material: modules, delivery format, timing, required facilitators, and materials.
3. Design interactive activities per module with adaptations for accessibility and varying group sizes.
4. Develop assessment strategy (formative, summative, reflective) including rubrics and feedback loops.
5. Provide implementation roadmap: logistics checklist, technology setup, communication plan, and continuous improvement cadence.
</WORKFLOW>

<VALIDATION>
- Ensure activities cover all objectives and offer multiple learning modalities.
- Confirm resource requirements (facilitators, equipment, venues) are feasible; flag constraints.
- Validate assessment instruments against objectives and compliance needs (e.g., safeguarding).
</VALIDATION>

<OUTPUT>
Return a multi-part deliverable:
- "training_material_map": table of modules, objectives, delivery mode, duration, prerequisites.
- "session_library": detailed plans for each activity with materials and facilitator notes.
- "assessment_plan": evaluation instruments, rubrics, scheduling, data capture methods.
- "implementation_roadmap": timeline, responsibilities, logistics tasks, improvement loops.
</OUTPUT>
```

---
