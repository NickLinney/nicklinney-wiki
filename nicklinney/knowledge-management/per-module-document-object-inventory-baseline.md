---
title: Per-Module Document Object Inventory Baseline
description: Baseline per-module inventory of current wiki document objects and procedural documentation gaps across the canonical NickLinney.* module set.
published: true
date: 2026-07-27T11:06:35.358Z
tags: inventory, documents, modules, knowledge-management, baseline
editor: markdown
dateCreated: 2026-07-27T11:06:35.358Z
---

# Per-Module Document Object Inventory Baseline

## Status

- Status: Canonical
- Canonicality: Canonical
- Created: July 27, 2026
- Basis: current Wiki.JS page inventory reconciled against the canonical module registry

## Purpose

This page establishes the baseline per-module inventory of document objects presently represented in the wiki.

It is intended to support a definitive and procedural documentation program by answering three questions for each canonical module:

1. What separately addressable document objects currently exist?
2. Which of those are direct module objects versus cross-module supporting records?
3. What minimum object set is still missing before the module can be considered procedurally grounded?

## Definition of Document Object

For this baseline, a document object is any separately addressable wiki page intended to function as one of the following:

- module landing page
- executive abstract
- strategy or plan
- standard, procedure, framework, or manual
- ADR or governance record
- register, inventory, or structured companion artifact

Shared navigation pages, templates, and enterprise-wide hub pages are tracked separately and are not counted as direct module objects unless they are clearly owned by a module.

## Summary Matrix

| Module | Direct Objects | Cross-Module Supporting Objects | Procedural Posture |
| --- | ---: | ---: | --- |
| `NickLinney.System` | 1 | 2 | Partial recovery only |
| `System` | 0 | 1 | No direct module objects yet |
| `NickLinney.Agents` | 3 | 4 | Early baseline established |
| `NickLinney.Contracts` | 0 | 1 | No direct module objects yet |
| `NickLinney.DataInfrastructure` | 0 | 1 | No direct module objects yet |
| `NickLinney.DevOps` | 0 | 1 | No direct module objects yet |
| `NickLinney.env` | 0 | 1 | No direct module objects yet |
| `NickLinney.KnowledgeManagement` | 12 | 3 | Strong operational baseline |
| `NickLinney.Modules` | 2 | 2 | Registry baseline established |
| `NickLinney.Ops` | 1 | 2 | Initial recovered baseline |
| `NickLinney.SecOps` | 0 | 1 | No direct module objects yet |
| `NickLinney.Security` | 2 | 2 | Initial recovered baseline |
| `NickLinney.SoftwareFactory` | 0 | 3 | Cross-module references only |
| `NickLinney.Strategy` | 3 | 2 | Initial recovered baseline |
| `NickLinney.AutoGit` | 0 | 1 | No direct module objects yet |
| `NickLinney.YubiKey` | 0 | 1 | No direct module objects yet |

## Detailed Module Inventory

### NickLinney.System

Procedural posture: partial recovery only.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| ADR Draft — Context Isolation and Agentic Cognitive Boundaries | ADR Draft Record | Draft | `/nicklinney/system/adr-draft-context-isolation-and-agentic-cognitive-boundaries` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Recognizes `NickLinney.System` as a canonical module. |
| Constitutional Objective / Goal 1 | Strategic objective framing the broader system architecture. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- scope and boundary statement
- module standards or architecture records beyond the recovered ADR draft

### System

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Preserves `System` as a distinct research and incubation project. |

Immediate missing minimum objects:

- module or project landing page
- executive abstract or research charter
- boundary statement distinguishing `System` from `NickLinney.System`
- research artifact index

### NickLinney.Agents

Procedural posture: early baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.Agents | Module Landing Page | Canonical | `/nicklinney/agents` |
| NickLinney.Agents Executive Project Abstract | Executive Abstract | Reviewed | `/nicklinney/agents/executive-project-abstract` |
| NickLinney.Agents Repository Information Architecture Draft | Repository Architecture Draft | Draft | `/nicklinney/agents/repository-information-architecture-draft` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney Agentic Development Strategy | Strategy shared with broader agentic architecture work. |
| ADR Draft — Context Isolation and Agentic Cognitive Boundaries | Cross-owned architectural boundary record. |
| Virtual Cybernetic Enterprise Production Manual and SOP Guide | Operational doctrine shared with agentic enterprise behavior. |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition and boundary definition. |

Immediate missing minimum objects:

- module standards set beyond the repository draft
- governed taxonomy or role-definition record
- lifecycle and runtime-state standards
- meeting or reporting lifecycle standard specific to agent operations

### NickLinney.Contracts

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- contracts and interfaces standard set
- compatibility and versioning record

### NickLinney.DataInfrastructure

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- data architecture standards
- storage and lifecycle records

### NickLinney.DevOps

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- CI/CD and infrastructure governance standards
- release engineering records

### NickLinney.env

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- environment/bootstrap standard set
- compatibility and provisioning records

### NickLinney.KnowledgeManagement

Procedural posture: strong operational baseline.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.KnowledgeManagement | Module Landing Page | Canonical | `/nicklinney/knowledge-management` |
| Knowledge Management Inventory and Dependency Map | Inventory Map | Canonical | `/nicklinney/knowledge-management/inventory-and-dependency-map` |
| Knowledge Management Strategy | Strategy | Canonical | `/nicklinney/knowledge-management/strategy` |
| Knowledge Management Plan | Plan | Canonical | `/nicklinney/knowledge-management/plan` |
| Document Control and Publication Standard | Standard | Canonical | `/nicklinney/knowledge-management/document-control-and-publication-standard` |
| Document Naming and Ownership Standard | Standard | Canonical | `/nicklinney/knowledge-management/document-naming-and-ownership-standard` |
| Enterprise Document Register Schema | Schema Standard | Canonical | `/nicklinney/knowledge-management/enterprise-document-register-schema` |
| Chat-Generated Artifact Recovery Procedure | Procedure | Canonical | `/nicklinney/knowledge-management/chat-generated-artifact-recovery-procedure` |
| Canonical Source Declaration Record Standard | Standard | Canonical | `/nicklinney/knowledge-management/canonical-source-declaration-record-standard` |
| Enterprise Document Register | Register | Canonical | `/nicklinney/knowledge-management/enterprise-document-register` |
| Retrieved Project Source Reconciliation | Reconciliation Record | Canonical | `/nicklinney/knowledge-management/retrieved-project-source-reconciliation` |
| Enterprise Document Register Machine-Readable Companion | Structured Register Companion | Canonical | `/nicklinney/knowledge-management/enterprise-document-register-machine-readable-companion` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| Enterprise Document Inventory and Artifact Register | Upstream enterprise inventory source. |
| Software Documentation and Repository Architecture Standard | Shared structural standard. |
| Module Registry | Shared module boundary and classification source. |

Immediate missing minimum objects:

- approval-authority registry
- formal document-object lifecycle workflow record
- per-module recovery playbooks for remaining low-documentation modules

### NickLinney.Modules

Procedural posture: registry baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| Module Directory | User-Facing Directory | Canonical | `/nicklinney/modules` |
| NickLinney.Modules Canonical Module Registry | Canonical Module Registry | Reviewed | `/nicklinney/modules/canonical-module-registry` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| Module Registry | Formal governance-side module registry. |
| NickLinney.KnowledgeManagement Enterprise Document Register | Structured record system for module-owned artifacts. |

Immediate missing minimum objects:

- dedicated module landing page distinct from the directory
- executive abstract for `NickLinney.Modules`
- lifecycle-state and ownership schema for module records

### NickLinney.Ops

Procedural posture: initial recovered baseline.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| Virtual Cybernetic Enterprise Production Manual and SOP Guide | Operating Manual / SOP | Reviewed | `/nicklinney/ops/virtual-cybernetic-enterprise-production-manual-and-sop-guide` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| Organizational Cadence and Enterprise Reporting Standard | Shared reporting and cadence governance. |
| Executive and Cabinet Meeting Record Standard | Shared meeting-record control model. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- incident, observability, and service-governance records

### NickLinney.SecOps

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- monitoring, detection, and incident-response standards

### NickLinney.Security

Procedural posture: initial recovered baseline.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| Safety and Assurance Charter | Constitutional Charter | Reviewed | `/nicklinney/security/safety-and-assurance-charter` |
| Risk Classification Framework | Framework Standard | Reviewed | `/nicklinney/security/risk-classification-framework` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| Good Faith Diligence Rule | Shared governance and due-diligence principle. |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition and scope summary. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- policy hierarchy and control-family index

### NickLinney.SoftwareFactory

Procedural posture: cross-module references only.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| Guide and Standards | Engineering philosophy and lifecycle doctrine aligned with software-factory concerns. |
| Virtual Cybernetic Enterprise Production Manual and SOP Guide | Shared operating doctrine with software production implications. |
| NickLinney Agentic Development Strategy | Strategic framing of the broader software-factory vision. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- production-methodology standards set
- lifecycle and release-governance records

### NickLinney.Strategy

Procedural posture: initial recovered baseline.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| Constitutional Objective / Goal 1 | Strategic Objective | Reviewed | `/nicklinney/strategy/constitutional-objective-goal-1` |
| NickLinney Cybernetic Vision | Vision Document | Reviewed | `/nicklinney/strategy/nicklinney-cybernetic-vision` |
| NickLinney Agentic Development Strategy | Strategy | Reviewed | `/nicklinney/strategy/nicklinney-agentic-development-strategy` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Portfolio and architectural context. |
| Portfolio Model and Context Management | Shared governance framing for portfolio boundaries. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- portfolio-governance or roadmap records specific to `NickLinney.Strategy`

### NickLinney.AutoGit

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- Git workflow standard
- repository lifecycle and release-governance records

### NickLinney.YubiKey

Procedural posture: no direct module objects yet.

Direct objects: none.

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- module landing page
- executive abstract
- hardware-trust and identity standards set
- operational enrollment and recovery procedures

## Shared Enterprise Objects Not Counted As Direct Module Objects

These pages support the portfolio broadly and should remain visible in planning, but are not counted as direct objects of a single module in this baseline:

- `/home`
- `/nicklinney`
- `/nicklinney/governance/*`
- `/nicklinney/templates/*`

## Procedural Next Step Order

To continue definitively and procedurally, the next-pass module work should be prioritized in this order:

1. Modules with zero direct objects but canonical status: `NickLinney.Contracts`, `NickLinney.DataInfrastructure`, `NickLinney.DevOps`, `NickLinney.env`, `NickLinney.SecOps`, `NickLinney.AutoGit`, `NickLinney.YubiKey`, and `System`.
2. Modules with partial recovery only: `NickLinney.System`, `NickLinney.Ops`, `NickLinney.Security`, and `NickLinney.SoftwareFactory`.
3. Modules with early baseline but still incomplete direct object sets: `NickLinney.Agents`, `NickLinney.Modules`, and `NickLinney.Strategy`.
4. Knowledge-management control refinement work that supports all later passes.

## Related Pages

- [NickLinney.KnowledgeManagement](/nicklinney/knowledge-management)
- [Enterprise Document Register](/nicklinney/knowledge-management/enterprise-document-register)
- [NickLinney.Modules Canonical Module Registry](/nicklinney/modules/canonical-module-registry)
- [Module Directory](/nicklinney/modules)