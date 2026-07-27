---
title: Enrollment and Issuance Procedure
description: Procedure for controlled enrollment, issuance, initialization, and assignment of YubiKey-backed trust credentials.
published: true
date: 2026-07-27T11:29:54.817Z
tags: procedure, yubikey, enrollment, issuance
editor: markdown
dateCreated: 2026-07-27T11:29:54.817Z
---

# Enrollment and Issuance Procedure

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native procedure artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.YubiKey`

## Purpose

This procedure defines the minimum controlled flow for issuing and enrolling hardware-backed identity devices.

## Procedure

1. Confirm the identity and authorization basis for issuance.
2. Assign the device to an accountable owner or role.
3. Initialize the required trust functions for the authorized use case.
4. Record enrollment metadata and recovery dependency information.
5. Validate successful enrollment and operational usability.
6. Publish or retain the controlled issuance record.

## Minimum Record Elements

- device identifier
- assigned owner or role
- authorized trust functions
- enrollment date
- accountable approver
- recovery dependency notes

## Related Pages

- [NickLinney.YubiKey](/nicklinney/yubikey)
- [Recovery and Replacement Procedure](/nicklinney/yubikey/recovery-and-replacement-procedure)
- [Safety and Assurance Charter](/nicklinney/security/safety-and-assurance-charter)