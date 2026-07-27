---
title: Risk Classification Framework
description: Recovered operational assurance framework defining assurance levels, evidence requirements, approval authorities, and reclassification rules across the NickLinney.* ecosystem.
published: true
date: 2026-07-27T10:18:31.954Z
tags: nicklinney, security, assurance, risk, framework
editor: markdown
dateCreated: 2026-07-27T10:18:31.954Z
---

# Risk Classification Framework

## Recovery Status

- Status: Reviewed
- Canonicality: Candidate Canonical
- Recovery basis: retrieved ChatGPT export corpus
- Recovery date: July 27, 2026
- Companion document: [Safety and Assurance Charter](/nicklinney/security/safety-and-assurance-charter)

## Executive Statement

This framework operationalizes the constitutional assurance philosophy established by the Safety and Assurance Charter.

Every governed component in the NickLinney.* ecosystem should possess an explicit and documented risk classification.

Risk classification determines:

- required assurance activities
- required documentation
- required testing
- required approvals
- required monitoring
- deployment authority
- operational constraints
- review cadence

The greater the credible consequence of failure, compromise, misuse, or emergent behavior, the greater the required level of assurance.

## Purpose

The framework exists to ensure that assurance activities are:

- proportional
- repeatable
- auditable
- deterministic
- organization-wide

Risk classifications are assigned according to the Principle of Maximum Risk rather than development effort, convenience, schedule pressure, or politics.

## Principle of Maximum Risk

Every component should be classified according to the highest reasonably credible consequence that could result from:

- malfunction
- compromise
- misuse
- adversarial abuse
- cascading failures
- emergent behavior
- governance failure
- long-term ecosystem evolution

Intended use alone is never sufficient for classification.

## Risk Assessment Factors

Each assessment should evaluate:

- human safety
- security
- privacy
- operational continuity
- financial impact
- legal and regulatory impact
- reputational impact
- AI autonomy
- systemic dependency
- recoverability
- explainability
- detectability

## Assurance Levels

### AL-0 Experimental

Purpose: research and experimentation.

Typical characteristics:

- isolated
- disposable
- non-production
- no sensitive data
- no autonomous authority

Required controls:

- version control
- basic documentation
- isolated environment

Approval authority: Project Maintainer.

### AL-1 Standard

Purpose: internal productivity software.

Typical characteristics:

- limited operational impact
- authenticated users
- recoverable failures

Required controls include:

- peer review
- automated testing
- SBOM
- dependency scanning
- basic threat assessment

Approval authority: Technical Lead.

### AL-2 Business Critical

Purpose: core business systems.

Typical characteristics:

- production environments
- operational dependencies
- sensitive information

Required controls include:

- formal architecture review
- security review
- threat modeling
- disaster recovery testing
- observability
- change management

Approval authority: Architecture Review Board.

### AL-3 High Assurance

Purpose: critical infrastructure or organizational control systems.

Typical characteristics:

- organization-wide impact
- elevated security exposure
- privileged authority

Required controls include:

- independent security assessment
- hazard analysis
- penetration testing
- supply-chain verification
- reproducible builds
- provenance attestation
- continuous monitoring

Approval authority: NickLinney.Security.

### AL-4 Safety Critical

Purpose: systems capable of influencing high-consequence outcomes.

Examples include:

- autonomous orchestration
- infrastructure control
- production deployment authority
- organizational governance automation

Required controls include:

- formal verification where practical
- Failure Mode and Effects Analysis (FMEA)
- Fault Tree Analysis (FTA)
- safety case
- independent review
- staged deployment
- rollback validation
- operational readiness review

Approval authority: Security Governance Board.

### AL-5 Strategic Restricted

Purpose: exceptional capabilities whose misuse could produce catastrophic consequences.

Examples include:

- unrestricted autonomous agents
- recursive self-modification
- critical infrastructure automation
- advanced dual-use AI
- biosecurity-sensitive capabilities

Required controls include everything required for AL-4 plus:

- executive governance
- independent technical review
- ethics review
- documented justification
- continuous auditing
- explicit operational boundaries
- periodic reauthorization

Approval authority: Executive Governance Council.

Deployment requires unanimous approval.

## Evidence Requirements

The recovered source defines evidence expectations across the assurance ladder, including:

- requirements
- ADRs
- threat models
- hazard analysis
- FMEA
- FTA
- safety case
- security review
- independent review
- verification report
- validation report
- provenance attestation
- SBOM
- audit trail

Higher assurance levels inherit all lower-level requirements.

## Mandatory Review Gates

The recovered source specifies these review gates:

1. Concept Review
2. Architecture Review
3. Risk Classification
4. Threat Assessment
5. Safety Assessment
6. AI Assessment
7. Verification
8. Validation
9. Operational Readiness
10. Deployment Approval
11. Continuous Monitoring
12. Post-Deployment Review

## Risk Reclassification

Risk classification is not permanent.

Reassessment is required when authority, deployment scope, external integrations, AI capability, operating environments, regulations, incident history, or architecture changes materially.

Risk classification should increase automatically when risk rises.

Risk reduction requires documented evidence and formal approval.

## Relationship to Agent Authority

The recovered source distinguishes between:

- Assurance Levels: how much evidence is required
- Agent Authority Levels: what autonomous systems are permitted to do

These mechanisms are complementary but not identical.

## Continuous Assurance

Assurance continues after deployment through ongoing observation of:

- vulnerabilities
- dependency health
- behavioral drift
- model drift
- policy violations
- audit findings
- incident reports
- architecture changes

Operational evidence becomes part of the permanent assurance record.

## Recovery Provenance

Recovered from the retrieved ChatGPT export corpus, including the `nicklinney-security` project chat titled `Risk Classification Framework` and associated transcript export.

## Related Pages

- [Safety and Assurance Charter](/nicklinney/security/safety-and-assurance-charter)
- [Enterprise Document Register](/nicklinney/knowledge-management/enterprise-document-register)
- [Retrieved Project Source Reconciliation](/nicklinney/knowledge-management/retrieved-project-source-reconciliation)