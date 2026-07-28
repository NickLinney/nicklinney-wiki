---
title: NickLinney.Ops - An Implementor's Guide to Evaluating for RCMF
description: Implementor guide defining the minimum viable method for evaluating enterprise capabilities through the Runtime Capability Maturity Framework.
published: true
date: 2026-07-28T04:27:51.528Z
tags: ops, ecegf, guide, rcmf
editor: markdown
dateCreated: 2026-07-28T04:27:51.528Z
---

# NickLinney.Ops - An Implementor's Guide to Evaluating for RCMF

## Metadata

| Field | Value |
| --- | --- |
| Document ID | ECEGF-004 |
| Document Type | Implementor Guide |
| Category | Assessment Methodologies |
| Status | Approved |
| Version | 1.0 |
| Effective Date | July 28, 2026 |
| Last Updated | July 28, 2026 |
| Owner | Governance Lead |
| Approval Authority | Nick Linney or delegated operating authority |
| Publication Release | PR-2026-07-28-01 |

## Purpose

This guide defines the minimum viable method for evaluating enterprise capabilities through the Runtime Capability Maturity Framework (RCMF). RCMF is used to assess whether a capability works in practice, is controlled in operation, and produces reliable outcomes in the running environment.

## Scope

RCMF applies to capabilities already in use or partially deployed. It is appropriate for operational reviews, post-implementation evaluations, service stabilization efforts, control assessments, and periodic maturity reviews of established capabilities.

## Core Position

RCMF evaluates operational maturity and running reality. It asks whether the capability is actually being performed, governed, measured, and sustained in the way the enterprise depends on.

## Principles

- Evaluate observable operation rather than intended design.
- Use live evidence whenever possible.
- Distinguish isolated success from repeatable performance.
- Treat control effectiveness and service reliability as core maturity signals.
- Report in language that supports management action and prioritization.

## Evaluation Domains

| Domain | Evaluation focus | Typical questions |
| --- | --- | --- |
| Process Execution | Day-to-day performance of work | Is the capability consistently performed as expected? |
| Role Adoption | Accountability in practice | Do owners, operators, and decision-makers act as defined? |
| Control Effectiveness | Risk and compliance operation | Are controls executed, evidenced, and effective? |
| Data and Reporting | Runtime visibility and decision support | Are metrics accurate, timely, and used for management? |
| Technology Reliability | System support in operation | Do tools, integrations, and automations work dependably? |
| Service Management | Incident, change, and issue handling | Can the capability absorb disruption and recover predictably? |
| Continuous Improvement | Learning and corrective action | Are issues tracked, prioritized, and closed through governance? |

## Evidence Expectations

Acceptable evidence should show actual execution, not only policy intent. Preferred evidence includes:

- Operational runbooks, schedules, and service records
- Samples of completed transactions, tickets, approvals, or control logs
- KPI packs, dashboards, trend reports, and exception reporting
- Incident, problem, risk, and change records
- Audit observations, management reviews, and corrective action logs
- User feedback, training records, and adoption measures
- System availability, integration, and performance evidence

Interviews should be used to validate how work is performed and to explain observed variance, but ratings should anchor on records and operational outputs.

## Scoring Approach

Use a five-point scale for each domain.

| Score | Interpretation | Decision meaning |
| --- | --- | --- |
| 1 | Ad Hoc | Activity is inconsistent, informal, or largely dependent on individuals |
| 2 | Repeatable | Basic routines exist but are weakly controlled or unevenly applied |
| 3 | Established | The capability operates consistently with defined management oversight |
| 4 | Controlled | Performance, controls, and reporting are reliable and actively managed |
| 5 | Adaptive | The capability is resilient, measured, and continuously improved |

Score according to sustained evidence, not best-case examples. If the capability performs well only in selected teams or time periods, score to the level that best reflects normal enterprise operation.

## Workflow

| Step | Activity | Output |
| --- | --- | --- |
| 1 | Confirm operational scope, service boundary, and stakeholders | Assessment charter note |
| 2 | Collect runtime evidence and sampling approach | Evidence register |
| 3 | Evaluate maturity by domain using records and observation | Working assessment notes |
| 4 | Calibrate scores and identify operational risks | Draft scorecard |
| 5 | Summarize root causes, constraints, and improvement priorities | Issue summary |
| 6 | Prepare the RCMF Assessment Report | Executive-ready report |
| 7 | Review outcomes in governance and operational forums | Approved findings and follow-up actions |

## Deliverables

- Completed RCMF domain scorecard
- Evidence register with sample references
- Summary of operating strengths, failure points, and risks
- RCMF Assessment Report

## Review Cadence

- After initial go-live stabilization
- Semiannually for critical or high-risk capabilities
- Annually for stable capabilities
- Following major incidents, audit findings, control failures, or significant platform change

## Reporting Expectations

The companion RCMF Assessment Report should be concise, standardized, and executive-friendly. It should highlight actual operating maturity, confirm the reliability of evidence, identify operational breakdowns, and recommend clear management actions.