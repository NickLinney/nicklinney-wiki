---
title: Information Lifecycle Governance Record
description: Governance record defining the baseline lifecycle states and control expectations for enterprise information objects.
published: true
date: 2026-07-27T11:28:50.753Z
tags: governance, record, data-infrastructure, lifecycle
editor: markdown
dateCreated: 2026-07-27T11:28:50.753Z
---

# Information Lifecycle Governance Record

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native governance artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.DataInfrastructure`

## Purpose

This governance record defines the baseline lifecycle model for information objects managed across the ecosystem.

## Lifecycle States

The minimum lifecycle states are:

- proposed
- active
- reviewed
- superseded
- archived
- retired

## Control Expectations

For each lifecycle state, the object should have clear expectations for:

- mutability
- approval authority
- discoverability
- retention posture
- replacement or supersession handling

## Governance Rule

Information should not move between lifecycle states implicitly. State transition should occur through an identifiable review or publication action.

## Implementation Note

This record complements, but does not replace, module-specific retention or control procedures.

## Related Pages

- [NickLinney.DataInfrastructure](/nicklinney/data-infrastructure)
- [Metadata and Indexing Standard](/nicklinney/data-infrastructure/metadata-and-indexing-standard)
- [Document Control and Publication Standard](/nicklinney/knowledge-management/document-control-and-publication-standard)