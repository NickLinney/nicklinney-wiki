---
title: Managed Toolchain Profile Register
description: Register of governed development environment profiles, toolchains, support posture, and validation status for NickLinney.env.
published: true
date: 2026-07-27T22:07:06.394Z
tags: register, env, toolchain, profiles
editor: markdown
dateCreated: 2026-07-27T22:07:06.394Z
---

# Managed Toolchain Profile Register

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native third-layer control artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.env`

## Purpose

This register records governed environment and toolchain profiles recognized by `NickLinney.env`.

## Minimum Record Fields

- profile identifier
- operating system
- shell profile
- runtime set
- package manager set
- support posture
- validation date

## Seed Entries

| Profile ID | Platform | Shell | Support Posture | Notes |
| --- | --- | --- | --- | --- |
| ENV-PROF-001 | macOS workstation | managed shell profile | Active baseline | Initial local-first environment posture. |
| ENV-PROF-002 | CI or ephemeral automation environment | non-interactive shell | Planned | To be normalized against automation workflows. |

## Related Pages

- [NickLinney.env](/nicklinney/env)
- [Environment Compatibility Matrix](/nicklinney/env/environment-compatibility-matrix)
- [Environment Governance Decision Record](/nicklinney/env/environment-governance-decision-record)