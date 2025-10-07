# Safety protocols and emergency procedures

**Category:** Administrators  
**Template type:** Policy and procedure documentation

**Collect these inputs before you start:**

- [NRL_CLUB/ORGANISATION_NAME]
- [EMERGENCY_TYPE - e.g., severe weather, medical emergencies, fire, crowd incidents]
- [LOCATION_TYPE - e.g., clubhouse, sports ground, training facility]
- [STAFF/VOLUNTEERS/PLAYERS/SPECTATORS]
- [VULNERABLE_POPULATIONS - e.g., juniors, people with disabilities]
- [SAFETY_CONCERN_TYPE - e.g., severe weather, medical emergencies, fire, facility hazards, crowd management]
- [TARGET_POPULATION - e.g., juniors, volunteers, spectators, people with disabilities]
- [FACILITY_TYPE - e.g., clubhouse, training field, sports ground]
- [SAFETY_CONCERN_TYPE]
- [FACILITY_SET - e.g., clubhouse, training field, stadium, community events]
- [REGULATORY_FRAMEWORK]


Document clear, actionable safety plans for any situation. Start with the low-complexity prompt for a standalone emergency guide, or use the medium-complexity workflow to produce a comprehensive protocol manual.

---

## Low complexity: Emergency procedure prompt

```text
Act as a safety protocol specialist for community sport organisations and create comprehensive emergency procedures for [NRL_CLUB/ORGANISATION_NAME] covering [EMERGENCY_TYPE - e.g., severe weather, medical emergencies, fire, crowd incidents] situations. Include step-by-step response protocols, volunteer/staff responsibilities, evacuation routes, and communication procedures. Search for current best practices in community sport and NRL safety protocols, and adapt them to our specific needs, considering our [LOCATION_TYPE - e.g., clubhouse, sports ground, training facility], typical number of [STAFF/VOLUNTEERS/PLAYERS/SPECTATORS] present, and any special considerations for [VULNERABLE_POPULATIONS - e.g., juniors, people with disabilities] we support. Format the document with clear headings, bulleted action steps, and include a one-page quick reference guide that can be posted throughout our facilities.
```

---

## Medium complexity: Comprehensive safety workflow

```text
# NRL club safety protocols and emergency procedures template (medium complexity)

<ROLE_AND_GOAL>
You are an experienced safety and emergency management specialist with expertise in developing clear, actionable safety protocols for community sport organisations. Your task is to create comprehensive safety procedures for [NRL_CLUB/ORGANISATION_NAME] that address [SAFETY_CONCERN_TYPE - e.g., severe weather, medical emergencies, fire, facility hazards, crowd management] while considering the unique needs of our [TARGET_POPULATION - e.g., juniors, volunteers, spectators, people with disabilities] and [FACILITY_TYPE - e.g., clubhouse, training field, sports ground].
</ROLE_AND_GOAL>

<STEPS>
1. Review the process steps and club context I provide.
2. Create a formal safety protocol document that includes:
   - Clear title and purpose statement
   - Scope and applicability (who must follow these procedures)
   - Roles and responsibilities for committee members, coaches, volunteers, and participants
   - Step-by-step emergency response procedures with decision points
   - Communication protocols during emergencies (e.g., PA announcements, SMS, emergency contacts)
   - Required safety equipment and resources (e.g., first aid kits, AEDs, evacuation maps)
   - Training requirements and frequency (e.g., first aid training, child safety briefings)
   - Documentation and reporting procedures (e.g., incident reports, notifications to the relevant State League or governing body)
   - Review and update schedule
3. Ensure all procedures comply with relevant local regulations, safeguarding policies, and community sport best practices.
4. Use plain language that can be understood by volunteers and staff with varying expertise levels.
</STEPS>

<OUTPUT>
Provide the complete safety protocol document with:
1. **Title:** [SAFETY_CONCERN_TYPE] safety protocol for [NRL_CLUB/ORGANISATION_NAME]
2. **Table of contents**
3. Clearly numbered sections with headers
4. Bulleted lists for action steps
5. Visual cues for critical information (using ** for emphasis)
6. Contact information placeholders (e.g., Safety Officer, Emergency Services)
7. Appendix with relevant forms or checklists (e.g., incident report form, emergency contact sheet, evacuation map template)
</OUTPUT>
```

---

## High complexity: Integrated safety management suite

Use this workflow when you must consolidate multi-venue protocols, regulatory change tracking, and training automation.

```text
# NRL safety and emergency orchestration template (high complexity)

<ROLE_AND_GOAL>
You are the Head of Safety for [NRL_CLUB/ORGANISATION_NAME], coordinating protocols for [FACILITY_SET - e.g., clubhouse, training field, stadium, community events]. You must harmonise procedures for [SAFETY_CONCERN_TYPE], ensure compliance with [REGULATORY_FRAMEWORK], and prepare assets for drills, training, and reporting.
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 8 (risk assessment, scenario planning, communication trees, compliance tracker)
- output_bundle: protocol manual, drill schedule, incident reporting forms, change log.
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: map hazards, response roles, and regulatory obligations per venue without redundancy.
- Summarise existing protocols, inspection reports, and incident logs; capture key risks with citations.
- Record dependencies (equipment, personnel, contractors) and availability constraints.
- Stop when each hazard has at least one mitigation and escalation path or is flagged as gap.
</CONTEXT_GATHERING>

<WORKFLOW>
1. Build a risk register by venue with probability, impact, controls, and responsible role.
2. Draft unified protocols with modular sections (pre-event checks, detection, response, recovery) and decision trees.
3. Generate drill and training calendar mapped to roles, frequency, and compliance deadlines.
4. Create communication cascade templates (PA, SMS, email, radio) with timing guidance.
5. Produce incident reporting toolkit: forms, data schema, escalation checklist, post-incident review template, and guidance on notifying the appropriate State League or governing body when required.
</WORKFLOW>

<VALIDATION>
- Ensure equipment and contact lists are current; flag outdated entries for update.
- Confirm protocols reference relevant legislation or NRL policies with citations.
- Verify accessibility: plain-language summaries, iconography suggestions, translations if required.
</VALIDATION>

<OUTPUT>
Publish a markdown safety dossier featuring:
### Risk register
- Table listing venue, hazard, rating, controls, and owner.

### Protocol manual
- Detailed instructions complete with decision trees and communication cues.

### Drill and training calendar
- Schedule outlining activity, audience, frequency, and responsible lead.

### Incident toolkit
- Forms, data schema, escalation checklist, and notification guidance ready for deployment.

### Change log
- Table capturing updates, rationale, and next review dates.
</OUTPUT>
```

---
