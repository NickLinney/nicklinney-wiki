---
title: Identity and Access Management Initiative - Systems-of-Record Review Meeting Minutes
description: First design working-session minutes for the IAM initiative systems-of-record review.
published: true
date: 2026-07-28T15:12:08.256Z
tags: nicklinney, identity-access-management, meeting-minutes, design
editor: markdown
dateCreated: 2026-07-28T15:12:08.256Z
---

# Identity and Access Management Initiative - Systems-of-Record Review Meeting Minutes

## Meeting Metadata

| Field | Value |
| --- | --- |
| Meeting ID | NLIAM-MTG-006 |
| Date | July 28, 2026 |
| Chair | Chief Information Officer |
| Recording Secretary | Technical Writer |
| Meeting Type | Design-phase systems-of-record review |
| Preceding Authority | `Design Phase Kickoff Cabinet Meeting Minutes` |

## Attendance

| Position | Status |
| --- | --- |
| Chief Information Officer | Present |
| Chief Information Security Officer | Present |
| PMO Director | Present |
| Director of Product Management | Present |
| Director of Information Technology | Present |
| Director of Information Security | Present |
| Vice President of Enterprise Architecture | Present |
| Director of DevOps | Present |
| Documentation Manager | Present |
| Technical Writer | Present |

## Agenda

1. Confirm the authoritative record categories required by the IAM initiative
2. Determine which records are governance publications, which are operational systems of record, and which are evidence stores
3. Surface cross-module dependency implications from the executive retrospective set
4. Establish systems-of-record decisions and open questions that must constrain the next design meetings

## Reference Set Considered

- `CVO Design Phase Kickoff Input`
- `Chief Vision Officer Retrospective`
- `Chief Operating Officer Retrospective`
- `Chief Information Officer Retrospective`
- `Chief Technology Officer Retrospective`
- `Chief Financial Officer Retrospective`
- `Chief Marketing Officer Retrospective`
- `Chief Product Officer Retrospective`
- `Chief Information Security Officer Retrospective`
- `Identity and Access Management Initiative Product Plan`
- `Identity and Access Management Initiative Project Plan`

## Working Framing

The chair opened by restating the CVO's kickoff message: IAM must become a cross-module service consumable at every enterprise layer, must support both human and agent access pathways, and must avoid shadow access designs by making approval, entitlement, and secrets pathways governable and reviewable. The CIO further stated that this meeting would not choose products. Its purpose was to determine what records must exist, where they must live, and which categories must never be conflated.

## Record Categories Reviewed

The cabinet reviewed the following candidate record categories:

1. identity principal registry for humans, agents, and service accounts
2. role catalog and role-to-module authority map
3. access policy and approval-rule definitions
4. access request, approval, grant, review, and revocation records
5. secrets inventory metadata and vault-control records
6. credential issuance, rotation, recovery, and exception records
7. audit, authentication, authorization, and privileged-action event logs
8. governance charters, standards, architectural decisions, and publication indexes

## Official Motions and Commentary

### Item 1 - Record Taxonomy for the IAM Initiative

Motion:

`Move that the IAM initiative adopt the eight reviewed record categories as the minimum canonical record taxonomy for design, with later implementation permitted to add subtypes but not remove categories without cabinet approval.`

Commentary:

- Chief Information Officer: supported the motion and stated that the CIO retrospective makes record taxonomy non-optional because evidence spine ambiguity is itself one of the enterprise's active problems.
- Chief Information Security Officer: supported the motion and clarified that security review depends on separating entitlement records, secrets-control records, and runtime evidence rather than treating them as one blended security archive.
- PMO Director: supported the motion and stated that a fixed taxonomy gives later design meetings a traceable frame and reduces the risk of hidden scope growth.
- Director of Product Management: supported the motion and added that the taxonomy is strong because it maps cleanly to user journeys for request, approval, issuance, use, review, and revocation.
- Director of Information Technology: supported the motion with caution and stated that the taxonomy must remain administratively workable for a young enterprise rather than becoming an abstract compliance shell.
- Director of Information Security: supported the motion and stressed that secrets inventory metadata must be explicitly separated from the secrets themselves so that governance records can be published without exposing protected material.
- Vice President of Enterprise Architecture: supported the motion and noted that the taxonomy also helps enforce boundary clarity between identity definition, access control, and runtime service behavior.
- Director of DevOps: supported the motion and added that agent and service-account pathways will fail later if machine records are not treated as first-class objects from the start.
- Documentation Manager: supported the motion and confirmed that the taxonomy is publishable as a crosswalk and can be maintained as a durable control index.

Disposition:

- Carried.

### Item 2 - Provisional System-of-Record Allocation by Record Category

Motion:

`Move that the cabinet adopt a provisional systems-of-record allocation under which governance publication records live in the wiki, operational secret values live only in approved vault systems, operational event evidence lives in runtime log stores, and IAM design work proceeds on the assumption that no single repository should be treated as the source of truth for every record category.`

Commentary:

- Chief Information Officer: supported the motion and stated that this aligns directly with the CIO retrospective warning against mistaking documentation neatness for full system realization.
- Chief Information Security Officer: supported the motion and clarified that the CISO retrospective requires vaults and evidence stores to remain distinct from publication surfaces if trust claims are to stay honest.
- PMO Director: supported the motion and stated that the allocation should be recorded as a design constraint so later tooling comparison does not quietly collapse the boundary model.
- Director of Product Management: supported the motion and added that the distinction improves product clarity because users need different experiences for requesting access, consuming access, and reviewing evidence.
- Director of Information Technology: dissented in part and warned that a fragmented record estate could become operationally brittle unless the initiative also defines an administrative lookup pattern and escalation path.
- Director of Information Security: supported the motion and responded that the dissent is valid operationally, but the security cost of flattening protected and publishable records into one store would be higher.
- Vice President of Enterprise Architecture: supported the motion and clarified that federated systems of record are acceptable so long as authority boundaries, ownership, and synchronization obligations are explicit.
- Director of DevOps: supported the motion and added that automation requires metadata discoverability, but not universal centralization; machine pathways can consume controlled APIs and records if they are well bounded.
- Documentation Manager: supported the motion and stated that the wiki should be treated as the canonical publication surface for governance and index records, not as the runtime home of secrets or log evidence.

Disposition:

- Carried, with the Director of Information Technology's caution entered into the record as a follow-up design requirement for administrative lookup and escalation pathways.

### Item 3 - Cross-Module Dependency Interpretation for Systems of Record

Motion:

`Move that the cabinet formally recognize `NickLinney.KnowledgeManagement`, `NickLinney.Modules`, `NickLinney.System`, `NickLinney.DataInfrastructure`, `NickLinney.DevOps`, and `NickLinney.Security` as the primary cross-module dependency surfaces for IAM systems-of-record design, with `NickLinney.Contracts` and `NickLinney.SoftwareDevelopment` treated as secondary dependency surfaces that shape control obligations and workflow adoption.`

Commentary:

- Chief Information Officer: supported the motion and stated that the CIO retrospective makes Knowledge Management, System, and DataInfrastructure unavoidable because record authority and evidence location sit in that portfolio.
- Chief Information Security Officer: supported the motion and clarified that Security and SecOps must shape the trust and review model even if the IAM module is not identical to the broader security portfolio.
- PMO Director: supported the motion and noted that distinguishing primary and secondary dependencies is useful because it keeps the initiative governable without pretending unrelated modules have no stake.
- Director of Product Management: supported the motion and added that SoftwareDevelopment matters because access workflows will only be real if they can be adopted by actual delivery pathways rather than remaining an executive control diagram.
- Director of Information Technology: supported the motion and stated that Operations, environment, and hosting concerns from the COO retrospective should be interpreted through System and DevOps dependency handling, not ignored.
- Director of Information Security: supported the motion and argued that Contracts must remain visible because interface obligations, API boundaries, and delegated approvals are all contract-like control surfaces even inside an internal enterprise.
- Vice President of Enterprise Architecture: supported the motion and added that the corrected CVO portfolio obligates the cabinet to preserve enterprise design coherence rather than optimizing only for one technical subsystem.
- Director of DevOps: supported the motion and clarified that DevOps is a primary dependency because service accounts, deployment credentials, and non-human entitlements are central to the CVO's agentic operating model.
- Documentation Manager: supported the motion and stated that the recognized dependency map will help Knowledge Management build navigable cross-links and requirement traceability between initiative artifacts and retrospective sources.

Disposition:

- Carried.

### Item 4 - Open Questions to Carry into the Next Design Meetings

Motion:

`Move that the cabinet carry forward four mandatory open questions to the remaining design meetings: what constitutes a principal, who is authorized to approve which access classes, which systems may hold machine credentials and under what controls, and what evidence must be retained to prove reviewable access governance across humans and agents.`

Commentary:

- Chief Information Officer: supported the motion and stated that these questions translate the evidence-spine problem into concrete decision work.
- Chief Information Security Officer: supported the motion and added that the question about principals must explicitly include service accounts, agents, and recovery pathways.
- PMO Director: supported the motion and stated that open questions are acceptable only because they are now bounded and assigned to later meetings rather than left as background ambiguity.
- Director of Product Management: supported the motion and clarified that each question corresponds to a future product interaction surface and therefore should guide the cabinet's user-journey thinking.
- Director of Information Technology: supported the motion and stressed that approver authority must stay realistic for current staffing levels and not assume an administrative workforce that does not exist.
- Director of Information Security: supported the motion and added that evidence retention criteria must distinguish between proof of control and sensitive operational payloads.
- Vice President of Enterprise Architecture: supported the motion and argued that the principal-definition question will also determine domain-boundary compatibility across future services.
- Director of DevOps: supported the motion and registered a caution that machine-credential design must not be deferred until the end, because automation constraints will otherwise distort the final control model.
- Documentation Manager: supported the motion and confirmed that the open questions can be turned into a traceability worksheet for the remaining meetings.

Disposition:

- Carried.

## Systems-of-Record Determinations

The cabinet determined the following:

1. The wiki is the canonical publication surface for IAM charters, decision records, meeting minutes, standards drafts, and navigational indexes, but not for live secrets or runtime security events.
2. Any future vault technology is expected to hold secret values and possibly associated policy objects, but the cabinet has not yet selected the technology stack.
3. Runtime evidence for authentication, authorization, privileged actions, and machine use must be expected to exist outside the wiki in operational log and audit surfaces.
4. IAM design must assume federated systems of record joined by explicit ownership, lookup, and review rules rather than one universal repository.
5. The next meeting, `RBAC Taxonomy Workshop`, must begin from the now-adopted record taxonomy and open-question set.

## Action Items

- Chief Information Officer: prepare the opening decision frame for the `RBAC Taxonomy Workshop`, anchored to principal classes and approval authority.
- Chief Information Security Officer: draft the trust-boundary considerations for human, agent, and service-account principal types.
- Director of Information Technology: propose an administrative lookup and escalation model so federated systems of record remain operable.
- Director of DevOps: prepare machine-identity and deployment-credential use cases for the next two design meetings.
- Documentation Manager: create a requirements-to-record-category crosswalk for cabinet use.
- Technical Writer: publish these minutes and update initiative navigation and registers with the Knowledge Manager.