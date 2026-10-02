# ADR-0006: Deliver reversible slices with promotion gates

ID: ADR-0006
Title: Deliver reversible slices with promotion gates
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: quality-delivery
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Short

Variants: [Short](0006-deliver-reversible-slices-with-promotion-gates.short.md) · [Long, canonical](0006-deliver-reversible-slices-with-promotion-gates.long.md) · [Guide](0006-deliver-reversible-slices-with-promotion-gates.guide.md)

## Decision summary

Each delivery slice has a path allowlist, input state, owner, acceptance proof, stop condition, rollback path, and last reversible point. A completed slice does not authorize later promotion.

This proposal is pending maintainer acceptance; it does not authorize implementation.
