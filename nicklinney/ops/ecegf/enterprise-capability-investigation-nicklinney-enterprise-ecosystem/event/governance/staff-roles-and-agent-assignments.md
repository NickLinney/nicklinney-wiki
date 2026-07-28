---
title: Staff Roles and Agent Assignments
description: Business Design-based staffing model and pod assignment record for the Enterprise Capability Investigation.
published: true
date: 2026-07-28T06:15:20.428Z
tags: ops, agents, enterprise, ecegf, investigation, staffing
editor: markdown
dateCreated: 2026-07-28T06:15:20.428Z
---

# Staff Roles and Agent Assignments

## Metadata

| Field | Value |
| --- | --- |
| Record ID | ECI-NEE-STAFF-001 |
| Parent Event | ECI-NEE-2026-07-28-01 |
| Status | Active |
| Date | July 28, 2026 |

## Business Design Basis

This staffing model follows the NickLinney Business Design patterns already established in the enterprise corpus:

- Governance is treated as a deterministic synchronization function
- Departments maintain recurring reporting obligations
- Enterprise Architecture operates in a judicial rather than execution role
- Operations, Security, Architecture, Strategy, and Marketing each hold distinct interpretive responsibilities
- One operational event may be coordinated across multiple functions when both execution and narrative value matter

## Required Investigation Roles

| Role | Primary responsibility | Assigned execution model |
| --- | --- | --- |
| Executive Sponsor | Authorizes scope, accepts material conclusions, preserves strategic alignment | Main agent acting on behalf of the event sponsor |
| Governance Lead | Maintains ECEGF compliance, artifact quality, and package completeness | Main agent |
| Enterprise Architect Reviewer | Protects scope boundaries, capability framing, and architectural coherence | Assigned sub-agent |
| Operations Assessment Lead | Evaluates operational maturity and workflow evidence | Assigned sub-agent |
| Security and Assurance Reviewer | Evaluates risk, controls, and evidence discipline across all modules | Assigned sub-agent |
| Knowledge and Evidence Curator | Consolidates source evidence and confidence notes | Main agent plus sub-agent support |
| Marketing Case Study Steward | Preserves the outputs as reusable narrative and proof assets | Main agent during synthesis |
| Module Assessment Pods | Produce module packages in bounded write scopes | Assigned sub-agents |

## Assessment Pod Structure

To keep write scopes separate and parallelizable, the module packages are grouped into five pods:

| Pod | Module set | Primary emphasis |
| --- | --- | --- |
| Pod A | NickLinney.System, SyntheOS, NickLinney.Agents, NickLinney.DataInfrastructure | Theory, cognition, and information substrate |
| Pod B | NickLinney.SoftwareFactory, NickLinney.DevOps, NickLinney.SoftwareDevelopment, NickLinney.AutoGit, NickLinney.env | Engineering and delivery systems |
| Pod C | NickLinney.Ops, NickLinney.Security, NickLinney.SecOps, NickLinney.YubiKey, NickLinney.InfrastructureHosting | Operations, resilience, and assurance |
| Pod D | NickLinney.Strategy, NickLinney.BusinessDesign, NickLinney.Modules, NickLinney.KnowledgeManagement, NickLinney.Comms | Strategy, governance, registry, and knowledge/reporting systems |
| Pod E | NickLinney.Contracts, NickLinney.Software | Asset, contract, and enterprise object stewardship |

## Assignment Rules

- Each pod agent must write only inside its assigned module directories under `01_Module_Assessments`
- Each pod agent must generate the full module package for every assigned module
- Each pod agent must score conservatively when evidence is thin
- Each pod agent must explicitly call out whether a finding is based on direct evidence, adjacent evidence, or observable absence
- The main agent remains the final reviewer and integrator for all pod outputs