---
title: Per-Module Document Object Inventory Baseline
description: Baseline per-module inventory of current wiki document objects and procedural documentation gaps across the canonical NickLinney.* module set.
published: true
date: 2026-07-28T04:40:56.594Z
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
- Updated: July 28, 2026 after ECEGF publication and Ops module reconciliation

## Purpose

This page establishes the baseline per-module inventory of document objects presently represented in the wiki.

It is intended to support a definitive and procedural documentation program by answering three questions for each canonical module:

1. What separately addressable document objects currently exist?
2. Which of those are direct module objects versus cross-module supporting records?
3. What minimum object set is still missing before the module can be considered procedurally grounded?

## Definition of Document Object

For this baseline, a document object is any separately addressable wiki page intended to function as one of the following:

- module landing page
- executive abstract or executive baseline abstract
- strategy or plan
- standard, procedure, framework, or manual
- ADR or governance record
- register, inventory, structured companion artifact, matrix, taxonomy, policy hierarchy, decision record, lifecycle control, or evidence model

Shared navigation pages, templates, and enterprise-wide hub pages are tracked separately and are not counted as direct module objects unless they are clearly owned by a module.

## Summary Matrix

| Module | Direct Objects | Cross-Module Supporting Objects | Procedural Posture |
| --- | ---: | ---: | --- |
| `NickLinney.System` | 1 | 2 | Partial recovery only |
| `System` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.Agents` | 3 | 4 | Early baseline established |
| `NickLinney.Contracts` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.DataInfrastructure` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.DevOps` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.env` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.KnowledgeManagement` | 13 | 3 | Strong operational baseline |
| `NickLinney.Modules` | 2 | 2 | Registry baseline established |
| `NickLinney.Ops` | 17 | 2 | ECEGF governance baseline established |
| `NickLinney.SecOps` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.Security` | 2 | 2 | Initial recovered baseline |
| `NickLinney.SoftwareFactory` | 0 | 3 | Cross-module references only |
| `NickLinney.Strategy` | 3 | 2 | Initial recovered baseline |
| `NickLinney.AutoGit` | 8 | 1 | Fourth-layer baseline established |
| `NickLinney.YubiKey` | 8 | 1 | Fourth-layer baseline established |

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

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| System Incubation Project | Project Landing Page | Canonical | `/nicklinney/system-incubation` |
| System Executive Research Baseline | Executive Research Baseline | Canonical | `/nicklinney/system-incubation/executive-research-baseline` |
| Canonical Promotion and Concept Review Procedure | Procedure | Canonical | `/nicklinney/system-incubation/canonical-promotion-and-concept-review-procedure` |
| Research Experiment Index Schema | Schema | Canonical | `/nicklinney/system-incubation/research-experiment-index-schema` |
| Promotion Decision Register | Register | Canonical | `/nicklinney/system-incubation/promotion-decision-register` |
| Research Cluster Taxonomy | Taxonomy | Canonical | `/nicklinney/system-incubation/research-cluster-taxonomy` |
| Experiment Lifecycle and Archival Procedure | Lifecycle Procedure | Canonical | `/nicklinney/system-incubation/experiment-lifecycle-and-archival-procedure` |
| Promotion Evidence and Supersession Record | Evidence / Supersession Record | Canonical | `/nicklinney/system-incubation/promotion-evidence-and-supersession-record` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Preserves `System` as a distinct research and incubation project. |

Immediate missing minimum objects:

- experiment population records
- thematic research cluster index entries
- concept lineage mappings from incubation to canonical destination artifacts

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

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.Contracts | Module Landing Page | Canonical | `/nicklinney/contracts` |
| NickLinney.Contracts Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/contracts/executive-baseline-abstract` |
| Interface and Schema Taxonomy Standard | Standard | Canonical | `/nicklinney/contracts/interface-and-schema-taxonomy-standard` |
| Contract Review and Approval Procedure | Procedure | Canonical | `/nicklinney/contracts/contract-review-and-approval-procedure` |
| Contract Artifact Register | Register | Canonical | `/nicklinney/contracts/contract-artifact-register` |
| Compatibility and Versioning Policy Hierarchy | Policy Hierarchy | Canonical | `/nicklinney/contracts/compatibility-and-versioning-policy-hierarchy` |
| Contract Exception and Waiver Decision Record | Exception / Decision Record | Canonical | `/nicklinney/contracts/contract-exception-and-waiver-decision-record` |
| Contract Validation Evidence Model | Evidence Model | Canonical | `/nicklinney/contracts/contract-validation-evidence-model` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- dependency and integration register
- contract catalog or schema inventory
- interoperability rollout playbooks for breaking or conditional change classes

### NickLinney.DataInfrastructure

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.DataInfrastructure | Module Landing Page | Canonical | `/nicklinney/data-infrastructure` |
| NickLinney.DataInfrastructure Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/data-infrastructure/executive-baseline-abstract` |
| Metadata and Indexing Standard | Standard | Canonical | `/nicklinney/data-infrastructure/metadata-and-indexing-standard` |
| Information Lifecycle Governance Record | Governance Record | Canonical | `/nicklinney/data-infrastructure/information-lifecycle-governance-record` |
| Governed Storage Class Taxonomy | Taxonomy | Canonical | `/nicklinney/data-infrastructure/governed-storage-class-taxonomy` |
| Data Infrastructure Decision Register | Decision Register | Canonical | `/nicklinney/data-infrastructure/data-infrastructure-decision-register` |
| Synchronization and Replication Control Procedure | Procedure | Canonical | `/nicklinney/data-infrastructure/synchronization-and-replication-control-procedure` |
| Metadata Stewardship and Lineage Evidence Model | Evidence Model | Canonical | `/nicklinney/data-infrastructure/metadata-stewardship-and-lineage-evidence-model` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- reference architecture for governed storage classes
- metadata stewardship operating assignments and population records
- retention, archival, and disposal evidence workflows

### NickLinney.DevOps

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.DevOps | Module Landing Page | Canonical | `/nicklinney/devops` |
| NickLinney.DevOps Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/devops/executive-baseline-abstract` |
| CI/CD and Deployment Governance Standard | Standard | Canonical | `/nicklinney/devops/cicd-and-deployment-governance-standard` |
| Release Control and Rollback Procedure | Procedure | Canonical | `/nicklinney/devops/release-control-and-rollback-procedure` |
| Deployment Target Matrix | Matrix | Canonical | `/nicklinney/devops/deployment-target-matrix` |
| DevOps Change Decision Register | Decision Register | Canonical | `/nicklinney/devops/devops-change-decision-register` |
| Infrastructure as Code Control Procedure | Procedure | Canonical | `/nicklinney/devops/infrastructure-as-code-control-procedure` |
| Deployment Validation Evidence Model | Evidence Model | Canonical | `/nicklinney/devops/deployment-validation-evidence-model` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- deployment exception register
- environment-specific release runbooks
- service verification and production acceptance evidence linkage

### NickLinney.env

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.env | Module Landing Page | Canonical | `/nicklinney/env` |
| NickLinney.env Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/env/executive-baseline-abstract` |
| Bootstrap and Provisioning Standard | Standard | Canonical | `/nicklinney/env/bootstrap-and-provisioning-standard` |
| Environment Compatibility Matrix | Structured Record | Canonical | `/nicklinney/env/environment-compatibility-matrix` |
| Managed Toolchain Profile Register | Register | Canonical | `/nicklinney/env/managed-toolchain-profile-register` |
| Environment Governance Decision Record | Decision Record | Canonical | `/nicklinney/env/environment-governance-decision-record` |
| Runtime and Package Management Policy | Policy | Canonical | `/nicklinney/env/runtime-and-package-management-policy` |
| Environment Recovery and Support Exception Procedure | Procedure | Canonical | `/nicklinney/env/environment-recovery-and-support-exception-procedure` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- explicit support-exception register
- managed profile population records
- environment verification evidence for supported baseline profiles

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
| Per-Module Document Object Inventory Baseline | Inventory Baseline | Canonical | `/nicklinney/knowledge-management/per-module-document-object-inventory-baseline` |

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
| Enterprise Document Register | Structured record system for module-owned artifacts. |

Immediate missing minimum objects:

- dedicated module landing page distinct from the directory
- executive abstract for `NickLinney.Modules`
- lifecycle-state and ownership schema for module records

### NickLinney.Ops

Procedural posture: ECEGF governance baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.Ops | Module Landing Page | Canonical | `/nicklinney/ops` |
| Enterprise Capability Evaluation and Governance Framework (ECEGF) | Framework Hub | Canonical | `/nicklinney/ops/enterprise-capability-evaluation-and-governance-framework` |
| NickLinney.Ops - Operational Charter | Charter | Canonical | `/nicklinney/ops/ecegf/operational-charter` |
| NickLinney.Ops - Capability Evaluation and Reporting Standards SOP | Standard Operating Procedure | Canonical | `/nicklinney/ops/ecegf/capability-evaluation-and-reporting-standards-sop` |
| NickLinney.Ops - An Implementor's Guide to Evaluating for SICAF | Implementor Guide | Canonical | `/nicklinney/ops/ecegf/implementors-guide-to-evaluating-for-sicaf` |
| NickLinney.Ops - An Implementor's Guide to Evaluating for RCMF | Implementor Guide | Canonical | `/nicklinney/ops/ecegf/implementors-guide-to-evaluating-for-rcmf` |
| NickLinney.Ops - SICAF Assessment Report | Assessment Report Template | Canonical | `/nicklinney/ops/ecegf/sicaf-assessment-report` |
| NickLinney.Ops - RCMF Assessment Report | Assessment Report Template | Canonical | `/nicklinney/ops/ecegf/rcmf-assessment-report` |
| NickLinney.Ops - An Implementor's Guide for Preparing an RCMF vs. SICAF Capability Gap Report | Implementor Guide | Canonical | `/nicklinney/ops/ecegf/implementors-guide-for-preparing-rcmf-vs-sicaf-capability-gap-report` |
| NickLinney.Ops - RCMF vs. SICAF Capability Gap Report | Comparative Assessment Report | Canonical | `/nicklinney/ops/ecegf/rcmf-vs-sicaf-capability-gap-report` |
| NickLinney.Ops - Considerations for Development of Action Planning after Capability Gap Reporting | Planning Guidance | Canonical | `/nicklinney/ops/ecegf/considerations-for-development-of-action-planning-after-capability-gap-reporting` |
| NickLinney.Ops - RCMF vs. SICAF Capability Gap Report and Action Plan | Executive Action Plan | Canonical | `/nicklinney/ops/ecegf/rcmf-vs-sicaf-capability-gap-report-and-action-plan` |
| NickLinney.Ops - Capability Improvement Register | Register | Canonical | `/nicklinney/ops/ecegf/capability-improvement-register` |
| NickLinney.Ops - Publication Release ADR Event | ADR Event | Canonical | `/nicklinney/ops/ecegf/publication-release-adr-event` |
| NickLinney.Ops - Publication Release Change Event | Change Event | Canonical | `/nicklinney/ops/ecegf/publication-release-change-event` |
| NickLinney.Ops - Publication Release Release Event | Release Event | Canonical | `/nicklinney/ops/ecegf/publication-release-release-event` |
| Virtual Cybernetic Enterprise Production Manual and SOP Guide | Operating Manual / SOP | Reviewed | `/nicklinney/ops/virtual-cybernetic-enterprise-production-manual-and-sop-guide` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| Organizational Cadence and Enterprise Reporting Standard | Shared cadence and reporting governance aligned with operating review routines. |
| Executive and Cabinet Meeting Record Standard | Shared meeting-record control model supporting governance decisions and action review. |

Immediate missing minimum objects:

- populated SICAF and RCMF assessment instances using the new templates
- worked capability-gap and action-plan examples tied to specific governed capability domains
- operational evidence and review-history records showing the ECEGF loop in sustained use

### NickLinney.SecOps

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.SecOps | Module Landing Page | Canonical | `/nicklinney/secops` |
| NickLinney.SecOps Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/secops/executive-baseline-abstract` |
| Monitoring and Detection Engineering Standard | Standard | Canonical | `/nicklinney/secops/monitoring-and-detection-engineering-standard` |
| Incident Response and Escalation Procedure | Procedure | Canonical | `/nicklinney/secops/incident-response-and-escalation-procedure` |
| Security Operations Reporting Matrix | Matrix | Canonical | `/nicklinney/secops/security-operations-reporting-matrix` |
| Security Operations Decision Register | Decision Register | Canonical | `/nicklinney/secops/security-operations-decision-register` |
| Vulnerability Management Lifecycle Standard | Lifecycle Standard | Canonical | `/nicklinney/secops/vulnerability-management-lifecycle-standard` |
| Defensive Automation Exception and Evidence Record | Exception / Evidence Record | Canonical | `/nicklinney/secops/defensive-automation-exception-and-evidence-record` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- security-operations exception register with populated cases
- vulnerability trend and closure analytics model
- control mappings between detection classes and risk authorities

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

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.AutoGit | Module Landing Page | Canonical | `/nicklinney/autogit` |
| NickLinney.AutoGit Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/autogit/executive-baseline-abstract` |
| Operational Git Workflow Standard | Standard | Canonical | `/nicklinney/autogit/operational-git-workflow-standard` |
| Repository Lifecycle and Release Governance Standard | Standard | Canonical | `/nicklinney/autogit/repository-lifecycle-and-release-governance-standard` |
| Repository Stewardship Register | Register | Canonical | `/nicklinney/autogit/repository-stewardship-register` |
| Git Attribution Policy Record | Policy Record | Canonical | `/nicklinney/autogit/git-attribution-policy-record` |
| Release Automation Control Procedure | Procedure | Canonical | `/nicklinney/autogit/release-automation-control-procedure` |
| Repository Exception and Attribution Decision Register | Exception / Decision Register | Canonical | `/nicklinney/autogit/repository-exception-and-attribution-decision-register` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- release evidence population and sample governed releases
- repository classification profile for differing stewardship models
- automation-control mappings to approval authorities

### NickLinney.YubiKey

Procedural posture: fourth-layer baseline established.

Direct objects:

| Object | Class | Status | Path |
| --- | --- | --- | --- |
| NickLinney.YubiKey | Module Landing Page | Canonical | `/nicklinney/yubikey` |
| NickLinney.YubiKey Executive Baseline Abstract | Executive Baseline Abstract | Canonical | `/nicklinney/yubikey/executive-baseline-abstract` |
| Enrollment and Issuance Procedure | Procedure | Canonical | `/nicklinney/yubikey/enrollment-and-issuance-procedure` |
| Recovery and Replacement Procedure | Procedure | Canonical | `/nicklinney/yubikey/recovery-and-replacement-procedure` |
| Hardware Trust Asset Register | Register | Canonical | `/nicklinney/yubikey/hardware-trust-asset-register` |
| YubiKey Trust Policy Hierarchy | Policy Hierarchy | Canonical | `/nicklinney/yubikey/yubikey-trust-policy-hierarchy` |
| Hardware Trust Lifecycle Control Standard | Lifecycle Standard | Canonical | `/nicklinney/yubikey/hardware-trust-lifecycle-control-standard` |
| Trust Exception and Recovery Evidence Record | Exception / Evidence Record | Canonical | `/nicklinney/yubikey/trust-exception-and-recovery-evidence-record` |

Cross-module supporting objects:

| Object | Relationship |
| --- | --- |
| NickLinney.Modules Canonical Module Registry | Canonical module recognition only. |

Immediate missing minimum objects:

- secrets-integration governance record
- operational key-management population records
- trust restoration analytics and bounded emergency-access patterns

## Shared Enterprise Objects Not Counted As Direct Module Objects

These pages support the portfolio broadly and should remain visible in planning, but are not counted as direct objects of a single module in this baseline:

- `/home`
- `/nicklinney`
- `/nicklinney/governance/*`
- `/nicklinney/templates/*`

## Procedural Next Step Order

To continue definitively and procedurally, the next-pass module work should be prioritized in this order:

1. Fourth-layer baseline modules and the newly published Ops framework that now need populated operational records, sample evidence instances, and real control-use objects: `NickLinney.Contracts`, `NickLinney.DataInfrastructure`, `NickLinney.DevOps`, `NickLinney.env`, `NickLinney.Ops`, `NickLinney.SecOps`, `NickLinney.AutoGit`, `NickLinney.YubiKey`, and `System`.
2. Modules with partial recovery only: `NickLinney.System`, `NickLinney.Security`, and `NickLinney.SoftwareFactory`.
3. Modules with early baseline but still incomplete direct object sets: `NickLinney.Agents`, `NickLinney.Modules`, and `NickLinney.Strategy`.
4. Knowledge-management control refinement work that supports later procedural population and versioned evidence handling.

## Related Pages

- [NickLinney.KnowledgeManagement](/nicklinney/knowledge-management)
- [Enterprise Document Register](/nicklinney/knowledge-management/enterprise-document-register)
- [NickLinney.Modules Canonical Module Registry](/nicklinney/modules/canonical-module-registry)
- [Module Directory](/nicklinney/modules)