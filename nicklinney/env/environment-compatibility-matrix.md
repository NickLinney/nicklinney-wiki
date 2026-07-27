---
title: Environment Compatibility Matrix
description: Structured compatibility record for supported operating systems, shells, runtimes, and tooling profiles within NickLinney.env.
published: true
date: 2026-07-27T11:29:49.155Z
tags: record, env, compatibility, matrix
editor: markdown
dateCreated: 2026-07-27T11:29:49.155Z
---

# Environment Compatibility Matrix

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native structured record
- Created: July 27, 2026
- Owning Module: `NickLinney.env`

## Purpose

This page defines the minimum structure for recording environment compatibility across supported workstation and tooling combinations.

## Minimum Matrix Dimensions

- operating system
- shell profile
- language runtime
- package manager
- provisioning method
- support posture

## Governance Rule

Compatibility should be treated as an explicit governed record rather than an implicit assumption.

## Baseline Record Structure

Each supported environment profile should declare:

- profile identifier
- platform
- supported versions
- required bootstrap method
- known limitations
- last validation date

## Related Pages

- [NickLinney.env](/nicklinney/env)
- [Bootstrap and Provisioning Standard](/nicklinney/env/bootstrap-and-provisioning-standard)
- [Enterprise Document Register Machine-Readable Companion](/nicklinney/knowledge-management/enterprise-document-register-machine-readable-companion)