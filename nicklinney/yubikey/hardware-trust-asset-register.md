---
title: Hardware Trust Asset Register
description: Register of governed hardware trust assets, assignment posture, recovery dependencies, and trust-function coverage.
published: true
date: 2026-07-27T22:07:13.007Z
tags: register, yubikey, hardware-trust, assets
editor: markdown
dateCreated: 2026-07-27T22:07:13.007Z
---

# Hardware Trust Asset Register

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native third-layer control artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.YubiKey`

## Purpose

This register records governed hardware-backed trust assets and their operational posture.

## Minimum Record Fields

- asset identifier
- assigned owner or role
- trust functions enabled
- issuance status
- recovery dependency status
- replacement readiness

## Governance Rule

A hardware trust asset should not be treated as operationally governed unless it can be identified, assigned, and reviewed through a controlled record.

## Related Pages

- [NickLinney.YubiKey](/nicklinney/yubikey)
- [Enrollment and Issuance Procedure](/nicklinney/yubikey/enrollment-and-issuance-procedure)
- [YubiKey Trust Policy Hierarchy](/nicklinney/yubikey/yubikey-trust-policy-hierarchy)