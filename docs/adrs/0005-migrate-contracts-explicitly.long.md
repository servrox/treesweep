# ADR-0005: Migrate contracts explicitly

ID: ADR-0005
Title: Migrate contracts explicitly
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: quality-delivery
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Long

Variants: [Short](0005-migrate-contracts-explicitly.short.md) · [Long, canonical](0005-migrate-contracts-explicitly.long.md) · [Guide](0005-migrate-contracts-explicitly.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

Use expand, migrate, and contract stages unless an approved atomic boundary proves them unnecessary. Add compatible capacity before moving consumers, then remove old capacity only after verified adoption and a separately authorized gate. Destructive or irreversible steps require explicit authority, recovery evidence, and a stop condition. Change accepted architectural intent through a successor ADR.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
