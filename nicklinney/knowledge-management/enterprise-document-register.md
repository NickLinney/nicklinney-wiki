---
title: Enterprise Document Register
description: Controlled register for key NickLinney.* documentation artifacts, including wiki-native records and source-backed recovery candidates.
published: true
date: 2026-07-27T10:19:54.643Z
tags: documents, register, knowledge-management, phase-2
editor: markdown
dateCreated: 2026-07-27T08:21:55.831Z
---

# Enterprise Document Register

## Purpose

This page is the first operational register implementing the Knowledge Management plan.

It records logical document identities, current control metadata, canonicality status, known wiki paths, and recovery posture for high-value artifacts.

## Register Scope

This current register covers:

- the core Knowledge Management control artifacts created for the wiki program
- upstream governance dependencies already represented in the wiki
- newly reconciled source-backed candidate records identified from the `retrieved_projects` export corpus
- first-tranche recovered Phase 3 artifacts published on July 27, 2026

## Controlled Wiki Records

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
| KM-REG-009 | Retrieved Project Source Reconciliation | NickLinney.KnowledgeManagement | Reconciliation Record | Canonical | Canonical | Wiki-native controlled artifact using retrieved export corpus | `/nicklinney/knowledge-management/retrieved-project-source-reconciliation` | Documents the first retrieval-backed reconciliation pass. |
| GOV-REG-001 | Enterprise Document Inventory and Artifact Register | Enterprise Governance / Knowledge Management | Inventory Register | Reviewed | Candidate Canonical | Wiki page synthesized from enterprise inventory matrix | `/nicklinney/governance/enterprise-document-inventory-and-artifact-register` | Strong basis for register expansion; should later be linked to structured record exports. |
| GOV-REG-002 | Module Registry | Enterprise Governance | Registry | Reviewed | Candidate Canonical | Wiki-native synthesized artifact | `/nicklinney/governance/module-registry` | Current formal registry of recognized modules. |
| GOV-REG-003 | Software Documentation and Repository Architecture Standard | Enterprise Governance / NickLinney.SoftwareDevelopment | Standard | Reviewed | Candidate Canonical | Derived from source document | `/nicklinney/governance/software-documentation-and-repository-architecture-standard` | High-value upstream control artifact for document structure. |
| GOV-REG-004 | Portfolio Model and Context Management | Enterprise Governance | Governance Standard | Reviewed | Candidate Canonical | Derived from source document | `/nicklinney/governance/portfolio-model-and-context-management` | Governs boundaries and context anchoring. |
| SEC-REG-001 | Risk Classification Framework | NickLinney.Security | Framework Standard | Reviewed | Candidate Canonical | Recovered from retrieved ChatGPT export corpus | `/nicklinney/security/risk-classification-framework` | First Phase 3 recovery tranche. |
| OPS-REG-001 | Virtual Cybernetic Enterprise Production Manual and SOP Guide | NickLinney.Ops / NickLinney.SoftwareFactory / NickLinney.Agents | Operating Manual / SOP | Reviewed | Candidate Canonical | Recovered from retrieved ChatGPT export corpus | `/nicklinney/ops/virtual-cybernetic-enterprise-production-manual-and-sop-guide` | First Phase 3 recovery tranche. |
| GOV-REG-005 | Good Faith Diligence Rule | Enterprise Governance | Governance Rule | Reviewed | Candidate Canonical | Recovered from retrieved ChatGPT export corpus | `/nicklinney/governance/good-faith-diligence-rule` | First Phase 3 recovery tranche. |

## Reconciled Source-Backed Candidate Records

| Record ID | Title | Owning Module | Class | Status | Canonicality | Source Origin | Recovery Source | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SRC-REG-001 | Risk Classification Framework | NickLinney.Security | Framework Standard | Reviewed | Candidate Canonical | Retrieved ChatGPT export corpus | `g-p-6a4ef7d1f9ec81919f5f72b77957a988-nicklinney-security` chat inventory and `004_Risk_Classification_Framework` | Now normalized into a controlled wiki artifact. |
| SRC-REG-002 | Virtual Cybernetic Enterprise Manual / Standard Operating Procedure | NickLinney.Ops / NickLinney.Agents | Operating Manual / SOP | Reviewed | Candidate Canonical | Retrieved ChatGPT export corpus | `g-p-6a0acd9d715c8191a9e57ae97945496e-business-design` chat `001_Virtual_Cybernetic_Enterprise_Manual` | Now normalized into a controlled wiki artifact. |
| SRC-REG-003 | Good Faith Diligence Rule | Enterprise Governance | Governance Rule | Reviewed | Candidate Canonical | Retrieved ChatGPT export corpus | `g-p-6a0acd9d715c8191a9e57ae97945496e-business-design` chat `003_Good_faith_diligence_rule...` | Now normalized into a controlled wiki artifact. |
| SRC-REG-004 | NickLinney Modules Index / Portfolio and Module Registry Lead | NickLinney.Strategy | Registry Lead | Reviewed | Candidate Canonical | Retrieved ChatGPT export corpus | `g-p-6a4fd8c552f88191b6da36886c161f5f-nicklinney-modules` chat `002_NickLinney_Modules_Index...` | Direct evidence for module-list recovery and refinement of the formal registry. |
| SRC-REG-005 | Goal: Create Cybernetic Software Ecosystem | NickLinney.Strategy | Strategic Objective | Reviewed | Candidate Canonical | Retrieved ChatGPT export corpus | `g-p-6a4ef41bd90c819189f7db15b84e5a8e-nicklinney-strategy` project manifest | Strong recovery lead for constitutional or strategy-root objective material. |
| SRC-REG-006 | NickLinney Agentic Development Strategy | NickLinney.Strategy / NickLinney.Agents / NickLinney.SoftwareFactory | Strategy | Reviewed | Candidate Canonical | Retrieved ChatGPT export corpus | `g-p-6a4ef41bd90c819189f7db15b84e5a8e-nicklinney-strategy` project manifest | Directly evidenced project source for a strategy artifact already referenced in the enterprise matrix. |

## Interpretation Notes

### Status

This register uses the controlled states introduced by the Document Control and Publication Standard.

### Canonicality

`Canonical` means the page is presently treated as the authoritative controlled wiki artifact.

`Candidate Canonical` means the page is acting as the best available controlled representation, or that final normalization and approval remain pending.

### Recovery Source

For source-backed candidate records, the `Recovery Source` column points to the retrieved-project export evidence rather than to an already-approved canonical source outside the wiki.

## Next Register Expansion Priorities

1. Refine the module registry using retrieved module and strategy exports.
2. Recover strategy-root artifacts, beginning with `Goal: Create Cybernetic Software Ecosystem` and related constitutional material.
3. Continue scanning retrieved exports for explicit ADR, repository-architecture, and governance-record source conversations.
4. Add confidence, approval authority, and supersession fields in a more structured machine-readable companion artifact.

## Related Pages

- [Retrieved Project Source Reconciliation](/nicklinney/knowledge-management/retrieved-project-source-reconciliation)
- [Enterprise Document Register Schema](/nicklinney/knowledge-management/enterprise-document-register-schema)
- [Knowledge Management Plan](/nicklinney/knowledge-management/plan)
- [Enterprise Document Inventory and Artifact Register](/nicklinney/governance/enterprise-document-inventory-and-artifact-register)