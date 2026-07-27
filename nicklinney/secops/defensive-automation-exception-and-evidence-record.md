---
title: Defensive Automation Exception and Evidence Record
description: Controlled fourth-layer record governing exceptions, approvals, and evidence for automated defensive actions in security operations.
published: true
date: 2026-07-27T22:27:34.330Z
tags: automation, secops, exceptions, evidence
editor: markdown
dateCreated: 2026-07-27T22:27:34.330Z
---

# Defensive Automation Exception and Evidence Record

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native fourth-layer operational control artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.SecOps`

## Purpose

This record governs when defensive automations may act automatically, when they require bounded exceptions, and what evidence must be retained.

## When It Applies

Use this record for any automation that can:

- isolate or block an entity
- alter access posture
- trigger containment actions
- suppress or override expected analyst review

## Minimum Record Fields

| Field | Description |
| --- | --- |
| Automation ID | Controlled identifier of the defensive automation. |
| Action Class | Monitoring, alerting, blocking, isolation, or containment. |
| Default Approval Mode | Automatic, analyst-reviewed, or executive-approved. |
| Exception Trigger | Condition requiring exception handling. |
| Evidence Retained | Required proof of trigger, action, and outcome. |
| Review Authority | Responsible authority for oversight. |

## Governance Rule

Higher-autonomy defensive actions require stronger evidence retention and tighter exception boundaries.

## Related Pages

- [NickLinney.SecOps](/nicklinney/secops)
- [Vulnerability Management Lifecycle Standard](/nicklinney/secops/vulnerability-management-lifecycle-standard)
- [Security Operations Reporting Matrix](/nicklinney/secops/security-operations-reporting-matrix)
- [Security Operations Decision Register](/nicklinney/secops/security-operations-decision-register)