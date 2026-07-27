---
title: Recovery and Replacement Procedure
description: Procedure for loss, compromise, rotation, replacement, and trust re-establishment for YubiKey-backed identity assets.
published: true
date: 2026-07-27T11:29:56.029Z
tags: recovery, procedure, yubikey, replacement
editor: markdown
dateCreated: 2026-07-27T11:29:56.029Z
---

# Recovery and Replacement Procedure

## Status

- Status: Canonical
- Canonicality: Canonical
- Origin: Wiki-native procedure artifact
- Created: July 27, 2026
- Owning Module: `NickLinney.YubiKey`

## Purpose

This procedure defines the minimum response model for lost, compromised, rotated, or replaced hardware trust devices.

## Procedure

1. Declare the loss, compromise, or planned replacement event.
2. Assess immediate trust and access impact.
3. Revoke or disable affected trust relationships where appropriate.
4. Provision replacement hardware under controlled issuance rules.
5. Re-establish the required trust functions.
6. Record the transition and any residual risk posture.

## Minimum Record Elements

- event type
- affected identity or role
- revocation or disablement action
- replacement device reference
- recovery completion status
- approving authority

## Related Pages

- [NickLinney.YubiKey](/nicklinney/yubikey)
- [Enrollment and Issuance Procedure](/nicklinney/yubikey/enrollment-and-issuance-procedure)
- [Risk Classification Framework](/nicklinney/security/risk-classification-framework)