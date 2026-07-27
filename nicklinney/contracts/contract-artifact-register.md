---
title: Contract Artifact Register
description: Structured register of governed contract artifacts, classes, status, compatibility posture, and supersession relationships for NickLinney.Contracts.
published: true
date: 2026-07-27T22:05:52.561Z
tags: register, contracts, control, artifacts
editor: markdown
dateCreated: 2026-07-27T22:05:52.561Z
---

# Contract Artifact Register

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native third-layer control artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.Contracts`

## Purpose

This register records governed contract artifacts owned by or routed through `NickLinney.Contracts`.

## Register Fields

Each record should identify at minimum:

- contract identifier
- title
- contract class
- owning module
- status
- version posture
- compatibility posture
- approval authority
- supersession relationship

## Seed Register

| Contract ID | Title | Contract Class | Owning Module | Status | Compatibility Posture | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| CTR-ART-001 | Interface and Schema Taxonomy Standard | Standard | NickLinney.Contracts | Canonical | Governing | Defines contract classes and naming rules. |
| CTR-ART-002 | Contract Review and Approval Procedure | Procedure | NickLinney.Contracts | Canonical | Governing | Defines admission and supersession workflow. |

## Governance Rule

No contract artifact should be treated as governed unless it is capable of being recorded in this register with explicit class, scope, and status.

## Related Pages

- [NickLinney.Contracts](/nicklinney/contracts)
- [Compatibility and Versioning Policy Hierarchy](/nicklinney/contracts/compatibility-and-versioning-policy-hierarchy)
- [Interface and Schema Taxonomy Standard](/nicklinney/contracts/interface-and-schema-taxonomy-standard)