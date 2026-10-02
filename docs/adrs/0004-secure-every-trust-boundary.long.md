# ADR-0004: Secure every trust boundary

ID: ADR-0004
Title: Secure every trust boundary
Status: Proposed
Date: 2026-10-02
Owner: treesweep maintainers
Scope: repository
Category: security-data
Supersedes: none
Superseded by: none
Canonical variant: Long
Variant: Long

Variants: [Short](0004-secure-every-trust-boundary.short.md) · [Long, canonical](0004-secure-every-trust-boundary.long.md) · [Guide](0004-secure-every-trust-boundary.guide.md)

## Context

The repository currently has no application architecture or implementation. This proposal establishes a durable guardrail for future scoped work without choosing a stack or product boundary.

## Decision

Before adding a trust boundary, name its owner, principal, allowed action and object, data classification, and failure behavior. Keep secrets out of source, client artifacts, logs, prompts, fixtures, and public reports. Treat model output, retrieved content, and tool arguments as untrusted. High-impact identity, credential, payment, child, health, cross-tenant, destructive, and code-execution paths require manual threat review and negative tests.

## Status and authority

This ADR is Proposed. It becomes binding only when the maintainer explicitly accepts it. An accepted change of intent requires a successor rather than silent edits.

## Consequences

The first implementation must apply this rule at its owning boundary and record evidence. If the product design conflicts with it, resolve the decision before dependent source changes.

## Acceptance

The maintainer reviews the rule against the first concrete implementation slice and explicitly changes its status to Accepted or records a revised proposal.
