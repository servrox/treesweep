# ADR-0002: Assign source ownership and file roles

ID: ADR-0002
Title: Assign source ownership and file roles
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: repository-architecture
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Long

Variants: [Short](0002-assign-source-ownership-and-file-roles.short.md) · [Long, canonical](0002-assign-source-ownership-and-file-roles.long.md) · [Guide](0002-assign-source-ownership-and-file-roles.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

Before implementation, map each planned file to an owner, source role, runtime audience, and caller. Keep framework entrypoints thin; keep generated and infrastructure files distinct from hand-written runtime code. Do not create speculative empty units or pass-through layers. Exact product layout remains undecided until there is an implementation proposal.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
