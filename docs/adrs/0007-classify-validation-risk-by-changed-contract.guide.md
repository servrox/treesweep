# ADR-0007: Classify validation risk by changed contract — Guide

ID: ADR-0007
Title: Classify validation risk by changed contract
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: quality-delivery
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Guide

Variants: [Short](0007-classify-validation-risk-by-changed-contract.short.md) · [Long, canonical](0007-classify-validation-risk-by-changed-contract.long.md) · [Guide](0007-classify-validation-risk-by-changed-contract.guide.md)

This guide is non-normative. The Long variant is canonical.

## First use

Use the receipt fields in docs/architecture/receipts/. Check candidate, harness, stage, environment, freshness, and invalidators before reuse. Report skipped or unavailable proof as such.

## Provenance

Adapted from Architecture Compass AC-ADR-049; see [provider mapping](../architecture/provider-mapping.md). Provider acceptance does not accept this local proposal.
