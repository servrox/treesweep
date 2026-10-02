# ADR-0001: Govern architecture through accepted ADRs

ID: ADR-0001
Title: Govern architecture through accepted ADRs
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: governance
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Long

Variants: [Short](0001-govern-architecture-through-accepted-adrs.short.md) · [Long, canonical](0001-govern-architecture-through-accepted-adrs.long.md) · [Guide](0001-govern-architecture-through-accepted-adrs.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

One canonical index and one durable decision per ADR make intent discoverable. Accepted Long variants govern architecture within authorized work. A new durable decision needs a proposal and maintainer acceptance before dependent implementation. Changing accepted intent requires an accepted successor with reciprocal lineage.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
