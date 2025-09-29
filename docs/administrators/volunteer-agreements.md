# Volunteer Agreements and Contracts

**Category:** Administrators  
**Template type:** Policy and procedure documentation

Draft volunteer agreements that balance legal protection with community warmth. Choose the low-complexity prompt for a quick comprehensive draft, or the medium-complexity workflow for structured, customisable documents.

---

## Low Complexity: Volunteer Agreement Prompt

```text
Act as a community sport legal document specialist and create a comprehensive volunteer agreement for [NRL_CLUB/ORGANISATION_NAME] that includes clear responsibilities, time commitments, confidentiality requirements, child safety expectations, and liability protections. Use [STATE/COUNTRY] legal standards for volunteer relationships and incorporate [NRL_CLUB/ORGANISATION_NAME]'s specific volunteer policies, ensuring the document is both legally sound and aligned with our club's values and mission of [MISSION_STATEMENT - e.g., growing participation, supporting volunteers, strengthening community spirit].
```

---

## Medium Complexity: Structured Agreement Workflow

```text
# NRL Volunteer Club Agreement and Contract Template Generator (Medium Complexity)

<ROLE_AND_GOAL>
You are a community sport legal document specialist with expertise in volunteer management and organisational policy development. Your task is to create a comprehensive, legally sound volunteer agreement for [NRL_CLUB/ORGANISATION_NAME] that clearly outlines expectations, responsibilities, and protections for both the club and its volunteers, while reflecting our values of community, respect, and integrity.
</ROLE_AND_GOAL>

<STEPS>
Create a volunteer agreement that includes:
1. Review the [CLUB_MISSION] and [VOLUNTEER_ROLE_DESCRIPTION] to understand the context.
2. Draft a complete volunteer agreement with all standard sections.
3. Ensure the document balances legal protection with a welcoming, community-aligned tone.
4. Include customisation notes for sections that may require local or state legal review or alignment with NRL Integrity and Safeguarding policies.
</STEPS>

<OUTPUT>
Provide the volunteer agreement as a complete document with:
1. **Club header** with [NRL_CLUB/ORGANISATION_NAME] and logo placeholder.
2. **Title:** Volunteer Agreement and Commitment
3. All standard sections including:
   - Introduction and mission statement
   - Volunteer responsibilities and commitments
   - Club responsibilities and commitments
   - Time commitment and scheduling
   - Confidentiality, data protection, and child safeguarding
   - Health and safety guidelines
   - Photo/media release
   - Liability and insurance coverage
   - Termination conditions
   - Signature blocks for volunteer and club representative
4. **Implementation guidance** for the Volunteer Coordinator (e.g., when to issue, how to store signed copies, renewal process).
</OUTPUT>
```

---

## High Complexity: Volunteer Contract Lifecycle Manager

Use this when you need GPT-5 to build agreement suites, jurisdictional variations, and onboarding automation.

```text
# Volunteer agreement orchestration template (High Complexity)

<ROLE_AND_GOAL>
You are the Legal and Governance Manager for [NRL_CLUB/ORGANISATION_NAME], responsible for delivering customised agreements for multiple volunteer roles (e.g., coaches, team managers, game day crew) across jurisdictions ([JURISDICTIONS]). Contracts must align with [MISSION_STATEMENT], NRL Integrity policies, and local regulations.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (jurisdiction comparison, clause library mapping, tone tailoring, checklist creation)
- version_control: maintain change log with clause IDs and rationale.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: integrate legal requirements, policy clauses, and role-specific expectations.
- Summarise applicable laws/regulations by jurisdiction and note mandatory clauses.
- Ingest existing templates and highlight reusable vs. obsolete clauses.
- Stop when each clause category (duty of care, safeguarding, confidentiality, termination) has authoritative sources or flagged gaps.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Assemble a clause matrix mapping requirements to volunteer roles and jurisdictions.
2. Generate master agreement plus annexes (role-specific schedules, code of conduct, safeguarding) with merge tags for custom data.
3. Create compliance checklist (documents to collect, training to complete, sign-off sequence) with automation hooks.
4. Draft communication plan: onboarding email series, acknowledgement reminders, and renewal notices.
5. Provide audit trail guidance (where to store, retention periods, review cadence).
</WORKFLOW>

<VALIDATION>
- Ensure each clause states legal basis or policy reference; flag unresolved legal review items.
- Confirm tone balances warmth with legal clarity; highlight sections that may require plain-language rewrite.
- Verify all merge tags have descriptions and fallback text.
</VALIDATION>

<OUTPUT>
Create a markdown agreement pack containing:
### Master Agreement
- Contract with placeholders, clause IDs, and guidance notes.

### Annexes
- Role-specific schedules and policy acknowledgements ready for attachment.

### Clause Matrix
- Table linking each clause to requirement, jurisdiction, source, and role coverage.

### Compliance Checklist
- Ordered steps with responsible owner and due date for document collection and training.

### Communication Plan
- Timeline of onboarding messages with key templates and calls to action.
</OUTPUT>
```

---
