---
title: Identity and Access Management Initiative Technical Action Plan
description: Technical action plan for moving the IAM initiative from design into execution.
published: true
date: 2026-07-28T19:05:46.567Z
tags: nicklinney, action-plan, identity-access-management, execution
editor: markdown
dateCreated: 2026-07-28T19:05:46.567Z
---

# Identity and Access Management Initiative Technical Action Plan

## Metadata

| Field | Value |
| --- | --- |
| Artifact ID | NLIAM-EXE-002 |
| Initiative ID | NLIAM-2026-07-28-01 |
| Authorizing Roles | Chief Information Officer; PMO Director |
| Date | July 28, 2026 |
| Status | Draft for execution use |

## Executive Basis

This action plan is governed by:

- the `Chief Vision Officer Retrospective`
- the `CVO Design Phase Kickoff Input`
- the `Identity and Access Management Initiative Product Plan`
- the `Identity and Access Management Initiative Project Plan`
- the completed design-phase meeting corpus

The plan is intentionally bounded. It is designed to move the initiative from theory to evidence-bearing implementation without pretending that full enterprise IAM deployment is already justified.

## Action Plan Summary

The initiative will enter execution through a federated IAM service pattern built around:

1. `OpenLDAP` as the initial directory authority and group or role-anchor service
2. `OpenBao` as the initial secrets-control and machine-credential service
3. Wiki-governed publication artifacts for approvals, decisions, and traceability
4. a bounded first implementation slice covering one human approval path and one machine credential path

`Vaultwarden` and `Psono` remain meaningful candidate tools for later human-secret workflow expansion, but they are not selected for the first execution slice because the current CVO-directed need weights machine credential lifecycle, policy control, and agent-capable automation more heavily than convenience-first personal vault workflows.

## Technical Direction

### Selected First-Slice Stack Pattern

- directory authority: `OpenLDAP`
- secrets and policy authority: `OpenBao`
- publication and control records: WikiJS and initiative governance corpus
- machine workflow posture: policy-controlled service authentication and leased credentials

### Reasoning

- `OpenLDAP` is suitable as a directory foundation because it is purpose-built for searchable identity data and supports detailed access control at the directory layer.
- `OpenBao` is suitable for the first slice because its official documentation shows policy-based authorization, multiple authentication methods, machine-oriented `AppRole` support, leased secrets, and auditable request handling.
- `OpenBao` is the stronger first-slice fit than `Vaultwarden` or `Psono` for the current enterprise direction because the CVO explicitly emphasized agentic access, IaC deployment, secure key retrieval, constrained pathways, and trusted service-to-service connectivity.
- `Vaultwarden` and `Psono` should not be discarded. They remain defensible future candidates for more human-centric secret experience layers after the machine-governance spine is proven.

## First Implementation Slice

The first execution slice will prove one governed pathway that includes both a human and a machine control surface:

- a human requester submits an access request for a bounded module resource
- a named module owner and security approver review and approve the request
- the approved role and identity record are represented in the directory authority
- a machine credential is issued through `OpenBao` for one approved automation path
- the request, approval, issuance, and review evidence are retained in named record locations

## Delivery Workstreams

### Workstream 1 - Directory Authority Foundation

- define initial directory schema and naming convention for humans, agents, and service accounts
- define the initial group and role-anchor structure for the first slice
- define administrative and recovery boundaries

### Workstream 2 - Secrets and Machine Credential Control

- stand up a bounded `OpenBao` configuration for policy-controlled access
- define the first machine authentication workflow
- define lease, rotation, and revocation expectations for the selected credential path

### Workstream 3 - Approval and Governance Controls

- publish the draft approval matrix
- define request, approval, exception, and review steps
- confirm evidence locations for each control event

### Workstream 4 - Slice Delivery and Evidence

- implement one end-to-end pilot path
- collect request, approval, issuance, use, and review evidence
- prepare the evidence pack for monitoring and controlling review

## Execution Sequence

1. approve the architecture comparison and first-slice recommendation
2. approve the draft approval matrix and role-to-authority mapping
3. define the initial implementation slice boundary and success criteria
4. stand up the bounded directory and vault control plane
5. execute one governed human-plus-machine access workflow
6. review evidence, exceptions, and required next-cycle changes

## Deliverables

- architecture comparison and recommendation artifact
- approval matrix draft
- initial implementation slice plan
- execution mobilization meeting record
- first-slice control evidence pack

## Assumption Challenges

- The initiative rejects the assumption that a password-manager-first approach is enough for the current enterprise need.
- The initiative rejects the assumption that directory selection alone solves secret issuance, leasing, and machine governance.
- The initiative rejects the assumption that a first slice should span the whole enterprise.
- The initiative rejects the assumption that documentation completion is equivalent to implementation success.

## Risks and Mitigations

| Risk | Mitigation |
| --- | --- |
| Directory and secret services may be designed more broadly than current operations can support | keep the first slice narrow and require explicit operational ownership |
| Human-secret convenience needs may pressure the initiative toward the wrong first product emphasis | preserve Vaultwarden and Psono as later options while prioritizing machine-governance requirements now |
| Execution may drift into platform-building without a user workflow | require one named request-to-issuance pilot path |
| Evidence may remain incomplete even if infrastructure is stood up | treat review artifacts and retained records as mandatory deliverables |