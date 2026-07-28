---
title: Identity and Access Management Initiative - RBAC Taxonomy Workshop Minutes
description: Design working-session minutes for the IAM initiative RBAC taxonomy workshop.
published: true
date: 2026-07-28T15:18:52.270Z
tags: nicklinney, identity-access-management, meeting-minutes, design
editor: markdown
dateCreated: 2026-07-28T15:18:52.270Z
---

# Identity and Access Management Initiative - RBAC Taxonomy Workshop Minutes

## Meeting Metadata

| Field | Value |
| --- | --- |
| Meeting ID | NLIAM-MTG-007 |
| Date | July 28, 2026 |
| Chair | Chief Information Security Officer |
| Recording Secretary | Technical Writer |
| Meeting Type | Design-phase RBAC taxonomy workshop |
| Preceding Authority | `Systems-of-Record Review Meeting Minutes` |

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

1. Define principal classes for the IAM operating model
2. Establish role families and approval authorities
3. Determine how human, agent, and service-account pathways differ
4. Set constraints for the future secrets and vault design review

## Reference Set Considered

- `CVO Design Phase Kickoff Input`
- `Systems-of-Record Review Meeting Minutes`
- `Chief Vision Officer Retrospective`
- `Chief Information Officer Retrospective`
- `Chief Technology Officer Retrospective`
- `Chief Information Security Officer Retrospective`
- `Chief Product Officer Retrospective`
- `Chief Operating Officer Retrospective`

## Working Framing

The chair opened by stating that the IAM initiative cannot credibly evaluate technologies until the cabinet first decides what kinds of principals exist, how authority is delegated, and which approval paths must govern access for both humans and machines. The CVO's kickoff requirement for trusted authentication, federated access, access requests, and key retrieval at every enterprise layer was treated as the controlling design condition.

## Principal Classes Reviewed

The cabinet reviewed the following principal classes:

1. executive human principals
2. operational human principals
3. privileged administrative principals
4. agent principals
5. service-account principals
6. emergency and recovery principals

## Official Motions and Commentary

### Item 1 - Minimum Principal Taxonomy

Motion:

`Move that the IAM initiative adopt the six reviewed principal classes as the minimum enterprise principal taxonomy for the initial IAM design package.`

Commentary:

- Chief Information Officer: supported the motion and stated that system-of-record clarity requires the enterprise to distinguish people from machine actors rather than treating both as generic account objects.
- Chief Information Security Officer: supported the motion and clarified that emergency and recovery identities must be explicit because otherwise exceptional access will become invisible or informal.
- PMO Director: supported the motion and stated that a fixed principal taxonomy is necessary for scoped approvals and for preventing later architectural drift.
- Director of Product Management: supported the motion and added that separate principal classes are essential for designing different request and review experiences instead of one confusing universal workflow.
- Director of Information Technology: supported the motion with caution and stated that privileged administrative principals should be narrow and operationally realistic so the enterprise does not create an unusable separation model.
- Director of Information Security: supported the motion and stressed that agent principals must never be treated as aliases for their sponsoring humans because review obligations differ materially.
- Vice President of Enterprise Architecture: supported the motion and noted that the taxonomy usefully separates authority domains without implying a separate platform for every actor type.
- Director of DevOps: supported the motion and added that service-account principals need to remain first-class because deployment pathways and inter-service connectivity cannot be forced through human-login assumptions.
- Documentation Manager: supported the motion and confirmed that the taxonomy can be published as a stable reference object for later role and approval artifacts.

Disposition:

- Carried.

### Item 2 - Role Family Model

Motion:

`Move that the cabinet establish a role-family model composed of enterprise governance roles, module ownership roles, operational execution roles, security and trust roles, agent execution roles, and platform integration roles, with named roles to be defined beneath those families in later implementation planning.`

Commentary:

- Chief Information Officer: supported the motion and stated that role families provide enough control structure for design without pretending that the enterprise has already named every operational role.
- Chief Information Security Officer: supported the motion and clarified that security and trust roles must remain separately reviewable even when one individual may temporarily hold multiple duties.
- PMO Director: supported the motion and stated that the family model is a practical compromise between premature detail and dangerous vagueness.
- Director of Product Management: supported the motion and added that role families will make it easier to map future user stories and service workflows.
- Director of Information Technology: dissented in part and warned that too many theoretical role families could outpace the enterprise's current staffing footprint if not paired with consolidation rules.
- Director of Information Security: supported the motion and responded that the concern is valid, but collapsing roles too early would hide segregation-of-duties requirements before they can be consciously waived.
- Vice President of Enterprise Architecture: supported the motion and noted that role families also help preserve cross-module coherence because module ownership and platform integration are different design concerns.
- Director of DevOps: supported the motion and added that platform integration roles are necessary so pipeline, secret, and deployment permissions are not improvised later.
- Documentation Manager: supported the motion and stated that the family model can be published with an explicit note distinguishing conceptual families from currently staffed seats.

Disposition:

- Carried, with the Director of Information Technology's caution entered as a requirement that later role definitions include consolidation notes for the current enterprise scale.

### Item 3 - Approval Authority Model

Motion:

`Move that the cabinet adopt a provisional approval model in which module owners approve standard module access, security authorities approve privileged and trust-sensitive access, platform owners approve infrastructure-integrated machine access, and emergency access requires both post-use review and retained exception evidence.`

Commentary:

- Chief Information Officer: supported the motion and stated that module ownership must become an active control object if the CVO's module-coherence concerns are to be addressed honestly.
- Chief Information Security Officer: supported the motion and clarified that privileged and trust-sensitive access should never rely solely on line ownership because the trust boundary extends beyond delivery convenience.
- PMO Director: supported the motion and stated that the approval model is bounded enough to govern now while still leaving space for future refinement by named role.
- Director of Product Management: supported the motion and added that the model aligns well with the expected request paths for ordinary access, elevated access, and exceptional access.
- Director of Information Technology: supported the motion and stressed that operational turnaround time must remain part of the design so approval chains do not become performative bottlenecks.
- Director of Information Security: supported the motion and added that emergency access is acceptable only if exception evidence is retained and reviewed as a normal governance requirement.
- Vice President of Enterprise Architecture: supported the motion and noted that platform-integrated machine access should be approved with awareness of system boundary effects, not just tool ownership.
- Director of DevOps: supported the motion and clarified that machine access approvals must include intended usage scope, not just static grant decisions, so automation permissions remain reviewable.
- Documentation Manager: supported the motion and confirmed that the model can be captured as a simple approval matrix in future artifacts.

Disposition:

- Carried.

### Item 4 - Constraints for the Secrets and Vault Design Review

Motion:

`Move that the next design meeting treat human secret storage, machine credential issuance, privileged administrative recovery, and audit evidence as related but distinct control surfaces, and prohibit any future design from assuming that one mechanism should own all four by default.`

Commentary:

- Chief Information Officer: supported the motion and stated that the systems-of-record review already showed that one-store thinking would blur authority and evidence boundaries.
- Chief Information Security Officer: supported the motion and clarified that the initiative should expect different controls for human convenience secrets, machine credentials, recovery artifacts, and audit evidence.
- PMO Director: supported the motion and stated that the constraint will make the next meeting more disciplined because candidates can be evaluated against clearly separated control surfaces.
- Director of Product Management: supported the motion and added that separating control surfaces will help maintain usable workflows rather than forcing every actor through the most restrictive path.
- Director of Information Technology: supported the motion and stated that operational administration will be safer if recovery procedures are deliberately designed instead of appended later.
- Director of Information Security: supported the motion and stressed that machine credential issuance must be treated as a lifecycle process, not as a static storage problem.
- Vice President of Enterprise Architecture: supported the motion and noted that this constraint also matches the CVO's call for domain-boundary compatibility.
- Director of DevOps: supported the motion and cautioned that any candidate unable to handle machine-credential lifecycle cleanly should be considered a poor fit for the enterprise's agentic direction.
- Documentation Manager: supported the motion and confirmed that the separated control surfaces can become headings in the architecture comparison package.

Disposition:

- Carried.

## RBAC Determinations

The cabinet determined the following:

1. The IAM design package will explicitly distinguish human, agent, service-account, privileged administrative, and emergency principal types.
2. Role families will be used before detailed named roles are finalized, so the design remains bounded but actionable.
3. Module ownership, security approval, and platform approval are separate approval authorities that must remain visible in later workflow design.
4. The secrets and vault review must evaluate separate control surfaces rather than searching for a single undifferentiated tool answer.

## Action Items

- Chief Information Security Officer: prepare the control-surface evaluation frame for the `Secrets and Vault Design Review`.
- Chief Information Officer: prepare the module-owner approval assumptions to be used in future access matrices.
- Director of Information Technology: draft a current-scale consolidation note for role families and approver duties.
- Director of DevOps: document machine-credential lifecycle needs for deployment, agent execution, and inter-service connectivity.
- Documentation Manager: prepare a draft approval-matrix outline for cabinet review.
- Technical Writer: publish these minutes and update the design-phase navigation with the Knowledge Manager.