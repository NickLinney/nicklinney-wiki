---
title: Repository Exception and Attribution Decision Register
description: Controlled fourth-layer register for repository exceptions, attribution decisions, and bounded governance deviations in machine-assisted Git operations.
published: true
date: 2026-07-27T22:27:36.353Z
tags: register, autogit, attribution, exceptions
editor: markdown
dateCreated: 2026-07-27T22:27:36.353Z
---

# Repository Exception and Attribution Decision Register

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native fourth-layer control artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.AutoGit`

## Purpose

This register records repository-level exceptions and attribution decisions, especially where machine assistance or nonstandard workflows require explicit governance treatment.

## Example Decision Classes

- attribution override
- nonstandard branch or release workflow
- temporary repository stewardship exception
- automated commit-policy deviation
- emergency release bypass

## Minimum Register Fields

| Field | Description |
| --- | --- |
| Decision ID | Unique decision identifier. |
| Repository | Governed repository in scope. |
| Decision Class | Type of exception or attribution decision. |
| Rationale | Why the deviation is necessary. |
| Approval Authority | Reviewing or approving authority. |
| Expiration / Review Date | Bound on decision validity. |
| Remediation Path | Return to standard governance posture. |

## Governance Rule

Machine-assisted repository activity should be attributable, reviewable, and procedurally reversible.

## Related Pages

- [NickLinney.AutoGit](/nicklinney/autogit)
- [Git Attribution Policy Record](/nicklinney/autogit/git-attribution-policy-record)
- [Release Automation Control Procedure](/nicklinney/autogit/release-automation-control-procedure)
- [Repository Stewardship Register](/nicklinney/autogit/repository-stewardship-register)