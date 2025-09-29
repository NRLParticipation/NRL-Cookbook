# Training Materials and Onboarding Guides

**Category:** Administrators  
**Template type:** Policy and procedure documents

Capture club knowledge in reusable guides that make onboarding easy. The low-complexity prompt creates a comprehensive how-to, while the medium-complexity workflow turns detailed inputs into formal documentation.

---

## Low Complexity: Procedure Guide Builder

```text
Act as a community sport documentation specialist, create a comprehensive [PROCEDURE_TYPE] guide for [NRL_CLUB/ORGANISATION_NAME] that explains the step-by-step process for [PROCESS_NAME - e.g., game day setup, player registration, volunteer onboarding, canteen operations]. Include required materials, key stakeholders (e.g., coaches, managers, volunteers), compliance requirements (e.g., NRL Integrity and Safeguarding policies, Working with Children/Vulnerable People checks), and common troubleshooting tips. Format this as a clear, scannable document with numbered steps, callout boxes for important notes, and references to any relevant club or NRL policies that impact this procedure, making it suitable for both new volunteers onboarding and as an ongoing reference resource for the committee.
```

---

## Medium Complexity: Formal Training Document Workflow

```text
# NRL Club training and onboarding documentation template (Medium Complexity)

<ROLE_AND_GOAL>
You are an experienced community sport training specialist who excels at creating clear, accessible documentation for [NRL_CLUB_NAME]. Your task is to create a comprehensive [DOCUMENT_TYPE - e.g., Volunteer Onboarding Guide, Game Day Operations Manual, Registration Process Guide] for [PROCESS_NAME] that will help [TARGET_AUDIENCE - e.g., new volunteers, team managers, junior coaches] understand and follow the correct procedures.
</ROLE_AND_GOAL>

<STEPS>
1. Review the process steps and club context I provide.
2. Organise the information into a logical, step-by-step format.
3. Include necessary background information, purpose, and scope (e.g., how this supports club operations or NRL requirements).
4. Add relevant compliance requirements or best practices (e.g., NRL Safeguarding policies, Working with Children/Vulnerable People checks).
5. Incorporate [NRL_CLUB_NAME]'s terminology, culture, and values to reflect the spirit of grassroots rugby league.
6. Create a document that balances thoroughness with accessibility so it is useful for both onboarding and as an ongoing reference.
</STEPS>

<OUTPUT>
Create a formal [DOCUMENT_TYPE] with these sections:
1. **Purpose and scope** - Brief overview of why this process exists and who it applies to
2. **Roles and responsibilities** - Who is involved and what they are accountable for (e.g., coaches, managers, volunteers)
3. **Required resources** - Tools, systems, or materials needed (e.g., NRL registration system, equipment lists)
4. **Procedure** - Clearly numbered steps with any decision points noted
5. **Troubleshooting** - Common issues and their solutions
6. **Related policies or references** - Links to other relevant NRL or club documentation
7. **Version history** - Document creation date and revision information
</OUTPUT>
```

---

## High Complexity: Knowledge Base Automation Flow

Use this when you need to consolidate process notes, compliance requirements, and multimedia resources into a live handbook.

```text
# NRL club training knowledge base template (High Complexity)

<ROLE_AND_GOAL>
You are the Operations Enablement Lead for [NRL_CLUB/ORGANISATION_NAME], building a modular [DOCUMENT_TYPE] for [PROCESS_NAME]. Integrate SOPs, compliance mandates, and learner feedback while preparing assets for LMS upload and printable quick guides.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (process synthesis, compliance mapping, role-specific tailoring, validation)
- output_mode: multi-document bundle with both narrative and checklist artifacts.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: map all tasks, actors, and decision points without duplicating content.
- Skim provided SOPs, policy excerpts, and training feedback; capture bullet summaries with citations.
- Identify where process steps diverge for different roles or venues.
- Stop once you can explain the full flow end-to-end and list outstanding questions.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a process architecture diagram description (stages, decision gates, responsible roles).
2. Draft instructor guide, participant workbook, and quick-reference checklist variants.
3. Generate equipment/materials Bill of Materials with storage location and pre-event checks.
4. Create assessment assets: knowledge check questions, practical evaluation rubric, and reflection prompts.
5. Outline change-management plan including rollout timeline, training sessions, and feedback loops.
</WORKFLOW>

<VALIDATION>
- Ensure each step indicates responsible role and compliance references.
- Confirm prerequisites (certifications, approvals) are emphasised before procedure steps.
- Provide accessibility guidance (formatting, alternative text, translations) for all assets.
</VALIDATION>

<OUTPUT>
Assemble a markdown training bundle containing:
### Instructor Guide
- Facilitator notes with timing, key messages, and setup tips.

### Participant Pack
- Learner-friendly instructions and practice activities.

### Operational Checklists
- Role-specific numbered lists for pre-, during-, and post-activity steps.

### Assessment Assets
- Question bank, rubrics, and reflection prompts ready for use.

### Change Management Plan
- Rollout schedule with owners, milestones, and feedback mechanisms.
</OUTPUT>
```

---
