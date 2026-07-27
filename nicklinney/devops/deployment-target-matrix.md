---
title: Deployment Target Matrix
description: Matrix defining governed deployment target classes, validation expectations, promotion posture, and rollback sensitivity.
published: true
date: 2026-07-27T22:05:57.290Z
tags: devops, deployment, matrix, targets
editor: markdown
dateCreated: 2026-07-27T22:05:57.290Z
---

# Deployment Target Matrix

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native third-layer control artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.DevOps`

## Purpose

This matrix defines the baseline target classes used for governed deployment planning.

## Target Classes

| Target Class | Promotion Sensitivity | Validation Expectation | Rollback Sensitivity |
| --- | --- | --- | --- |
| local or ephemeral | Low | Basic functional validation | Low |
| integration | Medium | Integration validation | Medium |
| staging or pre-release | High | Full pre-release validation | High |
| production | Maximum | Controlled release validation | Maximum |

## Governance Rule

Deployment governance should scale with target criticality. Production and pre-release targets should never be treated as equivalent to ephemeral environments.

## Related Pages

- [NickLinney.DevOps](/nicklinney/devops)
- [Release Control and Rollback Procedure](/nicklinney/devops/release-control-and-rollback-procedure)
- [DevOps Change Decision Register](/nicklinney/devops/devops-change-decision-register)