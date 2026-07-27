---
title: Document Naming and Ownership Standard
description: Defines naming, ownership, title structure, identifiers, and repository or wiki placement expectations for controlled artifacts.
published: true
date: 2026-07-27T08:07:58.176Z
tags: naming, documents, knowledge-management, ownership
editor: markdown
dateCreated: 2026-07-27T08:07:58.176Z
---

# Document Naming and Ownership Standard

## Purpose

This standard defines how controlled artifacts are titled, owned, identified, and placed within the NickLinney.* knowledge estate.

## Naming Objectives

Document names should be:

- stable
- descriptive
- module-aware
- human-readable
- suitable for both wiki paths and repository-backed storage

## Title Structure Guidance

Preferred pattern:

```text
<Module or Domain> <Artifact Title>
```

Examples:

- `NickLinney.Security Safety and Assurance Charter`
- `NickLinney.KnowledgeManagement Knowledge Management Strategy`
- `NickLinney.DevOps Initial Debian Virtual Machine Deployment Strategy`

Where a shorter public wiki title improves usability, the canonical module ownership should still be explicit in page metadata or opening identity lines.

## Ownership Rules

Every controlled artifact should declare:

- owning module
- responsible maintainer or authority
- approval authority when applicable
- canonical location or canonical page path

## Identifier Expectations

Where identifiers exist, they should be stable and never reused.

Where identifiers do not yet exist, documents should still be structured so that identifiers can be added later without ambiguity.

## Placement Rules

- governance and standards belong in stable governance or module policy spaces
- templates belong in dedicated template spaces
- product and project records should live beneath their domain or portfolio structure
- evidence and external references should not be mixed indistinguishably with native controlled policy

## Historical Note

Renaming should be minimized. When a title must change, relationships to prior titles should be preserved through redirects, related pages, or declared supersession notes.
