---
title: Identity and Access Management Initiative Approval Matrix Draft
description: Execution-phase approval matrix draft for the IAM initiative.
published: true
date: 2026-07-28T19:05:55.180Z
tags: nicklinney, identity-access-management, execution, approval-matrix
editor: markdown
dateCreated: 2026-07-28T19:05:55.180Z
---

# Identity and Access Management Initiative Approval Matrix Draft

## Metadata

| Field | Value |
| --- | --- |
| Artifact ID | NLIAM-EXE-004 |
| Initiative ID | NLIAM-2026-07-28-01 |
| Date | July 28, 2026 |
| Status | Draft for execution use |

## Purpose

This matrix converts the design-phase authority model into an execution-ready draft that can govern the first implementation slice without overstating enterprise staffing depth.

## Approval Matrix

| Access or Control Type | Requester Types | Primary Approver | Secondary or Control Approver | Record Location |
| --- | --- | --- | --- | --- |
| Standard module read access | human operational principals; agent principals acting on bounded tasks | module owner | none unless elevated data scope applies | access request and grant record |
| Standard module write or change access | human operational principals | module owner | security approver when trust boundary changes | access request and approval record |
| Privileged administrative access | privileged administrative principals | platform owner | security approver | privileged access record |
| Machine credential issuance for approved automation path | service-account principals; agent principals | platform owner | security approver | credential issuance record and policy record |
| Secret retrieval for approved machine workflow | service-account principals; agent principals | policy-controlled automated approval | security review through periodic control review | vault audit trail plus review record |
| Emergency or recovery access | emergency or recovery principals | platform owner | security approver with post-use review required | exception and review record |
| Role or group definition changes | governance and platform roles | CIO delegate or module owner as applicable | security approver when privilege expands | decision record and directory change record |

## Operating Notes

- The matrix assumes module ownership is explicit and reviewable.
- The matrix assumes security approval is a real control surface, not a ceremonial notification.
- The matrix intentionally separates machine credential issuance from human password or secret convenience workflows.
- Emergency access is permitted only with retained exception evidence and post-use review.

## Current-Scale Consolidation Rule

Where the current enterprise staff footprint requires one person to hold more than one role family, the dual duty must be recorded explicitly and reviewed rather than treated as invisible overlap.

## Open Follow-Up Items

- confirm the first named module-owner set for the pilot slice
- confirm the exact platform-owner role for `OpenLDAP` and `OpenBao`
- define periodic review cadence for issued machine credentials