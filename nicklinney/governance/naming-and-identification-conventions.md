---
title: Naming and Identification Conventions
description: Portfolio naming and stable-identifier rules for projects, products, and subordinate artifacts.
published: true
date: 2026-07-27T07:51:59.725Z
tags: nicklinney, governance, naming, identifiers
editor: markdown
dateCreated: 2026-07-27T07:51:59.725Z
---

# Naming and Identification Conventions

## Purpose

This page documents the official naming and identification conventions used within the NickLinneyDev portfolio.

The intent is to ensure that products, projects, and feature-level artifacts are:

- unambiguously identifiable
- consistently named
- easy to navigate in filesystem and repository views
- traceable over time without relying on a specific tool

## Core Principle

Stable identifiers are assigned to products or long-lived projects and serve as the root for subordinate feature identifiers.

Identifiers are:

- human-readable
- stable over time
- tooling-independent
- never reused

## Identifier Format

Canonical project or product codes use the pattern:

```text
<CODE>
```

Where `CODE` is:

- 2 to 4 uppercase alphabetic characters
- unique across the portfolio
- chosen once
- never changed

Examples:

- `ENV`
- `SYS`
- `AUD`
- `NET`

## Feature Identifier Format

Feature identifiers use the pattern:

```text
<CODE>-<NUMBER>
```

Examples:

- `ENV-1`
- `ENV-2`
- `SYS-14`

Rules:

- numbering is per code
- numbers increase sequentially
- identifiers are never reused or renumbered
- gaps are acceptable

## Naming Conventions

### Feature Directory Naming

```text
Feature <CODE>-<NUMBER> - <Short Description>
```

### Feature File Naming

```text
<CODE>-<NUMBER> - <Artifact Type> - <Short Description>.md
```

### Product Directory Naming

Products use their canonical product name as the directory name.

The identifier code is defined in the documentation and used for subordinate artifacts rather than as the folder name itself.

## Wiki Relevance

This page should guide naming for future product, project, feature, and standards pages when identifiers are formalized in the wiki.

## Related Pages

- [NickLinney.* Ecosystem](/nicklinney)
- [Portfolio Model and Context Management](/nicklinney/governance/portfolio-model-and-context-management)
