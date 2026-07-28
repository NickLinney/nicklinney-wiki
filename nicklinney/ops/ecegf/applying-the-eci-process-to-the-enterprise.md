---
title: NickLinney.Ops - Applying the ECI Process to the Enterprise
description: Operating guidance for applying the ECI lifecycle, cadences, and evidence rules to enterprise and other eligible ECI targets.
published: true
date: 2026-07-28T07:51:13.258Z
tags: governance, ops, ecegf, eci, process
editor: markdown
dateCreated: 2026-07-28T07:51:13.258Z
---

# NickLinney.Ops - Applying the ECI Process to the Enterprise

## Metadata

| Field | Value |
| --- | --- |
| Document ID | ECEGF-013 |
| Document Type | Process Application Guide |
| Category | Operating Guidance |
| Status | Draft |
| Version | 1.0 |
| Effective Date | July 28, 2026 |
| Last Updated | July 28, 2026 |
| Owner | Director of Knowledge Management |
| Requesting Authority | Chief Information Officer |
| Originating Direction | Chief Vision Officer |
| Framework | NickLinney.Ops - Enterprise Capability Evaluation and Governance Framework (ECEGF) |

## Purpose

This document explains how to apply the Enterprise Capability Investigation process to the NickLinney Enterprise as an operating practice rather than as a one-time exercise. It models the sequence, cadences, and decision points used during the 2026 enterprise investigation and expresses them in a form that can be reused for any eligible ECI target.

## Intended Use

This guide is written for any future ECI application where the target is a governable capability-bearing object. Depending on scope, that target may be:

- a module
- a product or platform
- a project or initiative
- a department, function, or operating domain
- an enterprise or ecosystem
- an event, incident, or operational condition
- an external or adjacent entity where the enterprise has enough observable evidence to assess it

The exact target set remains governed by the ECI framework and the evidence actually available at the time of assessment.

## Core Operating Principle

The ECI process is not merely a scoring activity. It is a governed evidence-construction and interpretation cycle that:

- defines the target and its assessment boundary
- gathers and classifies evidence
- scores strategic design and realized maturity separately
- identifies the gap between them
- records the resulting actions, artifacts, and governance decisions
- repeats at a useful cadence so the enterprise can learn without overstating reality

## Controlling Realization Rule

When the ECI process is applied, realized maturity must be governed by the stricter realization rule:

- a capability counts as operationally realized only when a direct evidentiary object proves that it is deployed and active, or another artifact clearly demonstrates that such reality exists or must exist
- if such proof is absent, the capability is treated as `In Progress / Not Realized`

This rule prevents design strength from being mistaken for runtime maturity.

## Standard ECI Lifecycle

The following sequence models the process as it was applied to the NickLinney Enterprise and should be treated as the standard operating pattern unless a later ADR changes it.

### 1. Open the Governing Event

Create or identify the governing event record before assessment begins.

Required outputs:

- event or charter record
- purpose, scope, exclusions, and strategic alignment
- named owner and coordinating functions
- child-object model for downstream artifacts

### 2. Define the Assessment Boundary

Declare what the target is, what is in scope, what is out of scope, and what evidence sources are admissible.

Boundary questions:

- What exactly is being assessed?
- At what level is it being assessed: module, enterprise, event, function, or other target?
- What dependencies are adjacent but not primary?
- What claims cannot be made because the evidence boundary is too weak?

### 3. Establish Staffing and Roles

Assign the roles needed to perform the assessment and maintain evidentiary discipline.

Typical roles:

- governance lead
- assessment lead
- domain subject-matter reviewers
- knowledge management or recording authority
- executive or cabinet reviewers where synthesis or interpretation is required

### 4. Build the Artifact Spine

Create the tracking and control artifacts that will hold the assessment together.

Minimum artifact spine:

- planning record
- staffing or assignment record
- artifact register
- evidence register
- score reports
- gap report
- action plan
- lifecycle or closure note

At enterprise scale, additional synthesis and cabinet artifacts may be needed.

### 5. Gather and Classify Evidence

Collect the evidence corpus before deciding maturity. Separate evidence into:

- direct evidence
- adjacent evidence
- supporting design evidence
- explicit evidence absence

The process should record not only what exists, but what does not exist and therefore limits defensible claims.

### 6. Produce SICAF and RCMF Readings

Evaluate the target twice:

- once for strategic or structural design quality
- once for realized and evidenced operational maturity

This dual-reading is essential because many enterprise targets are stronger in design than in realized operation.

### 7. Compile the Capability Gap View

Translate the difference between the two readings into a governed gap statement.

The gap view should answer:

- How large is the gap?
- Why does the gap exist?
- What risks arise if the target is treated as more mature than the evidence allows?
- What improvements would most efficiently close the gap?

### 8. Produce the Action Plan

Create a bounded action plan with named owners, expected evidence outputs, and review points. The action plan should improve future realizability and future assessability at the same time.

### 9. Register the Outputs

Track the resulting artifacts so they can be reviewed later and cited as part of future enterprise synthesis.

Registration should include:

- document identity
- location
- status
- ownership
- relationship to the governing event

### 10. Synthesize Upward When Required

If the target belongs to a larger governed body, the completed output should feed upward into the next aggregation layer.

Examples:

- module outputs feed enterprise synthesis
- incident outputs feed security or operational reviews
- project outputs feed portfolio or product governance

### 11. Interpret Through Governance

Where stakes are higher, hold a cabinet, review board, or executive interpretation step. Commentary should stay disciplined and evidence-first. Interpretive review should never erase evidence limitations established earlier in the process.

### 12. Close, Reassess, or Recur

End each cycle by deciding whether the target is:

- complete for the present cycle
- ready for periodic reassessment
- awaiting stronger evidence
- ready for synthesis into a broader target

## Recommended Cadences

The right cadence depends on the target type and the cost of change, but the 2026 enterprise application suggests the following defaults:

| Cadence | Recommended use |
| --- | --- |
| Event-driven | New initiatives, incidents, material governance concerns, or newly visible targets |
| Monthly | Active gap tracking where evidence may change quickly |
| Quarterly | Executive review, synthesis refresh, and cross-target comparison |
| Semiannual or annual | Broad enterprise or ecosystem reassessment where the target set is large |

Cadence should be increased when evidence is changing rapidly and reduced when the target is stable and expensive to reassess.

## How the 2026 Enterprise Application Mapped to the Lifecycle

The NickLinney Enterprise application followed the lifecycle in this order:

1. Opened a governing operational event for the `Enterprise Capability Investigation: NickLinney.Enterprise Ecosystem`
2. Defined the enterprise target and separated module-level assessment from enterprise synthesis
3. Established staff roles, agent assignments, and governance ownership
4. Created a full artifact spine including registers, module packages, synthesis outputs, cabinet records, and publication records
5. Re-baselined realization to a stricter evidence rule
6. Produced module-level `RCMF vs. SICAF Capability Gap Report and Action Plan` outputs for all scoped modules
7. Compiled the enterprise-level gap report from those module outputs
8. Conducted a postmortem cabinet process to create an Executive Chair report
9. Published the evidence corpus into the canonical wiki
10. Opened an executive retrospective phase for forward-looking action priorities

## Adaptation Rules for Other ECI Targets

The same process can be adapted across target types if these rules are preserved:

- keep the target boundary explicit
- preserve the dual-reading model
- preserve the realization rule
- preserve artifact traceability
- scale the artifact set to the size of the target without collapsing the control logic

In practice:

- a small module may need only the minimum artifact spine
- an enterprise or portfolio may require synthesis, cabinet, and publication layers
- an incident or event may compress planning but expand evidence and chronology
- an external entity may require stronger admissibility rules because observability is weaker

## Minimum Success Conditions

An ECI cycle should be considered well-executed when it produces:

- a clear target definition
- a reviewable evidence body
- separate SICAF and RCMF positions
- a credible gap statement
- a bounded action plan
- tracked artifacts that can be cited later

## Failure Modes to Avoid

- treating design coherence as proof of realization
- allowing evidence absence to disappear from the report
- assessing too many targets at once without boundary control
- letting synthesis language overstate module reality
- creating artifacts without registering or governing them
- running the cycle without a planned reassessment cadence

## Closing Guidance

The ECI process is most valuable when it is applied repeatedly, honestly, and proportionately. Its purpose is not to produce flattering scores. Its purpose is to make the enterprise more governable, more evidence-literate, and more capable of converting strategic intent into reviewable operational reality.