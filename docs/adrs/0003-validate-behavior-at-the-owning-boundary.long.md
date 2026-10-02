# ADR-0003: Validate behavior at the owning boundary

ID: ADR-0003
Title: Validate behavior at the owning boundary
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: quality-delivery
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Long

Variants: [Short](0003-validate-behavior-at-the-owning-boundary.short.md) · [Long, canonical](0003-validate-behavior-at-the-owning-boundary.long.md) · [Guide](0003-validate-behavior-at-the-owning-boundary.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

Use focused tests for pure behavior, integration or contract tests for trust and I/O boundaries, and production-like end-to-end proof for critical journeys. Isolate mutable state, control time and network effects, and assert observable outcomes. A blocking gate needs a deterministic check, clear scope, negative fixtures, actionable failures, and an owner. Report source/static, local, CI, publication/install, deployed/production, and external/third-party evidence separately.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
