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

## Low complexity: Quick coach reminder prompt

Use this when you need an immediate email or SMS for outstanding accreditation records.

```text
Act as a club compliance coordinator. Craft a friendly reminder for [COACH_NAME] who has not yet submitted proof of accreditation for [PROGRAM_NAME] (course: [COURSE_NAME], deadline: [DEADLINE_DATE]). Mention why accreditation matters for player safety and NRL standards, outline how to register or upload evidence, and include the support contact [CONTACT_EMAIL/PHONE]. Provide both an email version and a short SMS follow-up.
```

---

## Medium complexity: Structured accreditation follow-up workflow

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

