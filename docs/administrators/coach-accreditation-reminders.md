# Coach accreditation reminder templates

**Category:** Administrators  
**Template type:** Compliance communications

**Collect these inputs before you start:**

- [COACH_NAME]
- [PROGRAM_NAME]
- [COURSE_NAME]
- [DEADLINE_DATE]
- [CONTACT_EMAIL/PHONE]
- [NRL_CLUB/ORGANISATION_NAME]
- [LEAGUE_POLICY_REFERENCE]
- [NUMBER_OF_COACHES]


Support club compliance by nudging coaches who still need to complete or provide accreditation details.

---

## Low complexity: quick coach reminder prompt

Use this when you need an immediate email or SMS for outstanding accreditation records.

```text
Act as a club compliance coordinator. Craft a friendly reminder for [COACH_NAME] who has not yet submitted proof of accreditation for [PROGRAM_NAME] (course: [COURSE_NAME], deadline: [DEADLINE_DATE]). Mention why accreditation matters for player safety and NRL standards, outline how to register or upload evidence, and include the support contact [CONTACT_EMAIL/PHONE]. Provide both an email version and a short SMS follow-up.
```

---

## Medium complexity: structured accreditation follow-up workflow

Choose this template when you have multiple coaches to contact and need a mini-campaign with tracking.

```text
# Coach accreditation follow-up template (medium complexity)

<ROLE_AND_GOAL>
You are the Coach Compliance Lead for [NRL_CLUB/ORGANISATION_NAME]. Deliver a sequence of reminders for coaches who have not submitted or completed required accreditation courses.
</ROLE_AND_GOAL>

<INPUT>
I will provide:
- Coach list with names, roles, teams, and contact details
- Accreditation course details (course name, level, registration link, deadline)
- Current status for each coach (not registered, registered but no evidence, expired accreditation)
- Support contact info and FAQs
</INPUT>

<STEPS>
1. Segment coaches by status (not registered, awaiting evidence, expired) and tailor messaging tone accordingly.
2. Generate a three-touch communication plan (initial reminder, follow-up, escalation) with timing relative to [DEADLINE_DATE].
3. Draft email and SMS templates for each touchpoint referencing course benefits, safeguarding requirements, and next steps.
4. Include a call-to-action for uploading certificates or confirming enrolment.
5. Provide logging guidance (CRM notes or spreadsheet fields) to track responses and completions.
</STEPS>

<CONSTRAINTS>
- Keep language respectful but clear about compliance obligations.
- Reference NRL accreditation expectations and player welfare.
- Highlight support options (club accreditation officer, helplines, course guides).
</CONSTRAINTS>

<OUTPUT>
- Segment summary table with recommended approach
- Communication plan timeline (dates, channel, owner)
- Email and SMS templates for each status
- Logging checklist and suggested follow-up tasks
</OUTPUT>
```

---

## High complexity: accreditation compliance orchestrator

Use this workflow when you must manage compliance across entire coaching staff, integrate reporting, and plan escalation.

```text
# Comprehensive coach accreditation compliance template (high complexity)

<ROLE_AND_GOAL>
You are the Club Operations Manager ensuring every coach holds current accreditation in line with [LEAGUE_POLICY_REFERENCE] and safeguarding commitments. Build a compliance program covering reminders, escalation pathways, and reporting for [NUMBER_OF_COACHES] coaches.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 6 (segmentation, escalation design, reporting templates)
- decision_mode: assess -> communicate -> escalate
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: gather the compliance data needed for accurate follow-up.
- Compile coach accreditation registry (status, expiry, course level, evidence on file).
- Capture deadlines from governing body and club policies.
- Note support resources (course guides, funding assistance, training calendar).
- Record previous communications or coaching director notes.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Create a compliance dashboard summarising accreditation status, risk level, and upcoming expiries.
2. Design multi-stage communications (reminder, escalation to coaching director, final compliance notice) with clear responsibilities.
3. Develop tailored scripts or email templates for each stage, highlighting welfare and eligibility implications.
4. Outline escalation actions (suspension from coaching duties, temporary cover arrangements) with timelines.
5. Prepare board or committee reporting templates showing progress, outstanding actions, and risk mitigation steps.
6. Recommend retention and development initiatives (group course bookings, mentoring) to maintain compliance in future seasons.

<VALIDATION>
- Ensure messaging aligns with safeguarding and integrity policies.
- Confirm escalation steps match club constitution or league rules.
- Flag gaps in data or required approvals before issuing notices.

<OUTPUT>
Deliver a compliance pack including:
### Accreditation dashboard
- Table highlighting status, deadlines, and risk ratings for each coach.

### Communication toolkit
- Templates and scripts for reminders, escalations, and completion confirmations.

### Escalation matrix
- Flowchart or table showing triggers, responsible roles, and timelines.

### Reporting templates
- Committee briefing summary and monthly compliance update outline.
```

---
