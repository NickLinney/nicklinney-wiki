---
title: Enterprise Document Register
description: Initial controlled register for key NickLinney.* documentation artifacts, beginning with Knowledge Management records and upstream governance dependencies.
published: true
date: 2026-07-27T08:21:55.831Z
tags: documents, register, knowledge-management, phase-2
editor: markdown
dateCreated: 2026-07-27T08:21:55.831Z
---

# Enterprise Document Register

## Purpose

This page is the first operational register implementing the Knowledge Management plan.

It records logical document identities, current control metadata, canonicality status, known wiki paths, and recovery posture for high-value artifacts.

## Register Scope

This initial seed covers:

- the core Knowledge Management control artifacts created for the wiki program
- a small set of upstream governance dependencies that strongly influence document control and discovery

## Seed Records

| Record ID | Title | Owning Module | Class | Status | Canonicality | Source Origin | Wiki Path | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| KM-REG-001 | NickLinney.KnowledgeManagement | NickLinney.KnowledgeManagement | Module Landing Page | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management` | Module root for knowledge governance. |
| KM-REG-002 | Knowledge Management Strategy | NickLinney.KnowledgeManagement | Strategy | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/strategy` | Strategic objective for versioned, historically retained wiki population. |
| KM-REG-003 | Knowledge Management Plan | NickLinney.KnowledgeManagement | Plan | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/plan` | Phase-based implementation plan. |
| KM-REG-004 | Document Control and Publication Standard | NickLinney.KnowledgeManagement | Standard | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/document-control-and-publication-standard` | Defines controlled states and retention rules. |
| KM-REG-005 | Document Naming and Ownership Standard | NickLinney.KnowledgeManagement | Standard | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/document-naming-and-ownership-standard` | Defines title, ownership, and placement rules. |
| KM-REG-006 | Enterprise Document Register Schema | NickLinney.KnowledgeManagement | Schema Standard | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/enterprise-document-register-schema` | Defines minimum register fields. |
| KM-REG-007 | Chat-Generated Artifact Recovery Procedure | NickLinney.KnowledgeManagement | Procedure | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/chat-generated-artifact-recovery-procedure` | Governs recovery from chat and transcript fragments. |
| KM-REG-008 | Canonical Source Declaration Record Standard | NickLinney.KnowledgeManagement | Standard | Canonical | Canonical | Wiki-native controlled artifact | `/nicklinney/knowledge-management/canonical-source-declaration-record-standard` | Governs canonical-source resolution when duplicates exist. |
| GOV-REG-001 | Enterprise Document Inventory and Artifact Register | Enterprise Governance / Knowledge Management | Inventory Register | Reviewed | Candidate Canonical | Wiki page synthesized from enterprise inventory matrix | `/nicklinney/governance/enterprise-document-inventory-and-artifact-register` | Strong basis for register expansion; should later be linked to structured record exports. |
| GOV-REG-002 | Module Registry | Enterprise Governance | Registry | Reviewed | Candidate Canonical | Wiki-native synthesized artifact | `/nicklinney/governance/module-registry` | Current formal registry of recognized modules. |
| GOV-REG-003 | Software Documentation and Repository Architecture Standard | Enterprise Governance / NickLinney.SoftwareDevelopment | Standard | Reviewed | Candidate Canonical | Derived from source document | `/nicklinney/governance/software-documentation-and-repository-architecture-standard` | High-value upstream control artifact for document structure. |
| GOV-REG-004 | Portfolio Model and Context Management | Enterprise Governance | Governance Standard | Reviewed | Candidate Canonical | Derived from source document | `/nicklinney/governance/portfolio-model-and-context-management` | Governs boundaries and context anchoring. |

## Interpretation Notes

### Status

This seed register uses the controlled states introduced by the Document Control and Publication Standard.

### Canonicality

`Canonical` means the page is presently treated as the authoritative controlled wiki artifact.

`Candidate Canonical` means the page is acting as the best available controlled representation, but may later need explicit reconciliation with external files, recovered chat artifacts, or more formal repository-backed sources.

## Next Register Expansion Priorities

1. Add the remaining high-value governance standards and module records.
2. Register foundational chat-generated but unrecovered artifacts such as the Risk Classification Framework and Repository Information Architecture Standard.
3. Add confidence, approval authority, and supersession fields in a more structured machine-readable companion artifact.
4. Begin module-by-module register population, starting with Knowledge Management and Governance.

## Related Pages

- [Enterprise Document Register Schema](/nicklinney/knowledge-management/enterprise-document-register-schema)
- [Knowledge Management Plan](/nicklinney/knowledge-management/plan)
- [Enterprise Document Inventory and Artifact Register](/nicklinney/governance/enterprise-document-inventory-and-artifact-register)