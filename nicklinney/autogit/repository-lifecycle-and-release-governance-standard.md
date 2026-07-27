---
title: Repository Lifecycle and Release Governance Standard
description: Standard defining repository creation, stewardship, versioning, release state, and retirement governance.
published: true
date: 2026-07-27T11:29:53.769Z
tags: standard, autogit, release, repository
editor: markdown
dateCreated: 2026-07-27T11:29:53.769Z
---

# Repository Lifecycle and Release Governance Standard

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native standards-layer artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.AutoGit`

## Purpose

This standard defines how repositories are created, stewarded, versioned, released, and retired as governed assets.

## Minimum Lifecycle States

- proposed
- active
- maintained
- release-managed
- archived
- retired

## Governance Rule

Every repository should have an identifiable stewardship posture, release model, and retirement path. Repositories should not remain ambiguous long-term artifacts.

## Minimum Artifact Expectations

Each governed repository should declare:

- repository purpose
- owning module
- stewardship owner
- release model
- semantic versioning posture
- archive or retirement condition

## Related Pages

- [NickLinney.AutoGit](/nicklinney/autogit)
- [Operational Git Workflow Standard](/nicklinney/autogit/operational-git-workflow-standard)
- [Enterprise Document Register Schema](/nicklinney/knowledge-management/enterprise-document-register-schema)