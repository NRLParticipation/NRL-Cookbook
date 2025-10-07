# Staff handbook and policy manual templates

**Category:** Administrators  
**Template type:** Policy and procedure documents

**Collect these inputs before you start:**

- [ORGANISATION_NAME]
- [POLICY_AREA]
- [LOCATION]
- [DOCUMENT_TYPE]


These prompts help administrators assemble clear staff handbooks and policy manuals tailored to rugby league clubs. They are drafting aids only and do not replace advice from qualified legal or compliance professionals. Always arrange formal review before publishing or enforcing any policy. Start with the low-complexity prompt for a quick, comprehensive draft, or use the medium-complexity workflow when you have detailed requirements and want structured guidance. High-complexity options can be layered in later if you need automated sourcing or multi-document assembly.

---

## Low complexity: Policy manual draft prompt

Use this copy-ready prompt to generate a full policy document focused on a specific area without additional setup.

```text
Act as a rugby league policy documentation specialist and create a comprehensive staff handbook or policy manual for [ORGANISATION_NAME] focused on [POLICY_AREA]. Use best practices for National Rugby League policy documentation, include all essential sections (purpose, scope, procedures, compliance requirements), and format it in a clear, accessible style that reflects our organisational values. Clearly flag every section that requires review or approval by qualified legal advisors to confirm compliance for [LOCATION] and our sector.
```

---

## Medium complexity: Structured handbook workflow

Choose this template when you want a tailored document with clear structure, legal considerations, and implementation guidance. Gather the information requested before running the prompt.

```text
# Staff handbook and policy manual template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced sports and nonprofit policy documentation specialist with expertise in creating clear, practical handbooks and policy manuals for community sport organisations. Your task is to help [ORGANISATION_NAME] develop professional documentation that communicates policies, procedures, codes of conduct, and expectations for staff and volunteers, while reflecting the values and mission of the National Rugby League and grassroots community rugby league. Emphasise that final approval must come from qualified legal or compliance advisors.
</ROLE_AND_GOAL>

<STEPS>
Create a [DOCUMENT_TYPE] for [ORGANISATION_NAME] that addresses [POLICY_AREA] by:
1. Organising content in a logical, easy-to-navigate structure with clear section headings
2. Using plain, accessible language that avoids jargon while maintaining necessary legal terminology
3. Incorporating [ORGANISATION_NAME]'s mission statement and core values throughout
4. Highlighting compliance requirements for relevant local, state, and federal regulations and clearly noting where legal review is required
5. Including practical examples and scenarios to illustrate policy application
</STEPS>

<OUTPUT>
Provide the completed documentation with:
1. A table of contents with hyperlinked sections
2. Clearly formatted policies with numbered sections and subsections
3. Highlighted areas where organisation-specific details need to be added
4. Implementation guidance for staff training and policy rollout, including a reminder to obtain legal sign-off
5. Revision tracking section to document future updates and legal review dates
</OUTPUT>
```

---

## High complexity: Policy suite automation workspace

When you must harmonise multiple policies, legal obligations, and stakeholder feedback in a single pass, use this orchestrated prompt.

```text
# NRL policy manual automation flow (high complexity)

<ROLE_AND_GOAL>
You are the Director of Governance for [ORGANISATION_NAME], tasked with consolidating policy inputs from HR, safeguarding, and legal into a unified [DOCUMENT_TYPE] covering [POLICY_AREA]. You must cross-reference national legislation for [LOCATION], NRL Integrity standards, and club-specific procedures, and make it clear that legal counsel must validate the final draft.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 evidence synthesis passes (legislation lookup, cross-policy comparison, stakeholder feedback)
- response_style: structured, citation-rich, ready for policy management system import.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Objective: build a policy knowledge map without reading redundancies.
- Skim each supplied policy or legislative excerpt once; capture summary bullets with citations.
- Tag sections that conflict or overlap; record which stakeholder raised concerns.
- Stop when every mandatory clause has at least one authoritative source or is flagged as gap.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Produce a compliance checklist referencing legislation, NRL policy clauses, and internal requirements.
2. Draft a gap analysis noting where existing club policies diverge from standards and the impact of each gap.
3. Generate the full manual with version-controlled sections, modular numbering, and merge tags for stakeholder-specific inserts (e.g., staff vs. volunteer).
4. Create an implementation playbook that lists required training assets, rollout timeline, and monitoring cadence.
5. Suggest automation hooks (e.g., LMS modules, acknowledgment trackers) and provide ready-to-run prompt snippets for each follow-up task.
</WORKFLOW>

<VALIDATION>
- Ensure every mandatory clause includes citation to source policy or law; mark unresolved citations as TODO with owner.
- Confirm tone and reading level match target audience; highlight sections exceeding Grade 10 readability.
- Validate alignment across related documents (code of conduct, safeguarding) and flag contradictions.
</VALIDATION>

<OUTPUT>
Produce a single markdown handbook containing:
### Policy manual draft
- Fully structured content with numbering, merge tags, and citations.

### Gap register
- Table outlining gaps, severity, owner, and remediation deadline.

### Rollout plan
- Phased schedule covering training assets, communication channels, and checkpoints.

### Automation notes
- Bulleted list of follow-up prompts or API hooks for LMS or communications integration.
</OUTPUT>
```

---
