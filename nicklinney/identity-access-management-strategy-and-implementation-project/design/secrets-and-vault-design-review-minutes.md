---
title: Identity and Access Management Initiative - Secrets and Vault Design Review Minutes
description: Design working-session minutes for the IAM initiative secrets and vault design review.
published: true
date: 2026-07-28T15:19:14.676Z
tags: nicklinney, identity-access-management, meeting-minutes, design
editor: markdown
dateCreated: 2026-07-28T15:19:14.676Z
---

# Identity and Access Management Initiative - Secrets and Vault Design Review Minutes

## Meeting Metadata

| Field | Value |
| --- | --- |
| Meeting ID | NLIAM-MTG-008 |
| Date | July 28, 2026 |
| Chair | Director of Information Security |
| Recording Secretary | Technical Writer |
| Meeting Type | Design-phase secrets and vault design review |
| Preceding Authority | `RBAC Taxonomy Workshop Minutes` |

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

1. Interpret the CVO's candidate-architecture prompt for secrets and directory capabilities
2. Compare control-surface needs for human secrets, machine credentials, directory-backed identity, and auditability
3. Establish a provisional architecture stance without prematurely selecting a final stack
4. Set publication-ready decision points for the current design package

## Reference Set Considered

- `CVO Design Phase Kickoff Input`
- `Systems-of-Record Review Meeting Minutes`
- `RBAC Taxonomy Workshop Minutes`
- `Chief Vision Officer Retrospective`
- `Chief Information Officer Retrospective`
- `Chief Technology Officer Retrospective`
- `Chief Information Security Officer Retrospective`
- `Chief Operating Officer Retrospective`
- `Chief Product Officer Retrospective`

## Working Framing

The chair opened by reading the CVO's recommendation that candidate architectures begin from proven systems rather than a not-invented-here approach, and specifically cited the suggested starting point of OpenLDAP combined with one of OpenBao, Vaultwarden, or Psono. The chair emphasized that this meeting would not lock a procurement or deployment decision. Its purpose was to determine what the cabinet expects a suitable stack pattern to do and which candidate directions remain credible after the prior meetings.

## Control Surfaces Reviewed

The cabinet reviewed four distinct control surfaces:

1. directory-backed identity and group authority
2. human-managed secret storage and sharing
3. machine credential issuance, storage, and rotation
4. audit, exception, and recovery evidence

## Official Motions and Commentary

### Item 1 - Architecture Pattern Separation

Motion:

`Move that the cabinet adopt a provisional architecture stance in which directory-backed identity authority and vault-backed secret control are treated as separate but integrated service domains, rather than assuming one product should serve as the full IAM control plane by itself.`

Commentary:

- Chief Information Officer: supported the motion and stated that the systems-of-record work already showed why publication, identity, secret control, and runtime evidence should not be collapsed into one repository.
- Chief Information Security Officer: supported the motion and clarified that separation improves trust-boundary clarity and reduces the risk of overstating one tool's control surface.
- PMO Director: supported the motion and stated that a pattern decision is useful here because it narrows later comparison work without prematurely making a product commitment.
- Director of Product Management: supported the motion and added that separate but integrated domains can still present coherent workflows if the approval and retrieval journeys are designed intentionally.
- Director of Information Technology: supported the motion and warned that the integration burden must remain proportionate to current operational capacity.
- Director of Information Security: supported the motion and stressed that secret-control depth and directory authority are related concerns, but they are not functionally identical.
- Vice President of Enterprise Architecture: supported the motion and noted that this separation is also the most compatible with the CVO's domain-boundary concerns.
- Director of DevOps: supported the motion and added that machine credential use cases are better served when secret lifecycles are designed independently of human authentication workflows.
- Documentation Manager: supported the motion and confirmed that this stance creates a clear comparison frame for future architecture notes.

Disposition:

- Carried.

### Item 2 - Candidate Direction Retention

Motion:

`Move that the cabinet retain a directory-plus-vault comparison pattern as the leading design direction, with OpenLDAP remaining an acceptable directory starting point and OpenBao, Vaultwarden, and Psono retained only as candidate components whose suitability depends on how well they address the distinct human-secret, machine-credential, and reviewability requirements already adopted.`

Commentary:

- Chief Information Officer: supported the motion and stated that it honors the CVO's suggestion without converting an executive prompt into a predetermined stack decision.
- Chief Information Security Officer: supported the motion and clarified that candidate retention should be evidence-led and must include security reviewability, recovery handling, and administrative safety.
- PMO Director: supported the motion and stated that retaining candidates rather than selecting one now keeps the phase disciplined and auditable.
- Director of Product Management: supported the motion and added that candidate evaluation should include how clearly each direction can support access request, approval, retrieval, and revocation journeys.
- Director of Information Technology: supported the motion with caution and noted that administrative burden, hosting practicality, and backup or recovery expectations should be explicit evaluation criteria.
- Director of Information Security: supported the motion and argued that any candidate centered primarily on human secret sharing should not automatically be assumed sufficient for machine credential governance.
- Vice President of Enterprise Architecture: supported the motion and stated that the motion is strong because it preserves stack optionality while making the service-domain pattern explicit.
- Director of DevOps: supported the motion and registered a caution that the machine-credential and IaC pathways should be weighted more heavily than convenience-only storage patterns.
- Documentation Manager: supported the motion and confirmed that the retained-candidate list can be published with an explicit note that no final selection has been made.

Disposition:

- Carried.

### Item 3 - Evaluation Criteria for Future Technology Comparison

Motion:

`Move that the cabinet adopt the following minimum evaluation criteria for future technology comparison: principal-type compatibility, RBAC and delegated approval fit, machine-credential lifecycle support, secrets reviewability, recovery and exception handling, domain-boundary compatibility, operational manageability, and audit-evidence integration.`

Commentary:

- Chief Information Officer: supported the motion and stated that the criteria convert the CVO's kickoff into testable design expectations rather than general aspirations.
- Chief Information Security Officer: supported the motion and clarified that recovery and exception handling are essential because trust failures often emerge there rather than in the happy path.
- PMO Director: supported the motion and stated that named criteria will keep later architecture comparison from becoming a loose discussion of preferences.
- Director of Product Management: supported the motion and added that principal-type compatibility and approval fit are especially important because they directly shape the experience of both humans and agents.
- Director of Information Technology: supported the motion and stressed that operational manageability must remain a first-class criterion or the initiative will design beyond its current operating estate.
- Director of Information Security: supported the motion and added that reviewability must include the ability to prove who had access, why, and under what exception path.
- Vice President of Enterprise Architecture: supported the motion and noted that domain-boundary compatibility is the criterion most likely to protect the enterprise from an attractive but ill-fitting stack.
- Director of DevOps: supported the motion and cautioned that machine-credential lifecycle support should be weighted heavily because the CVO specifically called for agent-capable software and IaC-driven deployments.
- Documentation Manager: supported the motion and confirmed that the criteria can serve as the skeleton of a future comparison matrix.

Disposition:

- Carried.

### Item 4 - Provisional Design Conclusion for the Current Package

Motion:

`Move that the current design package conclude provisionally that the enterprise should plan around a federated IAM service pattern with a directory authority component, a separate secrets-control component, and explicit publication and evidence surfaces, while deferring final product selection to a later comparison artifact built on the adopted evaluation criteria.`

Commentary:

- Chief Information Officer: supported the motion and stated that the conclusion is honest because it preserves architecture learning while still giving the initiative a clear shape.
- Chief Information Security Officer: supported the motion and clarified that deferring product selection is prudent given the enterprise's current maturity and the need for a reviewable comparison record.
- PMO Director: supported the motion and stated that this is the right level of closure for the current design package because it yields direction without false certainty.
- Director of Product Management: supported the motion and added that the conclusion is specific enough to enable future product and workflow planning.
- Director of Information Technology: supported the motion and stated that the federated pattern is acceptable so long as operational responsibilities remain explicit.
- Director of Information Security: supported the motion and stressed that the conclusion rightly avoids equating human convenience tooling with full machine trust governance.
- Vice President of Enterprise Architecture: supported the motion and noted that the federated pattern is the most consistent with the initiative's cross-module service posture.
- Director of DevOps: supported the motion and added that the conclusion leaves room to weight agent and service-account workflows properly during final comparison.
- Documentation Manager: supported the motion and confirmed that the provisional conclusion is publishable as a bounded design result rather than a final architecture decree.

Disposition:

- Carried.

## Secrets and Vault Determinations

The cabinet determined the following:

1. The initiative will compare candidate components within a directory-plus-vault service pattern rather than a one-tool-for-all pattern.
2. OpenLDAP remains an acceptable directory starting point for future comparison work, but no product has been selected.
3. OpenBao, Vaultwarden, and Psono remain candidate components for later comparison, but each must be evaluated against the full adopted criteria rather than by familiarity or convenience.
4. Machine credential lifecycle support is a decisive requirement because of the CVO's human-and-agent service vision.
5. The final design-phase meeting should test whether the current package is publishable, navigable, and ready for CVO review.

## Action Items

- Director of Information Security: draft a comparison-matrix outline using the adopted evaluation criteria.
- Chief Information Officer: prepare a concise design summary for the publication readiness review.
- Director of DevOps: prepare the machine-credential and IaC dependency note for later comparison work.
- Director of Information Technology: prepare an operational manageability note covering administration, recovery, and current-scale practicality.
- Documentation Manager: prepare the traceability package linking CVO input, retrospective sources, and design decisions.
- Technical Writer: publish these minutes and update the design-phase navigation with the Knowledge Manager.