---
title: Enterprise Document Register Schema
description: Machine-readable schema definition for tracking controlled and prospective document artifacts across the NickLinney.* ecosystem.
published: true
date: 2026-07-27T08:07:59.162Z
tags: register, knowledge-management, schema, metadata
editor: markdown
dateCreated: 2026-07-27T08:07:59.162Z
---

# Enterprise Document Register Schema

## Purpose

This schema defines the minimum machine-readable fields for the enterprise document register that backs the wiki and broader knowledge estate.

## Core Fields

```yaml
id:
title:
normalized_title:
owning_module:
document_class:
status:
canonicality:
version:
source_origin:
source_location:
wiki_path:
repository_path:
approval_authority:
maintainer:
created_date:
last_reviewed_date:
supersedes:
superseded_by:
related_artifacts:
confidence:
notes:
```

## Field Intent

- `id`: durable internal identifier for the logical artifact record
- `title`: current human title
- `normalized_title`: comparison-safe title for matching and deduplication
- `owning_module`: primary governance or operational owner
- `document_class`: standard, strategy, plan, template, evidence, reference, record, abstract, and similar classification
- `status`: draft, reviewed, approved, canonical, superseded, deprecated, archived, evidence-only, or other controlled state
- `canonicality`: whether this record is canonical, candidate-canonical, duplicate, or unresolved
- `version`: declared version if known
- `source_origin`: uploaded source, recovered chat, composite synthesis, external reference, and similar origin type
- `source_location`: known storage pointer or source reference
- `wiki_path`: canonical or current wiki page path when published
- `repository_path`: canonical repository source path when applicable
- `approval_authority`: who can approve or designate canonical status
- `maintainer`: who maintains currency and corrections
- `supersedes` and `superseded_by`: historical lineage
- `related_artifacts`: connected records, templates, standards, or evidence
- `confidence`: confidence in the reconstruction or metadata completeness

## Schema Use

The register should track both:

- existing controlled artifacts
- expected or proposed artifacts not yet fully recovered

This preserves planning continuity and prevents repeated loss of known-but-unrecovered documents.
