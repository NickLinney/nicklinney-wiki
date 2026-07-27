---
title: Metadata and Indexing Standard
description: Standard defining metadata expectations, indexing fields, and discoverability rules for enterprise information objects.
published: true
date: 2026-07-27T11:28:49.639Z
tags: standard, metadata, data-infrastructure, indexing
editor: markdown
dateCreated: 2026-07-27T11:28:49.639Z
---

# Metadata and Indexing Standard

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native standards-layer artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.DataInfrastructure`

## Purpose

This standard defines the minimum metadata and indexing expectations required for durable information retrieval across the ecosystem.

## Minimum Metadata Domains

Every governed information object should support as applicable:

- identity metadata
- ownership metadata
- classification metadata
- lifecycle metadata
- relationship metadata
- provenance metadata
- discoverability metadata

## Minimum Core Fields

- stable identifier
- title
- owning module
- object class
- status
- canonicality
- created date
- modified date
- supersession linkages
- related object references

## Indexing Rule

Information objects should be indexable by at least:

- owning module
- object class
- lifecycle status
- canonicality status
- approval authority where applicable

## Governance Principle

If an object cannot be described and found through structured metadata, it should not be treated as institutionally reliable.

## Related Pages

- [NickLinney.DataInfrastructure](/nicklinney/data-infrastructure)
- [Information Lifecycle Governance Record](/nicklinney/data-infrastructure/information-lifecycle-governance-record)
- [Enterprise Document Register Schema](/nicklinney/knowledge-management/enterprise-document-register-schema)