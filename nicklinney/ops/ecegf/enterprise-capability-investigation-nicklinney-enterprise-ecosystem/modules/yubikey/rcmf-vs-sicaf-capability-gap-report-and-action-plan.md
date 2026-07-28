---
title: NickLinney.YubiKey - RCMF vs. SICAF Capability Gap Report and Action Plan
description: NickLinney.YubiKey - RCMF vs. SICAF Capability Gap Report and Action Plan
published: true
date: 2026-07-28T06:34:47.174Z
tags: nicklinney, ops, yubikey, ecegf, investigation
editor: markdown
dateCreated: 2026-07-28T06:34:47.174Z
---

# NickLinney.YubiKey - RCMF vs. SICAF Capability Gap Report and Action Plan

## Metadata

| Field | Value |
| --- | --- |
| Parent Event | ECI-NEE-2026-07-28-01 |
| Module | NickLinney.YubiKey |
| Report Date | July 28, 2026 |
| Assessment Basis | SICAF strategic-design assessment plus re-baselined RCMF realization assessment |
| Realization Standard | Only explicit evidence of deployed-and-active operation, or artifacts that clearly prove such reality, count as realization |

## Executive Summary

NickLinney.YubiKey currently presents a **low** gap between strategic design maturity and realized operational maturity. SICAF indicates a design position of **1 / 5**, while the re-baselined RCMF position is **1 / 5** under a realization status of **In Progress / Not Realized**. The module cannot be treated as a dependable enterprise runtime dependency until stronger realization evidence exists.

## Comparative Position

| Measure | Result |
| --- | --- |
| SICAF overall | 1 / 5 |
| RCMF overall | 1 / 5 |
| Realization status | In Progress / Not Realized |
| Gap severity | Low |
| Planning priority | Planned |

## Realization Interpretation

| Field | Position |
| --- | --- |
| Current evidentiary conclusion | The module is conceptually defined, but no direct evidentiary object proves active deployment or use. |
| Governance effect | Design intent may be acknowledged, but runtime maturity may only be credited where realization is actually proven |
| Planning implication | Module-level actions should focus on evidence, bounded execution, and honest status management rather than optimistic expansion |

## Principal Gap Areas

| Gap area | Current condition | Target condition | Priority |
| --- | --- | --- | --- |
| Realization proof | Current operational claims are limited by the available evidence corpus | Realization status is supported by direct evidentiary objects and reviewable artifacts | Planned |
| Ownership and control evidence | Module governance and runtime evidence remain thinner than strategic design intent | Named ownership and repeatable evidence support dependable governance | Planned |
| Reporting and closed-loop review | Improvement can be described, but is not always strongly evidenced as a recurring control cycle | Reviews, updates, and closure decisions are recorded consistently | Planned |

## Risk Implication

If this module is treated as more operationally mature than the evidence allows, the enterprise may introduce dependency drift, false confidence, and unreliable cross-module planning assumptions.

## Recommended Disposition

Remediate from a non-realized baseline.

## Action Planning Position

This plan intentionally reuses the existing module action logic and reinterprets it through the stricter realization baseline. No new improvement track is introduced unless required by the realization rule itself.

## Active Workstreams

| Workstream | Objective | Expected outcome |
| --- | --- | --- |
| Realization and evidence discipline | Align module status with provable runtime evidence | More defensible maturity claims |
| Governance baseline | Preserve or clarify ownership, boundaries, and decision rights | Lower ambiguity and stronger accountability |
| Reporting cadence | Improve repeatability of reviewable outputs | Better enterprise-level synthesis inputs |

## Module Action Plan

| Timeframe | Action | Owner | Success measure |
| --- | --- | --- | --- |
| 0-30 days | Publish a scope note and standard for hardware identity use | Capability owner | Scope, ownership, and governance baseline are published |
| 0-30 days | Define minimum evidence requirements for this module | Governance Lead | Evidence standard is documented |
| 31-60 days | Define enrollment, recovery, rotation, and evidence requirements | Operations Lead | First module evidence pack is available |
| 31-90 days | Pilot the capability against one internal identity workflow | Capability owner | Review cadence is operating with logged outputs |

## Decision Logic

- Preserve the current module scope and do not broaden claims beyond the evidence.
- Treat SICAF as the design target and RCMF as the realized condition.
- Prefer evidence completion and controlled realization over feature expansion.
- Reassess after the module can present stronger direct realization proof.