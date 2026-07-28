---
title: Identity and Access Management Initiative Architecture Comparison and Recommendation
description: Execution-phase architecture comparison and first-slice recommendation for the IAM initiative.
published: true
date: 2026-07-28T19:05:51.034Z
tags: nicklinney, architecture, identity-access-management, execution
editor: markdown
dateCreated: 2026-07-28T19:05:51.034Z
---

# Identity and Access Management Initiative Architecture Comparison and Recommendation

## Metadata

| Field | Value |
| --- | --- |
| Artifact ID | NLIAM-EXE-003 |
| Initiative ID | NLIAM-2026-07-28-01 |
| Date | July 28, 2026 |
| Prepared By | CIO temporary cabinet |
| Status | Draft for execution use |

## Reference Basis

This comparison uses the evaluation criteria adopted during the design phase and supplements them with official product documentation reviewed on July 28, 2026.

Relevant source observations:

- `OpenBao` documents identity-based access, multiple auth methods, path-based policies, deny-by-default enforcement, `AppRole` for machine workflows, and leased or revocable credentials.
- `OpenLDAP` documents directory-oriented access control, schema extensibility, and fine-grained ACL patterns.
- `Vaultwarden` documents organizations, collections, member roles, groups, event logs, and directory connector compatibility, but its published emphasis remains closer to a Bitwarden-compatible self-hosted password-management surface.
- `Psono` documents API-key based secret access patterns, including sessionless options, but its published posture remains more oriented toward secret retrieval and sharing than toward the full machine-governance control model required for the first slice.

## Evaluation Criteria

1. principal-type compatibility
2. RBAC and delegated approval fit
3. machine-credential lifecycle support
4. secrets reviewability
5. recovery and exception handling
6. domain-boundary compatibility
7. operational manageability
8. audit-evidence integration

## Candidate Comparison

| Candidate Direction | Strengths | Concerns | Cabinet Read |
| --- | --- | --- | --- |
| `OpenLDAP` only | strong directory model; mature identity store; flexible ACL concepts | weak as a stand-alone secrets and machine-credential control plane | necessary directory component, insufficient alone |
| `OpenLDAP` + `OpenBao` | strong machine-oriented auth and policy controls; leased credentials; separation of identity and secrets; aligns with human-plus-agent design | higher integration effort than all-in-one convenience tooling | best first-slice fit |
| `OpenLDAP` + `Vaultwarden` | strong human-facing vault experience; org and collection concepts; lighter apparent admin path for personal and team secret use | less well aligned to leased machine credentials and agent-first service workflows | useful later adjunct, weaker first-slice core |
| `OpenLDAP` + `Psono` | credible secret-sharing and API access story; some automation-friendly patterns | less evidence of full first-slice machine-governance depth than `OpenBao`; some documented API-key paths are cautioned against | plausible alternate human-secret path, weaker first-slice core |

## Recommendation

The cabinet recommends:

- approve `OpenLDAP` as the first-slice directory authority
- approve `OpenBao` as the first-slice secrets and machine-credential authority
- defer `Vaultwarden` and `Psono` to later comparison for human-secret workflow augmentation after the first slice is proven

## Why This Recommendation Fits the CVO Direction

The CVO asked for:

- cross-module consumption at every enterprise layer
- secure access requests and constrained approved pathways
- safe evaluation of access needs
- programmatic secure key access
- trusted human and agent operation
- avoidance of not-invented-here design

The `OpenLDAP` plus `OpenBao` direction is the strongest match because it directly addresses directory-backed identity plus machine-capable secret issuance and control, while preserving a federated architecture compatible with the initiative's record, approval, and evidence boundaries.

## Explicit Non-Recommendations for the First Slice

- Do not begin with a vault chosen primarily for human convenience if it weakens machine-governance requirements.
- Do not treat any single tool as the whole IAM solution.
- Do not widen the first implementation slice to enterprise-wide rollout.

## Review Notes

- This recommendation is an inference from the reviewed official sources and the initiative's adopted criteria, not a claim that the products are identical in scope.
- A later implementation cycle may still add a human-oriented vault experience layer if the first slice proves the machine-governance spine successfully.