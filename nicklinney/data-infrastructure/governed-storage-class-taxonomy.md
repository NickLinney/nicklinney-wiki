---
title: Governed Storage Class Taxonomy
description: Governed taxonomy of storage classes, information forms, and lifecycle expectations for enterprise data assets.
published: true
date: 2026-07-27T22:05:54.914Z
tags: governance, data-infrastructure, taxonomy, storage
editor: markdown
dateCreated: 2026-07-27T22:05:54.914Z
---

# Governed Storage Class Taxonomy

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native third-layer taxonomy artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.DataInfrastructure`

## Purpose

This taxonomy defines the baseline storage classes used to reason about information assets across the ecosystem.

## Storage Classes

- relational
- graph
- vector
- document
- object or blob
- log or event stream
- transient cache

## Governance Rule

Each governed information object should be mappable to one primary storage class and any secondary supporting classes where relevant.

## Lifecycle Consideration

Storage class selection should inform indexing, retention, synchronization, and recoverability expectations.

## Related Pages

- [NickLinney.DataInfrastructure](/nicklinney/data-infrastructure)
- [Information Lifecycle Governance Record](/nicklinney/data-infrastructure/information-lifecycle-governance-record)
- [Data Infrastructure Decision Register](/nicklinney/data-infrastructure/data-infrastructure-decision-register)