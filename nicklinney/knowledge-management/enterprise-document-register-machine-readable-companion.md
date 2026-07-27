---
title: Enterprise Document Register Machine-Readable Companion
description: Machine-readable companion register with confidence, approval authority, and supersession metadata for high-value NickLinney.* records.
published: true
date: 2026-07-27T10:56:48.819Z
tags: register, knowledge-management, metadata, machine-readable, automation
editor: markdown
dateCreated: 2026-07-27T10:56:48.819Z
---

# Enterprise Document Register Machine-Readable Companion

## Purpose

This page provides a machine-readable companion to the human-readable [Enterprise Document Register](/nicklinney/knowledge-management/enterprise-document-register).

It extends the current register with fields needed for automation, confidence scoring, approval tracing, and supersession management.

## Companion Field Model

Each record in this companion should eventually support these fields:

- `record_id`
- `title`
- `owning_module`
- `document_class`
- `status`
- `canonicality`
- `approval_authority`
- `maintainer`
- `confidence`
- `source_origin`
- `source_reference`
- `wiki_path`
- `supersedes`
- `superseded_by`
- `related_records`
- `notes`

## Current Working Register

```yaml
records:
  - record_id: KM-REG-001
    title: NickLinney.KnowledgeManagement
    owning_module: NickLinney.KnowledgeManagement
    document_class: Module Landing Page
    status: Canonical
    canonicality: Canonical
    approval_authority: NickLinneyDev / Portfolio Maintainer
    maintainer: NickLinney.KnowledgeManagement
    confidence: high
    source_origin: wiki-native controlled artifact
    source_reference: /nicklinney/knowledge-management
    wiki_path: /nicklinney/knowledge-management
    supersedes: []
    superseded_by: []
    related_records: [KM-REG-002, KM-REG-003, KM-REG-010]
    notes: Module root for knowledge governance.

  - record_id: GOV-REG-006
    title: Organizational Cadence and Enterprise Reporting Standard
    owning_module: Enterprise Governance
    document_class: Governance Standard
    status: Reviewed
    canonicality: Candidate Canonical
    approval_authority: Executive Governance / Portfolio Maintainer
    maintainer: NickLinney.KnowledgeManagement
    confidence: high
    source_origin: retrieved ChatGPT export corpus
    source_reference: g-p-6a0acd9d715c8191a9e57ae97945496e-business-design :: 008_Marketing_PaaS_strategy enterprise reporting framework
    wiki_path: /nicklinney/governance/organizational-cadence-and-enterprise-reporting-standard
    supersedes: []
    superseded_by: []
    related_records: [GOV-REG-007, KM-REG-010]
    notes: Strong source-backed recovery for reporting cadence, ownership, and historiographic intent.

  - record_id: GOV-REG-007
    title: Executive and Cabinet Meeting Record Standard
    owning_module: Enterprise Governance
    document_class: Governance Standard
    status: Canonical
    canonicality: Canonical
    approval_authority: Executive Governance / Portfolio Maintainer
    maintainer: NickLinney.KnowledgeManagement
    confidence: medium
    source_origin: wiki-native normalized artifact derived from recovered source-backed governance
    source_reference: normalized from enterprise reporting framework and cabinet-cadence planning materials
    wiki_path: /nicklinney/governance/executive-and-cabinet-meeting-record-standard
    supersedes: []
    superseded_by: []
    related_records: [GOV-REG-006, KM-REG-010]
    notes: New normalized standard created to make meeting-record capture operational.

  - record_id: AGT-REG-001
    title: NickLinney.Agents Executive Project Abstract
    owning_module: NickLinney.Agents
    document_class: Executive Abstract
    status: Reviewed
    canonicality: Candidate Canonical
    approval_authority: NickLinney.Agents / Portfolio Maintainer
    maintainer: NickLinney.KnowledgeManagement
    confidence: high
    source_origin: retrieved ChatGPT export corpus
    source_reference: g-p-6a0df82eb84481919763836a51a1853d-nicklinney-agents :: 003_NickLinney.Agents - Executive Project Abstract
    wiki_path: /nicklinney/agents/executive-project-abstract
    supersedes: []
    superseded_by: []
    related_records: [AGT-REG-002, STR-REG-003, MOD-REG-001]
    notes: Strong recovery of executive positioning for the module.

  - record_id: AGT-REG-002
    title: NickLinney.Agents Repository Information Architecture Draft
    owning_module: NickLinney.Agents
    document_class: Repository Architecture Draft
    status: Draft
    canonicality: Candidate Canonical
    approval_authority: NickLinney.Agents / Portfolio Maintainer
    maintainer: NickLinney.KnowledgeManagement
    confidence: medium
    source_origin: retrieved ChatGPT export corpus
    source_reference: g-p-6a1153728f0c819198b731c47bf16234-nicklinney-ops :: planning matrix repository-design tasks
    wiki_path: /nicklinney/agents/repository-information-architecture-draft
    supersedes: []
    superseded_by: []
    related_records: [AGT-REG-001, SRC-REG-008, GOV-REG-003]
    notes: Partial recovery lead only; full structural standard still requires additional source recovery.

  - record_id: SYS-REG-001
    title: ADR Draft — Context Isolation and Agentic Cognitive Boundaries
    owning_module: NickLinney.System
    document_class: ADR Draft Record
    status: Draft
    canonicality: Candidate Canonical
    approval_authority: NickLinney.System / Portfolio Maintainer
    maintainer: NickLinney.KnowledgeManagement
    confidence: medium
    source_origin: retrieved ChatGPT export corpus
    source_reference: g-p-6a1153728f0c819198b731c47bf16234-nicklinney-ops :: planning export
    wiki_path: /nicklinney/system/adr-draft-context-isolation-and-agentic-cognitive-boundaries
    supersedes: []
    superseded_by: []
    related_records: [AGT-REG-002, SRC-REG-008]
    notes: Recovery preserves title and rationale but not a complete ADR body.
```

## Confidence Interpretation

- `high` means the retrieved corpus preserves a directly recognizable artifact body or clearly named recovery source.
- `medium` means the retrieved corpus preserves a strong planning or partial-content lead but not a complete final document.
- `low` should be reserved for weak or indirect evidence and is not yet used in this companion.

## Approval Authority Interpretation

These values are provisional governance fields intended to make later approval workflows machine-addressable. They should be normalized further once a formal approval-authority registry exists.

## Related Pages

- [Enterprise Document Register](/nicklinney/knowledge-management/enterprise-document-register)
- [Enterprise Document Register Schema](/nicklinney/knowledge-management/enterprise-document-register-schema)
- [Retrieved Project Source Reconciliation](/nicklinney/knowledge-management/retrieved-project-source-reconciliation)