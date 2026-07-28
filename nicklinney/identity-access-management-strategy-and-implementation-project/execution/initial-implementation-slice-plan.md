---
title: Identity and Access Management Initiative Initial Implementation Slice Plan
description: Execution-phase initial implementation slice plan for the IAM initiative.
published: true
date: 2026-07-28T19:05:59.518Z
tags: nicklinney, identity-access-management, execution, implementation-slice
editor: markdown
dateCreated: 2026-07-28T19:05:59.518Z
---

# Identity and Access Management Initiative Initial Implementation Slice Plan

## Metadata

| Field | Value |
| --- | --- |
| Artifact ID | NLIAM-EXE-005 |
| Initiative ID | NLIAM-2026-07-28-01 |
| Date | July 28, 2026 |
| Status | Draft for execution use |

## Slice Objective

Prove one governed IAM workflow that combines:

- one human access-request and approval path
- one machine credential issuance and use path
- retained evidence for request, approval, issuance, review, and exception handling

## Recommended Slice Boundary

The first slice should govern access for the IAM initiative's own delivery and documentation pathway rather than immediately attempting a broad enterprise rollout. This keeps the scope self-referential, auditable, and proportionate to current maturity.

## Proposed Pilot Workflow

### Human Path

1. A named human principal requests bounded access to the IAM initiative implementation resources.
2. The relevant module or platform owner approves or rejects the request.
3. If approved, the requester is assigned the appropriate role anchor in `OpenLDAP`.
4. The approval and assignment are recorded in the canonical governance records.

### Machine Path

1. A named service account or agent principal is created for one approved automation pathway.
2. The machine principal authenticates through the selected machine workflow in `OpenBao`.
3. `OpenBao` issues a bounded credential or token for the approved task.
4. The credential lease, use, and review obligations are recorded through the approved evidence surfaces.

## Implementation Components

- initial directory entries and group anchors in `OpenLDAP`
- initial machine auth role and policy path in `OpenBao`
- wiki-based decision and approval records
- first review checklist for credential issuance and renewal

## Success Criteria

- one human request is approved through the published matrix and reflected in the directory authority
- one machine workflow retrieves an approved credential through policy-controlled access
- the issuance path is revocable and reviewable
- the evidence pack can be published without exposing secret values

## Explicit Exclusions

- enterprise-wide SSO rollout
- broad migration of existing secrets
- final human-oriented vault standardization
- claims that the whole IAM capability is realized after the pilot