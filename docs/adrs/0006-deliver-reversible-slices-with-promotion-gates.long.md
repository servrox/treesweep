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
Variant: Long

Variants: [Short](0006-deliver-reversible-slices-with-promotion-gates.short.md) · [Long, canonical](0006-deliver-reversible-slices-with-promotion-gates.long.md) · [Guide](0006-deliver-reversible-slices-with-promotion-gates.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

Separate reversible changes from destructive or irreversible steps. Identify the exact artifact and required gate before promotion. Local validation, CI, publication, installation, deployment, production behavior, and external integration are distinct proof stages and authorities.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
